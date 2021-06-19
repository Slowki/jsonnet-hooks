# jsonnet-hooks

[`pre-commit`](https://pre-commit.com/) hooks to run `jsonnetfmt`

## `jsonnetfmt` Hook

### Using the System version of `jsonnetfmt`

```yaml
repos:
  - repo: https://github.com/Slowki/bazel-hooks
    rev: e4928686d7ddc7b22c2e8dae3649229cfa16c0e8
    hooks:
      - id: jsonnetfmt
```

### Using `jsonnetfmt` via Bazel

`bazel-jsonnetfmt` runs the `@jsonnet//cmd:jsonnetfmt` target.

```yaml
repos:
  - repo: https://github.com/Slowki/bazel-hooks
    rev: e4928686d7ddc7b22c2e8dae3649229cfa16c0e8
    hooks:
      - id: bazel-jsonnetfmt
```
