---
title: Contributing Index
layout: wiki
position: 0
---
# Contributing
This contribution guide applies to all of my open-source projects. It not only outlines my
my expectations for contributors, but should also serve as an "intro to open-source" for beginners.
If you are experienced, you can simply skip over the basic sections.

## Jobs within my projects:
### Maintainer
In most of my projects, I am the sole maintainer. The maintainer(s) decide the direction of the
project, including what feature requests will be accepted or rejected, when (or if) bugs are fixed,
when releases come out, etc. Any code that is deployed or released goes through the maintainer(s).

I spend as much time as I can on my projects, but I don't get paid to do so, and I'm still a 
full-time student. Please be patient. If you don't get a response to a ticket within a week, please
tag @Morpheus636 on GitHub so I get notified again.

### Core Contributor
Core Contributors are trusted contributors with direct commit access to the project's main repo.
While their changes must still go through the Maintainer(s), Core Contributors are trusted to make 
larger architectural decisions than the general public. Core Contributors also help the
Maintainer(s) respond to [tickets](/contributing/tickets) and support requests, freeing them up to 
make decisions instead of sorting through tickets.

### Contributor
Anyone else who helps the project, whether through submitting a ticket, reviewing pull requests, or 
opening a pull request with changes, is considered a contributor.

## How To Contribute Code
If you'd like to contribute code, this is the 
process you should follow:
1. Pick up a ticket.
  - The process for this is explained on the [Tickets](/contributing/tickets) page, but I'll make it
  simple - if you're new, look for a ticket labeled `good first issue`, and ask to be assigned
  to it. Once a Core Contributor or Maintainer assigns you, continue with the rest of these steps.
2. Create a fork of the repo.
  - Hit the `Fork` button at the top right of the project's GitHub repo.
3. Setup your development environment
  - Instructions for configuring your development environment should be linked in the project's
  README.
4. Make your changes in your fork.
  - Make sure you're following the correct Git Workflow for the project (it should say in the 
  project's README what workflow it uses, but it's either my
  [Semantic Versioning Workflow](/contributing/semantic-version-workflow) or my 
  [CI/CD Workflow](/contributing/cicd-workflow)), including following commit comment guidelines, 
  code style guidlines (linked in the README) and other best practices.
5. Create a Pull Request to merge your changes back into the main repo.
  - Once again, you should follow the correct Git Workflow when doing this and set the destination 
  branch accordingly. Please also make sure there are no merge conflicts before submitting (this 
  may require that you merge the upstream changes from the main repo into your fork before you open 
  the PR).
  - When you create a PR, it should give you a template. Please fill it out completely, including 
  noting your changes, linking the associated ticket(s), marking the type of change, and completing 
  the Copyright Assignment. Do not modify the template except as indicated.
7. Fix any issues.
  - If any of the automated checks fail, please fix the problem as soon as you can. If you need 
  help fixing it, say so in a comment and someone should be able to help.
8. Get code review.  
  - Wait for a Core Contributor or Maintainer to conduct a code review, in which they read 
  through all your changes, comment on anything they think needs improvement, and then either 
  accept or reject your PR. Note that rejecting a PR is not the same as closing it - it just means 
  that you need to make the changes noted in the comments of the review. Repeat this step until all 
  reviews are approved.
9. Wait for a merge.
  - Once all of this is done, wait for a maintainer to merge your pull request (or close it without 
  merging, described below). If you PR gets merged, make sure that the associated issues got closed 
  along with it.

### Closing Pull Requests
Just like Tickets, Pull Requests have a couple routes to closure:
1. The pull request gets merged into the project
2. The pull request gets closed without merging because:
  - The author of the PR did not fill out the form correctly (in which case the author can fix it 
  and re-open it)
  - Changes were requests in code review or by automated checks and they have not been addressed in 
  a timely manner
  - There's a problem with the associated Ticket, i.e no ticket was submitted, the ticket was not 
  marked as ready to be worked on (or was marked as `wontfix`), someone else is working on the 
  ticket, etc.
  - The changes were implimented poorly, and they are beyond fixing without starting over.
  - The PR is a duplicate

**Only a Maintainer should merge or close a Pull Request** The Maintainer that closes a PR should 
provide a comment as to why it was closed. If not, you may tag them and ask for a reason.
