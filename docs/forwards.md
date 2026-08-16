# Script forwards & callbacks

A script subscribes to a forward by name with `globals.register_callback` -- any number of
independent callbacks may stack on the same name, and every subscriber fires in
registration order.

## Forwards

| Name | Fires when |
| --- | --- |
| `"on_tick"` | per-frame, before the draw pass |
| `"on_paint"` | per-frame draw pass, render.* is legal here |
| `"on_menu_toggle"` | menu visibility changed, receives the new state |
| `"on_game_event"` | game event fired, receives a csgo.event |
| `"on_player_created"` | player entity created/destroyed, receives a csgo.entity |
| `"on_player_deleted"` | player entity created/destroyed, receives a csgo.entity |
| `"on_config_load"` | configuration profile has been read/written |
| `"on_config_save"` | configuration profile has been read/written |
| `"on_log"` | log line has been emitted, receives (text, level) |
| `"on_shutdown"` | script is about to be unloaded |

## globals.register_callback

globals.register_callback(name, callback): subscribes callback to a known forward name (e.g. "on_tick") or a raw game event name (e.g. "bomb_planted"); an event name not already tracked by the listener is added to it lazily on first registration

```lua
-- any forward name above, any number of subscribers
globals.register_callback("on_tick", function() ... end)

-- a raw game event name not covered by a forward: the listener starts tracking it
-- lazily on first registration
globals.register_callback("bomb_planted", function(event) ... end)
```
