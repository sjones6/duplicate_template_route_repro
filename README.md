# Duplicate Template Bug Repro

There are two template files, `routes/__bar.tsx` and `routes/__foo.tsx`.

The result is an error during compilation:

```
Path undefined defined by route "routes/__foo" conflicts with route "routes/__bar"
```

Although there should not be any conflicting routes.

The routes should be `/baz` and `/qux`.