## github integration

- git/github is a most amazing tool to track changes and can be used in many more ways than people deem possible.
- We suggest using github for
  - specs
  - documentation
  - planning work (stories in home repo, see [stories](stories.md))
  - tracking of bugs
  - tracking of feature requests
  - of course all coding work using pull requests as tool to track changes
  - tickets from customers (*)
- why
  - its important that all change is being tracked and people get visibility on everything which happened and is going to happen


### requirements

- if security is important to you make sure everyone uses 2-factor authentication
- if possible use clean login names on github, many people use funny names which is nice but makes it hard for people to remember
  - our suggested login names are  $first7lettersLastName+$firsLetterFirstname e.g. Kristof De Spiegeleer becomes *despiegk*



### how to use github (or any other git mgmt system)

### different types of repo's (IMPORTANT)

#### home repo

- is a repo with as name ```home```
- it is the main repo of an organization
- it holds 
  - starting point of documentation
  - explains what other repo's are used & what their purpose is
  - holds specifications which are not related to 1 repo
  - holds info like product PRD, ... which are bigger than 1 repo
- milestones
  - defines a deadline for x nr of stories/tasks
  - a story or task can only belong to 1 deadline
- issue types used
  - story, question, task
- stories are only used in a home repo if they are not scheduled to a milestone yet (same remark for tasks)
    - in other words try NOT to put stories & tasks in this type of repo 
  
#### milestone repo

- ```milestone_$name```
- is a repo which starts with name ```milestone```
- in our development process all effort is organized around milestones
- a milestone holds X nr of stories which need to be finishined within that milestone.
- this repo holds
  - holds the stories as part of the milestone
  - tasks as part of the stories
  - specs/documentation specific to this milestone (NOT TO THE PRODUCT), so related to the process, specs & doc related to product belong in the home or code repo's
  - test plans
- issue types used
  - story, question, task, test
- milestone repo's are also used to group our test effort

#### product code related

- no special convention today, can be any name but NOT starting with the prefixes as described in this doc
- this is where the main code of products live
- milestones
  - freely to be chosen names per repo, they are used to group bugs or features
  - these milestones are then linked to a specific story !!! to get them executed
- issue types used
  - bug, feature, question
- DO NOT
    - use stories or tasks or tests at this level !!! 
- bug/feature management
    - all issues reported or feature requests are grouped, it acts like a funnel    

#### project related

- ```proj_$customer_$projname```
  - projects relate to customers
  - we use this to organize our work related to 1 customer project, only useful if customer project is large enough
  - issues can be leads, tickets, monitoring issues, stories, questions or tasks
- milestones
  - defines a deadline for the project, there can be multiple but tasks or stories can only belong to one
  - freely chosen per project



#### documentation/gitbook

- ```doc_$name```
- IMPORTANT
  - often it makes more sense to leave the documenation inside the product/code repo
  - when put in code repo put under subdir /doc
  - advantage to keep it in a code repo is that documentation is lined to the code
  - the only reason to put it in a separate repo is when the doc is not related to code or related to more than 1 code repo  
- milestones
  - groups features & bugs
- issues can be of type
    - bug,feature,question

#### www = websites

- ```www_$name```
- the code for a website
- when code changes normally a website is updated & hosted automatically
- issues can be of type
    - bug,feature,question

#### cockpit

- ```cockpit_$customer_$name``` e.g. ```infra_gig_gentTest1```
- is used to run an infrastructure from out of GIT
  - it documents a full it env
  - it has all required process information embedded in ays
  - all changes are strictly controlled by git & pull requests 
- is the cockpit env which runs our management framework e.g.
    - ays robot
    - telegram robot
    - rogerthat robot
    - portal
- is used to manage an environment on our G8 grid
- ays repo's are inside
    - there can be more than 1 ays repo hosted inside a cockpit repo 
        - hosts the ays recipes and ays instances which make up the env to be managed
        - is a dir which has an empty file .ays inside 
- milestones
  - defines a deadline for the environment, freely to be chosen
- issues can be of type
    - story, task, bug, feature, question, monitor, test 

#### ays templates (At Your Service)

- an AYS repo starts with ays_ ...
  - ```ays_$customer_$envname``` e.g. ays_gig_gentTest1
- milestones
  - to group feature requests & bugs
- issues can be of type
    - bug,feature,question


### terminology git related

#### Branch

A branch is a parallel version of a repository. It is contained within the repository, but does not affect the primary or master branch allowing you to work freely without disrupting the "live" version. When you've made the changes you want to make, you can merge your branch back into the master branch to publish your changes.

#### Clone

A clone is a copy of a repository that lives on your computer instead of on a website's server somewhere, or the act of making that copy. With your clone you can edit the files in your preferred editor and use Git to keep track of your changes without having to be online. It is, however, connected to the remote version so that changes can be synced between the two. You can push your local changes to the remote to keep them synced when you're online.

#### Collaborator

A collaborator is a person with read and write access to a repository who has been invited to contribute by the repository owner.

#### Commit

A commit, or "revision", is an individual change to a file (or set of files). It's like when you save a file, except with Git, every time you save it creates a unique ID (a.k.a. the "SHA" or "hash") that allows you to keep record of what changes were made when and by who. Commits usually contain a commit message which is a brief description of what changes were made.

#### Contributor

A contributor is someone who has contributed to a project by having a pull request merged but does not have collaborator access.

#### Diff

A diff is the difference in changes between two commits, or saved changes. The diff will visually describe what was added or removed from a file since its last commit.

#### Fetch

Fetching refers to getting the latest changes from an online repository (like GitHub.com) without merging them in. Once these changes are fetched you can compare them to your local branches (the code residing on your local machine).

#### Fork

A fork is a personal copy of another user's repository that lives on your account. Forks allow you to freely make changes to a project without affecting the original. Forks remain attached to the original, allowing you to submit a pull request to the original's author to update with your changes. You can also keep your fork up to date by pulling in updates from the original.

#### Git

Git is an open source program for tracking changes in text files. It was written by the author of the Linux operating system, and is the core technology that GitHub, the social and user interface, is built on top of.


#### Markdown

Markdown is an incredibly simple semantic file format, not too dissimilar from .doc, .rtf and .txt. Markdown makes it easy for even those without a web-publishing background to write prose (including with links, lists, bullets, etc.) and have it displayed like a website. GitHub supports Markdown, and you can learn about the semantics here.

#### Merge

Merging takes the changes from one branch (in the same repository or from a fork), and applies them into another. This often happens as a Pull Request (which can be thought of as a request to merge), or via the command line. A merge can be done automatically via a Pull Request via the GitHub.com web interface if there are no conflicting changes, or can always be done via the command line. See Merging a pull request.


An organization holds X repositories

#### Private Repository

Private repositories are repositories that can only be viewed or contributed to by their creator and collaborators the creator specified.

#### Pull

Pull refers to when you are fetching in changes and merging them. For instance, if someone has edited the remote file you're both working on, you'll want to pull in those changes to your local copy so that it's up to date.

#### Pull Request

Pull requests are proposed changes to a repository submitted by a user and accepted or rejected by a repository's collaborators. Like issues, pull requests each have their own discussion forum. See Using Pull Requests.

#### Push

Pushing refers to sending your committed changes to a remote repository such as GitHub.com. For instance, if you change something locally, you'd want to then push those changes so that others may access them.

#### Remote

This is the version of something that is hosted on a server, most likely GitHub.com. It can be connected to local clones so that changes can be synced.


#### SSH Key

SSH keys are a way to identify yourself to an online server, using an encrypted message. It's as if your computer has its own unique password to another service. GitHub uses SSH keys to securely transfer information from GitHub.com to your computer.

#### Upstream

When talking about a branch or a fork, the primary branch on the original repository is often referred to as the "upstream", since that is the main place that other changes will come in from. The branch/fork you are working on is then called the "downstream".

#### Blame

The "blame" feature in Git describes the last modification to each line of a file, which generally displays the revision, author and time. This is helpful, for example, in tracking down when a feature was added, or which commit led to a particular bug.



