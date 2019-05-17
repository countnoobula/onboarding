# Guidelines for Pull Requests

This readme aims to give a decent guideline for authors and reviewers of pull requests.

The aim of this document is not to implement PR standards or Commit guidelines, it's purpose is to serve as a standard for how we should *approach*
reviewing and authoring code inside the company.

If at any time a team member is not following these guidelines- feel free to point them to this document.

Even though this document cannot be systematically enforced (there's a reason for that) - it's principles should be upheld throughout
the team.

For a TL;DR - scroll to the bottom of the document

## As an Author

### In Large PRs...
Large PRs are never easy or fun to write but they are also hell to review.

When you are creating a large PR, keep your commit messages clear and use the description to help give context
to what is happening in the commit.

1. Try to not group commits by file

eg: "Added Feature.php model"

Instead, try to group commits by concerns

eg: "Implemented the API for Feature A"
"
Implemented Feature A those does so and so. The migration creates a table for this-and-that.

This commit includes the tests and covers all standard processes, however, they don't cover this and that 

edge cases, this will be done at a later stage - refer to issue #42
"

2. If possible, do a pre-review of your own PR and if you find yourself getting lost or spot something that might

be confusing to other - you can add a comment and future reviewers can use your comment to ~understand wtf is going on~ gain some insight

from the author himself!

### Complete the PR templates

The PR template is there to help give context to reviewers, all sections serve to give a nice window into what this PR aims to achieve and where it achieves it.

This is a way for Reviewers to gain some context to the PR and to understand what steps have been taken and what state the PR is in.

The more information you can give in the pr template - the easier it will be for reviewers to jump in and understand how much time and effort they'll be putting into
the review.


## As a Reviewer

### Be Explicit
When requesting a change, instead of a vague one-liner comment, try to be more explicit about your opinion on the change
and why you feel it is necessary, or if you spot a bad pattern- perhaps you can explore why it might be harmful to the codebase
to implement it.

Much like our code can't be too bound in context (hence comments, commits, documentation, and PRs) - neither should our review comments.


### Acknowledge the cool stuff!
"Code review does not mean “point out only the problems.” `@TejasKumar_`
We all _hopefully_ enjoying coding- so be sure to acknowledge someone when they've implemented something cool
or do a solid job.

This is especially true for tests! Testing isn't a lot of fun but the whole team reaps the benefits from it. Give a
thumbs up

### Questions over statements
Instead of commenting "This is wrong, do it this way"
Rather ask "why have you done it this way instead of this way"?

If someone has gone against the standard in a project there's a fairly decent chance there was a reason in doing so.

This can be a great opportunity to find flaws in our standards, or hey, maybe they just forgot.

Obviously, there are instances where a statement is required...

eg - introducing a world-ending security flaw, or include a `debugger` or `dd` call in a file

..if you encounter one of these cases - don't be an asshole.



# The Golden Rule - Empathy

We all have bad days, we all have chosen lazy paths, and we've all made mistakes.

Both as a reviewer and an author try to have empathy towards the other party. We're all part of the same team, and merging a PR is a team effort.

So - in conclusion:

When you create a PR - be considerate of the time and effort of the reviewer.

When you review a PR - be considerate of the time and effort of the author.

