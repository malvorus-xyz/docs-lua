# docs-lua

Generated GitBook-style reference for the `base` project's sandboxed luajit scripting api,
built into a static site with [mdBook](https://rust-lang.github.io/mdBook/) and published to
GitHub Pages by `.github/workflows/deploy.yml` on every push to `main`.

Content under `docs/` is generated — do not hand-edit it. Regenerate from the `base` repo:

```text
py scripts/generate_gitbook.py
```

then copy `base/docs/` over this repo's `docs/` directory, commit, and push.

Local preview (requires the [mdBook](https://github.com/rust-lang/mdBook) binary):

```text
mdbook serve
```
