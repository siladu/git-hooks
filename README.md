# git-hooks
Usefull git hooks and [pre-commit](https://pre-commit.com) config.

## To Use

Save the the file somewhere on disk, e.g. `~/.githooks/pre-commit-config.yaml`

```
repos:
  - repo: https://github.com/siladu/git-hooks
    rev: 1.0.0 
    hooks:
      - id: add-dco
      - id: gradle-spotless
```

then run 
```
pre-commit install -c ~/.githooks/pre-commit-config.yaml -t pre-commit -t commit-msg
```
on the repo you want to enable commit hooks for.
