This fails:

```
bazel build foo # fails
```

While this doesn't:

```
cd foo
pnpm i
pnpm tsc
```
