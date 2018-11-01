---
title: Merge vs. Rebase
description: Should I use merge or rebase to synchronize my pull request with master?
categories:
- contributors
---

<center>**If you know how to merge, but not how to rebase without accidentally losing
work,<br/>then stick with merge.**</center>

Maintainers aren't in a position to help correct a rebase gone wrong, so when
in doubt, stick with the git commands that you know. 🤓

If you are comfortable using `git rebase` to tidy up your commit history,
here are a few tips:

* Before you have submitted your PR, or it is still marked as a Work in Progress (WIP),
  feel free to use rebase as much as you like.
* After someone has begun reviewing your code, or when you are making requested changes
  from a review, put your changes in a new commit. This helps the
  reviewer by isolating your recent changes and makes it easier for them to
  verify that you have followed through on their suggestions.
* When you rebase or amend your commits after the review has begun, the reviewer
  has to redo the entire review from scratch, which for non-trivial pull requests
  can require a lot more time!
* When a reviewer asks you to rebase or update an out-of-date pull request with
  the latest changes from master, you can use either merge or rebase, whichever
  you are more comfortable with.
* A reviewer may ask you to squash or tidy up your commits once the review is complete.
  If you run into trouble, it's okay to ask that they squash your commits when they
  merge your pull request.
