# Welcome

## About

Generated reference for the sandboxed luajit api that `base/scripts/` scripts run under.

## Getting Started

For runnable scripts covering the gui, render, entities, timers and event api, check out
the examples page.

{% content-ref url="examples.md" %}
[Examples](examples.md)
{% endcontent-ref %}

{% content-ref url="forwards.md" %}
[Script forwards & callbacks](forwards.md)
{% endcontent-ref %}

## Regenerating

Source of truth per api page: the `CreateNamespace`/`CreateType`/`CreateTable` calls in
`base/scripts/engine.cpp` (the lua-visible name -> binding mapping), enriched with the
maintainer comment above each binding in `base/scripts/api_def.h` when one exists, and a
source link into `base/scripts/api/*.cpp`. Nothing on these pages is hand-maintained —
edit the source, not the generated markdown:

```text
py scripts/generate_gitbook.py
```
