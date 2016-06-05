## bugs & feature requests funnel

IN: BUGS - FEATURES ->

![](http://www.rocketwatcher.com/wp-content/uploads/2011/01/Funnel-mod.jpg)

OUT: STORIES

### principles

- The idea is that in a code repo you log all the bugs & feature requests
- anyone can report bugs or feature requests
- the [productowner](roles.md) will sort through the issues & give them priorities (use labels)
- the bugs or FR's are grouped and planned to be executed (attached to milestones)
- there can be lots of milestones in a code repo, these milestones are used to link X nr of bugs/FR's to a story in the milestone repo, see milestone section to understand purpose.


### DO NOT

- plan work directly on FR's or BUGs, this result in very bad planning
  - there is a shortcut to create tasks automatically though, see below 

### WHY

- This forces product owners to think about organizing work & priorities

### how to automate task creation

- if you put $storycardname: at beginning of title of issue then this bug/fr will become a task underneath the story
- this only works if $storycardname is unique (which has to be for active stories)
- this is done by the incubaid development process tools

