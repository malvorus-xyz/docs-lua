# base lua scripting api

Generated reference for the sandboxed luajit api scripts run under (`base/scripts/`).
Regenerate after changing the api surface:

```text
py scripts/generate_gitbook.py
```

Source of truth per page: the `CreateNamespace`/`CreateType`/`CreateTable` calls in
`base/scripts/engine.cpp` (the lua-visible name -> binding mapping), enriched with the
maintainer comment above each binding in `base/scripts/api_def.h` when one exists, and a
source link into `base/scripts/api/*.cpp`. Nothing on these pages is hand-maintained —
edit the source, not the generated markdown.
