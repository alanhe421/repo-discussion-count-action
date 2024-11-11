## About

just use `${{steps.repo-discussion.outputs.count}}` to get repo's discussion-count.

### Example

```yml
...

on:
  # Triggers the workflow on push or pull request events but only for the master branch
  watch:
    action: started

steps:
- name: Discussion Count
  id: repo-discussion
  uses: alanhe421/repo-discussion-count-action@master

...

```
