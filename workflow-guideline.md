## Working with Git

By definition commits should address small, meaningful and complete pieces of the feature that is currently under development. The list of commits attached to the Pull Request should be a step-by-step guide on the approach that was taken to solve a problem.

Remember to include the general change log in the Pull Request description. It will serve as an explanation to the reviewers why those changes were needed.

As for the branching conventions - in most cases, the [git flow](https://nvie.com/posts/a-successful-git-branching-model/) approach works best. It's better to stick to it unless you have a good reason to not to.

### Things considered a good practice when working with Pull Requests:
- Stick to the naming convention that the team agreed on e.g. `feature/nut-123-style-appointment-screen/`. 
- Respect the template for opening new Pull Requests if one is provided. Otherwise it is the best time to [create one](https://help.github.com/en/articles/creating-a-pull-request-template-for-your-repository), you can find samples [here](https://github.com/HealthTechDevelopers/playbook/blob/master/pr_templates/) and adjust it to your needs.
- Make sure that your Pull Request is in fact ready and could be merged to master branch as is. Don’t force others to waste their time on finding typos or silly mistakes
- It is acceptable to use ‚work in progress’ Pull Requests to satisfy different needs during development process. In that case attach the `WIP` signature to the title or use GitHub's **Draft Pull Request** feature and do not ask for review until the Pull Request is good to go
- Feel free to friendly remind your teammates of a pending Code Review
- The final output is a shared responsibility of all of the team members. Make sure the code quality is sufficient, the feature is complete, working and fully tested
- Log history of the repo should be similar to a pleasant trip down the memory lane so treat it with respect and keep it clean. The way it is written say all about your professional attitude
- Clean after yourself - when the Pull Request is merged to master branch it is about time to delete the feature branch
- Keep the board up to date with your current status of work - this will help the team in recognizing the progress 

## Code Review

- Don’t get too attached to your code and don’t take the suggestions personal. It is all done in the name of constant improvement and sharing knowledge.
- Feel free to ask if anything is not clear for you. As in life, asking questions and constant challenging is the crucial part of making things better.
- Remember that both author and the reviewer are equal. Approach the review with empathy and understanding of the person trying to give their best. Everybody was a junior once.
- Don’t hesitate with submitting a review, it can block other things from moving forward, especially when couple of rounds are needed.
- Before asking for a review make sure that all the code checks and Continuous Integration status pass
- Note that when opening a Pull Request you commit to the fact that it is ready for review. That means everyone in the team can jump in and review it. If otherwise please use `WIP` signature in the title. If you care about a particular person reviewing it assign them to the ticket.
- Use the review summary as a place for general feedback. Mark your review with appropriate status of approved or rejected depending on your thoughts about the implementation.
- Approving Pull Request is a necessary step before merging it to master branch. For small teams (2-3 people) at least one approval is required, for larger teams set a bigger number of required approvals.

## General Workflow

- Refer to Continuous Integration tool status for the information about the current merging or deploy possibility. Similar to crossing the street - you would always want to have a green light before moving on
- Don’t skip any of the steps needed to fulfill the process that the team is following. Even if on the tight deadline code review or testing is an essential factor in delivering working solution to a problem
- There won’t ever be a better time to write tests for the feature than at the time you are working on the implementation
- Try to rely on single focus principle. If you find any additional problems during implementation always try to address them in a separate Pull Request. The first step in that case should be to ask the Product Owner for triage. Opening a new ticket with detailed description and context / steps to reproduce will be an extra help.
- Respect work in progress limits which is most often one item per person. If you are blocked by waiting for code review or other dependencies feel free to think about refactoring and optimization of the current codebase
- Try to manage your tasks in terms of a single work day. Calling a day with all the work in Code Review is a good start of the evening.

## The Daily Show

Daily Standup meetig should help the Development Team monitor progress towards the Sprint Goal. With all the tools available it really breaks down to have the following questions answered:
- do I know what is the progress of the team towards our current goal?
- do I know what shall I do next?
- do I have all of my impediments or blockers sorted out or being taken care of?

**As you may be familiar with the typical three questions beigng answered by each team member it is not the only way to fullfill the above needs. In fact it is recommended by the Scrum Guide only if there is no other idea to handle that meeting. You can find another way below.**

Each day different team member moderates the meeting. Sample steps to use:
- Take a minute before the meeting to synchronize Pull Requests on GitHub with Jira board (if applies) 
- Opening
  - how many days are left till the end of the Sprint?
  - what is the goal of this Sprint?
- Go through the board
  - go from top right to bottom left column
  - mind the days in column
  - leave space for people to comment/ask about each item
  - reflect on column limits
  - if some items need pairing or more discussion schedule a meeting after the Daily
  - sum up with any urgent action needed to move items forward
- Verify top items from To Do column
  - are the items to be worked on today/next clear and ready?
- Reflect on the team’s projection
  - are we still able to deliver what we have promised?
  - if anything can be bumped to the next Sprint do it
  - if you want to be fancy show burndown chart and comment on it
- Ask for final thoughts, comments
- Assign a person to host the meeting tomorrow
