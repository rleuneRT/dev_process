## Visualize

- use https://waffle.io/ to visualize this agile methodology 
- this gives you a Kanban method on top of all your stories/bugs/fr's/tickets/...

### How to use Waffle
Waffle present the issues and pull requests from one or more Github repository.
We use 5 columns to categorize our works.  

![waffle columns](2016-04-12_1271x343_scrot.png)

- **Backlog**: It's in this column that newly created issues or issues that don't have a type lives.
- **Accepted-Ready**: In this column we find the issue that are ready to be work on. No code should have been written for an issue before it reach this column.
- **In progress**: When someone is working on a task, the task is known as in progress. By looking at that column we can track on what the team is focusing on at the moment.
- **Completed**: When a task is done, the next step is to review it. At least one person need to review the solution proposed for the task.
- **Closed**: After review when the solution proposed is accepted, the task is closed.

### Workflow
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