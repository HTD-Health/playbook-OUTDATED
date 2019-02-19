## Workflow
- Commit often and use descriptive commit messages. List of your commits should be like a readable changelog for people doing a code review.
- Pull requests should be as small as possible and focused aroung one functionality 
   - When you work on some new feature and you find a bug which is not directly related to your task, add a card to the backlog. If the bug is a serious one decide within the team who shold take care of it. Patch should be done on separate branch.
- Each developer is responsible for their PR for the whole time, so:
   - Branch name should follow the convetion: feature/nut-123-something-descriptive
   - Obey the PR template (specific for each project)
   - Test and code cleanup before asking other developners for review. PR can be created earlier to present solution to other teammates, but in such case it should have a label "Work In Progress" just to be explicit that it shouldn't be merged yet. GitHub PR is also a good place to look at a diff of your own code and doing self-review.
   - Remind about PR if review isn't done for a long time
   - Quality in the project is a responsibility of all team. Everyone should care about doing code review, tests and delivering a complete feature.
   - Make sure that your commit history is clean
   - Remove feature branches after merging
   - Update the board in task management tool after completing a task




## Code review 
- First of all do not get too attached to your code :) Code review is for delivering better quality in the project and mutual learning and opionions exchange between developers. Suggestions to code are not a personal attack, so do not get mad if your PR was rejected.
- Do not afraid to ask questions! If you don't understand some part of the code ask the author for explanation. Code should be first and foremost readeable and understandable. Maybe you would be able to figure out more clean solution that way?
- As a person who is doing a review try to suggest changes and start a discussion. Do not point out mistakes in offensive way and do not criticize others - everone could have a bad day :)
- Code review should not be blocking for other's work, try to do it as soon as possible for you.
- Before asking for review make sure that CI has passed without any errors.
- Every open PR means it's ready for review unless it is labelled as "Work In Progress". Review should be done by every team member. If you need a review of specific person, assign it as a reviewer in GitHub.
- If you are doing a review, to not leave empty comments. If you want to give feedback, mark PR as rejected if it requires changes before merging or approved if everything is OK or suggestions are not so important.
- To merge PR to a main branch there should be at least 1 approval in 2-3 people teams or 2 approvals in 4+ people teams.




## Work discipline
- CI on main branch should be keep green all time, we don't merge or deploy branches which has failing builds
- Code reviews and tests are the requirement to maintain quality and integral part of work in the project. They shouldn't be skipped because of delays in feature delivery. We should consider untested code as a feature which is not working.
- Tests should be added on regular basis as an integral part of the task. There will be no good time to add tests "later" :)
- Work only on things from TODO, which You've planned during sprint planning or grooming. Try to keep focus only on current task you are working on. If you will encounter new bugs or refactor places - mark them by adding a backlog cards, You'll be able to do them in more appropriate time and do not forget them.
- TODO column should contain only the tasks with complete information to implement them, e.g. designs or API
- Work at two tasks at once at most and try to finish them as soon as possible. Do not start another tasks until you merge and update the board. If a code review is blocking you, remind reviewers about it. In the free time you can think about places in the code that can be refactored, added tests, update the docs or anything that would bring value to the team or product. 
- Try to finish the tasks the same day You've started them. Try to plan your work in such way, that at the end of the day your tasks are in "Code review" column.


