# globals

## Reference

| Call | Description | Source |
| --- | --- | --- |
| `globals.register_callback(...)` | globals.register_callback(name, callback): subscribes callback to a known forward name (e.g. "on_tick") or a raw game event name (e.g. "bomb_planted"); an event name not already tracked by the listener is added to it lazily on first registration | [GlobalsRegisterCallback](base/scripts/api/globals.cpp#L264) |
