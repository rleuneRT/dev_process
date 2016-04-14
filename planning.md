## planning

This section describes who in general we plan our work.

### product related

#### step 0: prepare

- per company there is an organization (on github)
- there is a home repo in which we can document generic specs, docs, ...
- there is are X nr of milestone repo's
    -in the milestone repo's we document the stories which need to be delivered for a certain deadline
    - a milestone repo is the most imporant element for our planning, our full planning is based on milestones, they are typically not far out e.g. 2 weeks
    - in 1 milestone we deliver stories which are finished & fully tested
    - testplans are defined per milestone
    - tasks are used to define subwork of a story
- each product repo has a code repo
    - in the code repo we group feature requests & bugs per github milestone in the code repo
    - be not confused with the term milestone as used above which is a repo
    - here we use the github repo milestone to group a set of FR's or Bugs, this github milestone is then linked to a story which is defined in a milestone repo


#### step 1: roadmap / strategic planning

- in home repo
  - Readme.md  (```$homerepo/Readme.md```)
    - link to docs mentioned below 
  - create terminology doc  (```$homerepo/terminology.md```)
    - define all relevant terms to do with your products 
  - create components doc  (```$homerepo/components.md```)
    - define the components which make up the product
    - what do these components do
    - link to relevant code repo's
  - create roadmap doc  (```$homerepo/roadmap.md```)
    - define a planning & link to milestones (which are repo's)
    - each milestone repo is linked to X nr of stories

- setup milestone repo's
  - (```$milestone_$name```)
  - describe the goal & deadline of this milestone (Readme.md)
  - describe story card owners (optional)
  - each milestone is linked to telegram group: ```milestone_$shortcompanyname_$shortMilestoneName```, put link to this telegram group
  - choose a milestone owner
  - make sure its clear that a milestone is active or not !!!
 
- setup communication
  - create milestone groups on telegram
    - make sure right people have access to it   
    - all relevant stakeholders & story card owners
    - announce the right milestone repo's over the telegram
  

#### step 2: story card preparation

- is an ongoing process
- create all story cards relevant for 1 or more milestones
    - put the story cards in the right milestones !!! 
- choose the story card owners wisely

#### step 3: stakeholder meeting (see [meetings doc](meetings.md))

- call stakeholder meeting to discuss milestone(s)
  - use telegram group: ```milestone_$shortcompanyname_$name``` to announce
- when approved, announce over telegram
- when not approved do more of these meetings, go back to step 2 when required

#### step 4: milestone meeting (see [meetings doc](meetings.md))

- present milestone & related story cards to everyone involved in the organization
- this is the official start of getting this milestone done

#### step 5: story group meetings (see [meetings doc](meetings.md))

- the story owners organize meetings to discuss progress
- happens every day, needs to be very short < 15 min
- use telegram group: ```milestone_$shortcompanyname_$name``` to coordinate
- use ```story_$shortcompanyname_$shortStoryName``` to communicate specifically about 1 story when this becomes relevant (is optional)

#### step 6: demo meeting (see [meetings doc](meetings.md))

- give demo's about what has been accomplished
- use telegram group: ```milestone_$shortcompanyname_$name```

#### step 7: milestone acceptance meeting (see [meetings doc](meetings.md))

- discuss how the milestone went, learn for future
- use telegram group: ```milestone_$shortcompanyname_$name```








