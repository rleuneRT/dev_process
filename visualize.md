## Visualize

- use https://waffle.io/ to visualize this agile methodology 
- this gives you a Kanban method on top of all your stories/bugs/fr's/tickets/...

### How to use Waffle
Waffle present the issues and pull requests from one or more Github repository.
We use 5 columns to categorize our works.  

![waffle columns](2016-04-12_1271x343_scrot.png)

- Waffle can visualize stories, tasks, bugs/feature requests.
- Waffle's are attached to milestone projects !
- The same waffle kanban can visualize all mentioned categories above, use filters to select
- Waffle also allows a user to see which tasks/stories are assigned to him over multiple repo's
- For each waffle linked to milestone we also link all relevant code repositories so we can use the same waffle to see progress on FR's & BUGS.

#### STORIES

- **NEW**: Stories selected for milestone but no work started yet.
- **PROGRESS**: Stories which are being worked on.
- **QUESTION**: Stories which need feedback and need to be discussed
- **VALIDATION**: When a story is done, the next step is to review it. This is a vey important step in our process.
- **CLOSED**: After review when the solution proposed is accepted, the story is closed.


#### TASKS

- **NEW**: Tasks not started yet.
- **PROGRESS**: When someone is working on a task, the task is known as in progress. By looking at that column we can track on what the team is focusing on at the moment.
- **QUESTION**: Task is unclear it needs attention
- **VALIDATION**: optional, sometimes a task needs to be validated
- **CLOSED**: Done

#### Bugs & Feature Requests

- **NEW**: Unsorted bugs/fr
- **PROGRESS**: Active people are working on it
- **QUESTION**: Need feedback
- **VALIDATION**: Being tested
- **CLOSED**: Done


### Workflow

- @todo need some work here to rewrite this around a story. SO NOT OK YET. Its now around a task, this is not right I believe.
- @todo is double info with other section in the gitbook, around process, we should try to merge content

SO CONTENT BELOW NOT READY FOR PRIMETIME YET

Let's follow the journey of a new task from it's creation till it get closed.  
1. Someone create a new task. It can be a bug or a feature request. At this point the task is shown in the *backlog* column from waffle.

2. Someone is assigned to the task or choose to work on the task.  
First thing that person needs to do is make sure the task is understood enough. Are the specs clear? Is there enough detail about the task?  
If any question, post a comment and set the label **state_question**, so the person responsible knows he need to provide more information about the task.  
Waffle allow filtering on labels. It's **good practice to check once a day the tasks with the label state_question**, see if you anyone needs your input.

3. When the task is understood enough, it can be moved into the Accepted-ready column. Make sure the task is assigned to you so we know who is working on what.

4. Create a new branch for you task, give it a meaning full name.  
You can push your work daily to that branch even if the code is not ready yet. (This prevent data loss if you did something wrong while playing with the last version on btrfs on your development machine and your filesystem get screwed up, for example.)  
Pushing regularly allow other people to have a look at your work and make comment if the feel like doing so.  
Notice that when a branch referencing an issue is created, it will move the issue in the **In progress** column

5. The code is now ready, the next step is to ask to merge the code back into the master branch. To do so, create a pull request on gihtub, reference the issue this PR solved in the comment. Move the issue from in progress to **Completed** so people knows this task is ready to be reviewed.

6. When the PR is reviewed and the solution accepted, the PR is merge into master, the branch deleted and the issue close. The issue and the PR land in the **Closed** column of waffle and the journey is over.
