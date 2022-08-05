[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/types-all/main.svg)](https://results.pre-commit.ci/latest/github/asottile/types-all/main)

types-all
=========

A shim for the typeshed changes in mypy 0.900

## installation

```bash
pip install types-all
```

## why

`--install-types` is annoying, this installs all the things in [typeshed]

```
error: Library stubs not installed for "toml" (or incompatible with Python 3.8)
```

(for pre-commit, use something like this)

```yaml
-   repo: https://github.com/pre-commit/mirrors-mypy
    rev: v0.902
    hooks:
    -   id: mypy
        additional_dependencies: [types-all]
```

[typeshed]: https://github.com/python/typeshed
