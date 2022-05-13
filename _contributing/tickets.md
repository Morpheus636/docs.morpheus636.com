---
exclude: true
layout: wiki
title: Tickets
position: 1
---
# Tickets
Morpheus636 projects use GitHub Issues for managing tasks.

## Submitting Tickets
Submitting tickets is an easy way to contribute to the project, with no programming skills required.
When submitting a ticket, please make sure to include as much information as you can,
so a contributor can best work off of it.

Before submitting a ticket, please search through existing tickets to make sure that you're not
submitting a duplicate. Duplicate tickets will be closed.

### Bug Reports and Feature Requests
If you discover a bug in the project, or you would like to have a feature added to it,
please submit a bug report or a feature request.

To submit a bug report or feature request, go to the "Issues" tab in the repository,
and click "New Issue". Then, select the Bug Report template or the Feature Request template.

Make sure you include as much of the requested information as you have, since it makes it much
easier for contributors to investigate.

## Working a Ticket
Core Contributors and Maintainers should "work" each ticket submitted, by applying the
proper labels, gathering information, answering questions, implementing new
features, and eventually, closing the ticket.

### Labels
It is important that each new ticket has the correct labels applied to it. This makes it easier
for contributors to quickly search through for related tickets, or find issues to work on.

Morpheus636 projects all have the following labels:
- `documentation` 
    - description: Improvements or additions to documentation
    - color: `#0075ca`
- `enhancement`
    - description: New feature or feature request
    - color: `#a2eeef`
- `bug`
    - description: A report that something isn't working
    - color: `#d73a4a`
- `duplicate` 
    - description: This issue or pull request already exists
    - color: `#cfd3d7`
- `invalid` 
    - description: This issue contains generally invalid or incorrect info
    - color: `#e4e669`
- `dependencies`
    - description: Issue is about dependencies
    - color: `#1d76db`
- `ci checks` 
    - description: Changes to the project's CI workflows and checks
    - color: `#fbca04`
- `p:<Platform>` 
    - description: A `p:` label exists for each platform that the project supports. Any tickets that apply 
      only to one platform should be tagged with the corresponding label.
    - color: `#c5def5`
- `triaged`
    - description: Issue is ready to be worked on by a core contributor
    - color: `#b3f660`
    - **Only a Maintainer should apply the `triaged` label to a ticket.**
- `help wanted`
    - description: Extra attention is needed
    - color: `#008672`
    - **Only a Maintainer should apply the `help wanted` label to a ticket.**
- `good first issue`
    - description: Good for newcomers
    - color: `#7057ff`
    - A `good first issue` ticket is detailed and easy to implement, and should have a detailed
      explanation of what needs to be done, so that a new contributor can easily pick it up.
    - **Only a Maintainer should apply the `good first issue` label to a ticket.**
- `wontfix`
    - description: This will not be worked on
    - color: `#ffffff`
    - **Only a Maintainer should apply the `wontfix` label to a ticket.**


## Assigning and Picking Up Tickets
### Core Contributors:
Once a ticket is marked as `triaged`, if you'd like to pick up the ticket to work on implementing it,
you can assign yourself to the ticket. Do this by clicking the 'assignees' button at the top right,
and selecting yourself.

Make sure that nobody has already assigned themselves before assigning yourself or beginning work,
so that you don't waste your time with a duplicate pull request.

### Other Contributors:
If a ticket is marked as `help wanted` or `good first issue`, and you'd like to pick up the ticket to
work on implementing it, post a comment in the ticket saying that you'll be working on it. When a
Core Contributor or Maintainer sees it, they will mark it as assigned to you.

Make sure that nobody has asked to be assigned or already been assigned before you begin working,
to prevent multiple people opening a pull request over the same thing.

## Closing Tickets
The criteria for ticket closure is as follows:
1. The ticket is a duplicate, has been labeled as `duplicate`, and the original has been linked.
2. The bugfix, feature, or documentation improvement requested will not be implemented, and the
  ticket has been labeled as `wontfix` by a Maintainer.
3. The bugfix, feature, or documentation improvement requested has been implemented, and a
  pull request has been accepted and merged.