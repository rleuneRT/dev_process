
## Stories are the Start of All

Stories help us to organize our work, they need to comply to certain requirements to be effective though.
  
![](http://2.bp.blogspot.com/_H0iqHTCqRyo/R4zyNrT94KI/AAAAAAAAATo/VY8M-kc1MyU/s400/user+stories+-+agile+software+development+-+cards.jpg)

A story normally represents the view of a person, e.g. I as product owner for product X would like to see Y features to be implemented because ... e.g. customer Z needs this, or strategic, ...


### Properties of a good story

- Well chosen name
- Clear description of what we want to achieve
- Priority, is a label: Critical, Urgent, Normal or Minor
- Milestone (only 1, date when this story has to be delivered)
- Assignee: is the [story card owner](roles.md)
- Effort (in days)
   - Put as ```(effort:4)``` anywhere in body of story 
- Clear set of requirements or link to another document which has the requirements (in same repo)
- Clear set of acceptance tests or link to another document which has these acceptance tests (in same repo)
- Links (URLs) in same repo to
  - Spec
  - Product Requirements Document (PRF) if relevant
  - Features or bugs which are related to it (milestone as used on specific repo)
- Format:
	- Title: ```Story title``` (```Story name```)
	- The story name is used to referenced in [Tasks](./tickets_tasks.md) related to the story


### stories can constantly be re-prioritized

![](http://agilemodeling.com/images/requirementsManagement.gif)


### Story format:

#### Title: ```$storyDescription ($storyname)```

E.g.: ```fix user escalated UI issues (ui_issues)```

	
### Body:


```
## GOAL:

- Clearly describe the goal what needs to be achieved when the story is delivered.

## DESCRIPTION

- describe what story is about

## REQUIREMENTS

- Add specifications, remarks, implementation hints, requirements
- IMPORTANT

## REMARKS

- anything relevant

**ESTIMATION**: [```number of hours```(h)|```number of days```(d)] 
```

- Goal and requirements are a must
- Estimation is optional and ONLY SET BY THE STORY CARD OWNER 
	- It's an assessment from the story card owner to visualize how many hours/days left to finish this story, is aggregated mandays/hours for all people working on this
	- This number is the amount of work left till completion
- Each story is linked to one owner who is responsible for putting the remaining hours/days in, this needs do be done on very regular basis

Example: [see here](https://github.com/Incubaid/dev_process/issues/21)


### When does story card go into validation stage

- For stories related to project, customer,...
	- When work or subproject is done and needs to be validated 
- For story related to code: 
	- When code done
	- When autotests (if relevant) are created
	- When all documentation relevant to story is done
		- Do not forget to document how to test this story card
		- Do not forget how to install / build everything to do with this story card 
	- When all tests are done


### When is a story card complete (closed)

- When validation was done by story card owner and other stakeholders
- Result is everyone can based on story card allone install & test the code/work relevant to this story


### What are the duties of a story card owner

- Format of story is OK
- Content of story is properly done (descr, requirements, ...)
	- Requirements are clear!
	- Everyone relevant understands the story properly
- Communicate around your story to all stakeholders at least every other day
	- How far are we
	- What are the blockers
	- What is planned now
	- Do this by commenting on story card
- Escalate to stakeholders when
	- Story has delay
	- There are questions
	- Do this by comments and also use relevant (e.g. Telegram) group to escalate in appropriate people
- In case of code:
	- Code is complete 
		- Features are in line with requirements
	- Tests are good enough
	- Good documentation that CAN BE UNDERSTOOD BY SOMEONE WHO DID NOT WORK ON THE STORY
	- On validation phase the pull request is properly merged in (after validation of course)
	- Code can easily be build and installed by anyone
	- Everyone relevant understands story is done and declare victory!


### Use of Incubaid GitHub development tools

- Our tools will automatically find the tasks and embed them in the story so it's very easy for people to follow what the linked tasks are and how far we are from completion