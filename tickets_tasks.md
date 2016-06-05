## Tickets & Tasks & Bugs & Feature Requests


### What is what

- Ticket
    - an issue raised by a customer or internal employee
    - escalates an issue like downtime, performance issue, question, ...
    - Tickets are put on project repo's or support repo.
 
- Bug
    - issue of product
    - only raised by support person or developer (gig or external if opensource)
    - If customers see a bug they normally will create a ticket first and the support person will create a bug & follow up
    - is done on the code repository
    - If someone tumbles upon a blocking bug, the link to the issue needs to posted to the BAM telegram so that the whole organisation does not have to wait to the next BAM meeting for the assessment of the blokker.
    
- Feature Request  (FR)
    - raised by developers or anyone having interest in the code base (is done on the code repository), these feature requests are funneled & prioritized before they become story cards.

- Tasks
    - only used on ```org_repo's``` or ```proj_repo's```     !!!
    - the tasks are linked to the subject for which the task is (not the proj where people belong too)
        - e.g. if our legal council needs to help on a contract in ```proj_mauritius``` as example then the task is in ```proj_mauritius``` NOT in ```org_legal```

### Task format:

#### Title: ```$storyname:$taskDescription [4h]```

- time format is optional
- can be in h or days e.g. 4h or 4d 
- e.g.: ```storyx:cleanup the text for button something [1h]```
- e.g.: ```storyx:complete the autotest nr ... [1d]```

	
### Body:


```
## GOAL:

- Clearly describe the goal what needs to be achieved when the task is delivered.
- often optional !!! and defined at story card level

## DESCRIPTION

- describe what task is about

## REQUIREMENTS

- Add specifications, remarks, implementation hints, requirements
- this is often optional, and defined at story card level 

**ESTIMATION**: [```number of hours```(h)|```number of days```(d)] 

```

- goal is optional, often they are put at story card level
- requirements are optional, normally they are put at story card level
- estimation is optional
- a task is linked to 1 owner who is responsible for putting the hours right

example: [link](https://github.com/Incubaid/dev_process/issues/20)

 


