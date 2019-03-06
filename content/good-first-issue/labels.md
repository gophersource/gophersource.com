---
title: 
description:
---
## Help Wanted

Items marked with the `help wanted` label need to ensure that they are:

- **Low Barrier to Entry**

  It should be tractable for new contributors. Documentation on how that type of
  change should be made should already exist.

- **Clear Task**

  The task is agreed upon and does not require further discussions in the
  community. Call out if that area of code is untested and requires new
  fixtures.

  API / CLI behavior is decided and included in the OP issue, for example: _"The
  new command syntax is `svcat unbind NAME [--orphan] [--timeout 5m]`"_, with
  expected validations called out.

- **Goldilocks priority**

  Not too high that a core contributor should do it, but not too low that it
  isn't useful enough for a core contributor to spend time to review it, answer
  questions, help get it into a release, etc.

- **Up-To-Date**

  Often these issues become obsolete and have already been done, are no longer
  desired, no longer make sense, have changed priority or difficulty , etc.

Related commands:

- `/help` : Adds the `help wanted` label to an issue.
- `/remove-help` : Removes the `help wanted` label from an issue. If the
  `good first issue` label is present, it is removed as well.

## Good First Issue

Items marked with the `good first issue` label are intended for _first-time
contributors_. It indicates that members will keep an eye out for these pull
requests and shepherd it through our processes.

**New contributors should not be left to find an approver, ping for reviews,
decipher prow commands, or identify that their build failed due to a flake.**
This makes new contributors feel welcome, valued, and assures them that they
will have an extra level of help with their first contribution.

After a contributor has successfully completed 1-2 `good first issue`'s, they
should be ready to move on to `help wanted` items, saving remaining `good first
issue`'s for other new contributors.

These items need to ensure that they follow the guidelines for `help wanted`
labels (above) in addition to meeting the following criteria:

- **No Barrier to Entry**

  The task is something that a new contributor can tackle without advanced
  setup, or domain knowledge.

- **Solution Explained**

  The recommended solution is clearly described in the issue.

- **Provides Context**

  If background knowledge is required, this should be explicitly mentioned and a
  list of suggested readings included.

- **Gives Examples**

  Link to examples of similar implementations so new contributors have a
  reference guide for their changes.

- **Identifies Relevant Code**

  The relevant code and tests to be changed should be linked in the issue.
