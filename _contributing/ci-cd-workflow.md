---
exclude: true
layout: wiki
title: CI/CD Workflow
position: 3
---
# Git Workflow: CI/CD

This project uses a github-flow based git workflow, described below.

## Branches:
### main or production
Code in the main or production branch is automatically deployed to the production environment. Code merged in this branch should be stable, and it must go through the full code review process described below. Code deployed to production should always be deployed to staging first.

### staging
In the staging branch, code is tested and verified before bing moved to production. All code (except for hotfixes) should go through staging.

The staging branch should be the destination for pull requests from feature or bugfix branches.

### feature/
Feature branches should be branched from the Production branch. They are where
active development of new features or improvements to existing features should take place.

Feature branches should start with `feature/`, and be followed by the GitHub issue
number and a brief description of the feature to be added. 

Example: `feature/#32_rate_limiting`

### bugfix/
Bugfix branches should be branched from production. They are where bug fixes should be developed.

Bugfix branches should start with `bugfix/`, followed by the GitHub issue number and a brief
description of the bug. Example: `bugfix/#33_rate_limit_crashes_client`

### hotfix/
Hotfix branches are where especially urgent fixes should be developed, since hotfix branches
are the only way to merge code directly into production without testing it in staging first.

Hotfix branches start with `hotfix/`, followed by the GitHub issue number, and
a brief description of the issue being fixed. 

Example: `hotfix/#34_remote_code_execution`

## Commit Messages
Commit messages are very important. They tell other developers what you did without
them having to read all the changes you made. Commit messages should be in the form:

`#<GitHub issue number>: <Description of what you did>`

Example: `#15: Added endpoints for adding/removing users`


## Merging
All merges into staging should happen via a pull request from a feature or bugfix 
branch. Once the code has been tested in staging, it can be merged into production via a 
pull request from staging. 

The [Code Submission Process](/contributing/index#:~:text=How%20To%20Contribute%20Code) 
outlines the requirements that pull requests must meet and the process they will go 
through.