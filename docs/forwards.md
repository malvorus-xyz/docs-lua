# Script forwards & callbacks

A script participates in the frame/event pump two ways: define one of the global functions
below directly, or subscribe any function to a name with `globals.register_callback`. Both
fire for the same dispatch — a script may stack any number of `register_callback`
subscribers next to, or instead of, the classic global-function forward.

## Forwards

| Name | Fires when |
| --- | --- |
| `function on_tick(...)` | per-frame, before the draw pass |
| `function on_paint(...)` | per-frame draw pass, render.* is legal here |
| `function on_menu_toggle(...)` | menu visibility changed, receives the new state |
| `function on_game_event(...)` | game event fired, receives a csgo.event |
| `function on_player_created(...)` | player entity created/destroyed, receives a csgo.entity |
| `function on_player_deleted(...)` | player entity created/destroyed, receives a csgo.entity |
| `function on_config_load(...)` | configuration profile has been read/written |
| `function on_config_save(...)` | configuration profile has been read/written |
| `function on_log(...)` | log line has been emitted, receives (text, level) |
| `function on_shutdown(...)` | script is about to be unloaded |

## globals.register_callback

globals.register_callback(name, callback): subscribes callback to a known forward name (e.g. "on_tick") or a raw game event name (e.g. "bomb_planted"); an event name not already tracked by the listener is added to it lazily on first registration

```lua
-- any forward name above, any number of subscribers
globals.register_callback("on_tick", function() ... end)

-- a raw game event name not covered by a forward: the listener starts tracking it
-- lazily on first registration
globals.register_callback("bomb_planted", function(event) ... end)
```
