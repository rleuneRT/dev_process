## stories are start of allStories help us to organize our work, they need to comply to certain requirements to be effective though.  ![](http://2.bp.blogspot.com/_H0iqHTCqRyo/R4zyNrT94KI/AAAAAAAAATo/VY8M-kc1MyU/s400/user+stories+-+agile+software+development+-+cards.jpg)### Properties of a good storyA story normally represents the view of a person,e.g. I as product owner for product X would like to see Y features to be implemented because ... e.g. customer Z needs this, or strategic, ...- well chosen name- clear description of what we want to achieve- priority ( is a label : critical, urgent, normal, minor)- milestone (only 1, when does this story have to be delivered)- assignee: is the [story card owner](roles.md)- effort (in days)   - put as ```(effort:4)``` anywhere in body of story - a clear set of requirements or link to another document which has the requirements (in same git)- a clear set of acceptance tests or link to another document which has these acceptance tests (in same git)- links to are put as link to right url in the git repo  - specs (in git)  - prd if relevant (in git)  - features or bugs which are related to it (milestone as used on specific repo)- format:	- Title: ```Story title``` (```Story name```)	- The story name is used to reference [Tasks](./tickets_tasks.md) to the story.### stories can constantly be re-prioritized![](http://agilemodeling.com/images/requirementsManagement.gif)

### story format:


#### Title: ```$storyDescription ($storyname)```

- e.g.: ```fix user escalated UI issues (ui_issues)```

	
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

- goal & requirements are a must
- estimation is optional and ONLY SET BY THE STORY CARD OWNER 
	- its an assessment from story card owner to visualize how many hours/days left to finish this story, is aggregated mandays/hours for all people working on this
	- this nr is amount of work left till completion
- a story is linked to 1 owner who is responsible for putting the remaining hours/days in, this needs do be done on very regular basis

example [see here](https://github.com/Incubaid/dev_process/issues/21)

### when does story card go into validation stage

- for story related to project/customer/...
	- when work/(sub)project is done & needs to be validated 
- for story related to code: 
	- when code done
	- when autotests (if relevant) are created
	- when all documentation relevant to story done
		- do not forget to document how to test this story card
		- do not forget how to install / build everything to do with this story card 
	- when all tests are done

### when is a story card complete (closed)

- when validation has done by story card owner and other stakeholders
- result is everyone can based on story card allone install & test the code/work relevant to this story

### what are the duties of a story card owner

- make sure format of story is ok
- make sure content of story is properly done (descr, requirements, ...)
	- make sure requirements are clear !!!
	- make sure everyone relevant understands the story properly
- make sure that you communicate around your story to all stakeholders at least every other day
	- how far are we ...
	- what are blockers ...
	- what is planned now ...
	- do this by commenting on story card
- make sure you escalate to stakeholders when
	- story has delay
	- there are questions
	- do this by comments & also use relevant e.g. telegram group to escalate in appropriate group
- if code:
	- make sure code is complete 
		- make sure the features are in line with requirements
	- make sure there are good enough tests
	- make sure there is good enough documentation AND IT CAN BE UNDERSTOOD BY SOMEONE WHO DID NOT WORK ON THE STORY
	- make sure that on validation phase the pull request is properly merged in (after validation ofcourse)
	- make sure the code can be easily build & installed by anyone
	- make sure everyone relevant understands story is done & declare victory !

### use of incubaid github development tools

- our tools will automatically find the tasks & embed them in the story so its very easy for people to follow which the linked tasks are & their completion


