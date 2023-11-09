# Bark Buddies
Code 201 final project

## TEAM NARK Team Members

- Niles Thompson
- Armando Bugarin
- Rhett Chase
- Kaitlin Davis

## Cooperation Plan

### Strengths and Areas for Improvement

- Niles
  - Strengths: technically savvy, great at technical research and implementing new ideas
  - Areas for improvement: can get hyper focused on an issue and get tunnel vision
- Armando
  - Strengths: project management, having a good attitude, perseverance
  - Areas for improvement: JavaScript
- Rhett
  - Strengths: JavaScript, analytical, problem solving, teaming
  - Areas for improvement: stubbornness when debugging can be unproductive
- Kaitlin
  - Strengths: persistent, learning new things, analytical
  - Areas for improvement: technically inefficient, time management

### Project Execution

- When it comes to researching topics the entire team is unfamiliar with, Niles' technical background will be important when it comes to familiarizing the team and implementing the features
- Armando's project management skills will be important to keeping the team on track with our workplan and hitting our timeline. His good attitude will keep us motivated!
- Rhett's JavaScript and problem solving skills will come in handy when figuring out how to implement different app features and help unblock the team when we get stuck
- Using Kaitlin's analytical skills can come in handy when running into issues and bugs that are be persistent

### Professional Competencies

- Niles: Improve CSS
- Armando: Improve Javascript skills
- Rhett: Improve technical skills in JavaScript and CSS; debugging
- Kaitlin: Improve technical skills in JavaScript and CSS

### Work Approach

- Utilize project management tool to maximize work time and schedules and track progress towards priorities
- Set clear roles and responsibilities so every team member understands how their contributions align with the overall goal
- Use communication/collaboration tools to stay up-to-date on progress (e.g., Slack, Remo)
- Work in pairs when possible to learn from each other's strengths

## Conflict Plan

### Resolving Conflict

- Listening to all team members' point of views and weigh the pros and cons
- Use democratic system and vote on it
- `Time out card` can be used to pause for clarification and/or take few minutes and then come back to discuss
- If someone is taking over the project, team members should feel comfortable to speak up and raise it as a concern
- Respect boundaries (e.g., don't change other people's code without permission)

### Approach Challenges

- Be patient and work together
- Constantly communicate
- Exercise the `15 minute rule`
- Take the time to explain the context and big picture before diving in to granular details

### Raising Concerns

- Speak to team member 1-on-1 if you feel they are not adequately contributing to fully understand what's going on
- Offer to help them

### Escalation

- When multiple attempts at resolution are unsuccessful and team members can't get on the same page
- Escalate to JB

## Communication Plan

### Hours Available

- Niles: 9 am - Midnight PT, weekends
- Armando: 9 am - Midnight PT
- Rhett: 9 am - Midnight PT
- Kaitlin: 9 am - Midnight PT

After hours communication protocol: Slack the group, if no response, update the PM software with a note on the task

### Platforms

- Slack, Remo, Monday (project management)

### Breaks

- As needed (aim for once per hour / 1.5 hrs)

### Time Management

- Leverage project management software to prioritize features that are critical
- Reassign tasks to those who have bandwidth
- Group/pair up on big features as needed or divide and conquer on smaller ones

### Creating a safe environment

- Ensuring everyone's voice is heard: Refer to `resolving conflict` section above
- Practice active listening and let everyone finish their thought/idea
- Feel free to speak up **respectfully** if you disagree

## Work Plan

- Develop milestones as a team in the Monday PM tool
- For each milestone/feature, build out the tasks and assign them to individuals or groups (after consensus reached)
- Each feature has its separate tasks and key outcomes, ownership and priority
- Change management requests are handled as a group
- PM Tool: Monday

## Git Process

### GitHub

#### Repo

- Main branch and all feature branches will live on GitHub
- Create GitHub org and share repo with teammates by entering teammates' github user names

#### Git Flow

**Follow best practices**
Source: chatGPT
Git flow is a branching model that defines a strict branching strategy designed around the project release. It helps in managing and organizing code development in a collaborative environment. Here's a simplified version of the Git flow that you can adapt for a GitHub organization:

- Master Branch: The master branch should always contain production-ready code. Consider this the stable branch. `git checkout master`
- Develop Branch: The develop branch is where active development occurs. It's a branch from which feature branches are created. `git checkout -b develop`
- Feature Branches: Each new feature or bugfix should be developed in a feature branch branching off from develop. `git checkout -b feature/new-feature develop`
- Once the feature is complete, it's merged back into develop.`git checkout develop git merge --no-ff feature/new-feature git branch -d feature/new-feature`
- Release Branches (optional):
- If you follow a versioning system, you might create release branches to prepare for a new version. `git checkout -b release/1.0.0 develop`
- Any necessary last-minute bugfixes can be done in this branch and merged back into both develop and master.

```zsh
git checkout master git merge --no-ff release/1.0.0 
git checkout develop git merge --no-ff release/1.0.0 
git branch -d release/1.0.0
```

- Hotfix Branches (optional): If a critical bug is discovered in production, a hotfix branch can be created.
`git checkout -b hotfix/1.0.1 master`
- Once the hotfix is complete, it's merged back into both master and develop.

```zsh
git checkout master git merge --no-ff hotfix/1.0.1 
git checkout develop git merge --no-ff hotfix/1.0.1 
git branch -d hotfix/1.0.1
```

- Pull Requests: For each feature, hotfix, or release, create a pull request on GitHub. This allows for code review and discussion before merging.
- Collaboration and Communication: Communication is crucial. Team members should be aware of ongoing work and branches. Use project management tools integrated with GitHub if needed.
- Continuous Integration (Optional): Implement continuous integration to automatically test changes on feature branches and ensure that the develop and master branches are always in a deployable state.

### Pull Request review workflow

- Yes, we plan to use a PR review workflow
- At least 2 additional team members review to confirm code functionality before pull
- The person who wrote the code will complete the merge (after it's reviewed/verified)
- Merge frequency with main branch: After successful testing and verification
- Communicate it's time to merge via slack (wait for confirmation from the entire team)
