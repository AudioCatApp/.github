# :rocket: Contribution Protocol :rocket:

The foundation for smooth merges and stable main.


## Content
- [Branch Basics](#branch-basics)
- [Pull Requests](#pull-requests)
- [Review Process](#review-process)
  - [For Reviewee (Assignee)](#for-reviewee-assignee)
  - [For Reviewer](#for-reviewer)
- [Merging](#merging)


## Branch Basics
- Remember: **NEVER COMMIT DIRECTLY TO MAIN**. Create a new branch off the latest main, commit your changes, make a PR.
- Branch naming structure should contain your name and the purpose of the branch divided by slash. E.g. `victoria/platform-refactoring` or `benjamim/graphics`.
- Commit changes as often as you feel reasonable, but keep them logical and focused (no one-symbol fixes or 10GB dumps all at once).
- Try to avoid committing non-working code, even if you plan to fix it in the next commit.
- There are no strict rules about commit name/description, however the recommendation is to keep it short and understandable.

## Pull Requests
- Rebase feature branch on top of main and resolve all the conflicts (if exist), then force-push.
```
git checkout your-branch
git fetch origin
git rebase origin/main
git push --force
```
- Fill out PR description according to provided template.
- Assign yourself as the author (reviewee).
- Request review from [@HenryGerretGruning](https://github.com/HenryGerretGruning) or someone who knows the code.

## Review Process

### For Reviewee (Assignee)
- Address all comments from all reviewers before merging. 
- *Non necessarly, but highly appreciated:* mark comments as addressed by replying with `Done.` or simply reacting with an emoji (e.g. :+1:).
- If the change will not be made (or the comment was a question/suggestion), respond with a reasonable explanation.
- Do not resolve conversations yourself – the reviewer does that.
- Once all comments are addressed, re-request review from the relevant person.

### For Reviewer
- Leave clear and constructive feedback on all added/changed code.
- Only resolve conversations when the change is fully addressed or the response is satisfactory.
- Approve when the PR is ready to be merged, not in advance.

## Merging
- The reviewee (assignee) is responsible for merging. PR can be merged when:
  - All conversations are resolved.
  - Approvals from every reviewer who left comments is given and no unreviewed changes are made.
  - Branch is 0 commits behind main (if not - rebase).
  - All conflicts with main branch are resolved.
- Corresponding feature branch will be deleted automatically after successful merge.
