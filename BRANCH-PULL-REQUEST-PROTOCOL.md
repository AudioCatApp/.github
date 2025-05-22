# :hammer: Branch & Pull Request Protocol :wrench:

The launch sequence for smooth merges.


## Content
- [Branch Basics](#branch-basics)
- [Pull Requests](#pull-requests)
- [Review Process](#review-process)
  - [Reviewee (Assignee)](#reviewee-assignee)
  - [Reviewer](#reviewer)
- [Merging](#merging)


## Branch Basics
- Remember: **NEVER COMMIT DIRECTLY TO MAIN**. Create a new branch off the latest main, commit your changes, make a PR.
- Branch naming structure should contain your name and the purpose of the branch divided by slash. E.g. `victoria/platform-refactoring` or `benjamim/graphics`.
- Commit changes as often as you feel resonable, but keep commits logical and focused (no one-symbol fixes or 10GB of data all at once).
- Try to avoid commiting non-working code even if you plan to fix it with the next commit.
- There are no strict rules about commit name/description, however the recomendation is to keep it short and understandable.

## Pull Requests
- Rebase your feature branch on top of main and resolve all the conflicts (if exist), then force-push.
```
git checkout your-branch
git fetch origin
git rebase origin/main
git push --force
```
- Fill out PR description according to provided template.
- Assign yourself as the author (reviewee).
- Request review from @HenryGerretGruning or someone who knows the code.

## Review Process

### Reviewee (Assignee)
- Be reviewed.

### Reviewer
- Rewiew.

## Merging
To be continued...
