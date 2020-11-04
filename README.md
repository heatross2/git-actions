# GitHub Action for running git commands

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/2e073d8e75024da7b1ed20b87aaa99ec)](https://app.codacy.com/gh/heatross2/git-actions?utm_source=github.com&utm_medium=referral&utm_content=heatross2/git-actions&utm_campaign=Badge_Grade)

You can run any `git` command you need. For example, you could run `git status` like this.

```hcl
workflow "My build" {
  resolves = [
    "git command",
  ]
  on = "push"
}

action "git command" {
  uses = "srt32/git-actions@v0.0.3"
  args = "git status"
}
```
