## usage of telegram

- telegram (and later rogerthat) is our main tool to let communication flow.
- in this doc we describe the main telegram groups & how we use them
- IMPORTANT: PEOPLE NEED TO USE 2FACTOR AUTHENTICATION !!!!

### milestone 

- ```milestone_$shortcompanyname_$name``` e.g. ```milestone_gig_ovc210```
- defines a milestone for the company an all main communication to do with this
- used for
    - announcing meetings e.g. stakeholder meeting, story meeting if change in time, ...
    - important events
    - inform about important information changes (e.g. stories, specs, roadmap, ...)
    - planning events e.g. story meeting is now different time per day
    - important bugs people should be aware about
- who is on it
    - everyone who has something to win or loose with this milestone internal to our company 


### support

- ```support_$shortcompanyname``` e.g. ```support_gig```
- used for
    - any customer isue which deserves attention from more than 1 person
    - for escalations
    - for information sharing
    - for planning events
- who is on it
    - everyone delivering support
    - everyone who wants to know what is going on
- IMPORTANT
    - on duty support guys
        - NEED to announce their duty ON & OFF event on this group (if less than 10 people active, for larger orgs this will not be practical). This will allow people to see how is online & active.
        - NEED to use & actively look at this group

### project

- `support_$shortcompanyname_$projname`
    - e.g. `project_gig_internalit`
    - e.g. `project_gig_mauritius`
    - e.g. `project_gig_funding`
    - often the name used is the same as the name of the git repo
- used for
    - communication around such a project
    - planning, info changes, ...
- who is on it
    - everyone which is working on this project 

### cockpit

- ```cockpit_$shortcompanyname_$name```
- in line with name of cockpit git repo
- used for
    - all communication around 1 IT environment (can be for 1 customer or internal, ...)
- is also used by cockpit: ays robot
    - means we can see on this group if there are issues with the environment
    - or we can give instructions to the ays robot to do something
- e.g. is done per test environment
    - can see if someone is doing a test and what the result is
    - can see monitoring state
    - can request changes
- who can use it
    - people with right security clearance !!! can be partners & internal


