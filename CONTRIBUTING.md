# How we work

For every sleepacta repository.

## Issues

- Every piece of work has an issue in the repository of the code it touches, opened with one of
  the forms: **Task** (the default), **Bug** or **Feature**. The title is enough.
- **Area** and **Priority** are organization fields: set them in the issue's sidebar or in the
  project.
- The issue lands in the [Sleepacta](https://github.com/orgs/sleepacta/projects/1) project on its
  own; set its **Sprint** there.
- Move the card on the Board to change its status (To Do, In Progress, Done). A card in Done closes
  the issue; a closed issue goes to Done.
- An issue number is only unique within its repository: outside it, say "frontend #18" or paste the
  link.

## Commits

One line, the issue number first:

```
GH-18 Title
GH-18 Title, fixes #18      closes the issue when the commit reaches the default branch
```

- `GH-18` and `#18` are the same to GitHub: a link to issue 18 of this repository, and the commit
  shows up on the issue. `#18 Title` works too, but only with `git commit -m`: in an editor (commit
  without `-m`, amend, rebase, merge) git drops lines that start with `#`.
- An issue in another repository: `sleepacta/exam-pipeline#12`.
- Older commits with `SAWOR-NNNN` refer to Jira tickets.
