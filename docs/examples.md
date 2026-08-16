# Examples

Small, complete scripts. Drop one in `<scripts>/` (next to `base.dll`) and load it from the
scripts menu.

## Minimal skeleton

Every forward is optional; define only what you use.

```lua
--. name: example
--. description: minimal skeleton
--. author: you

function on_tick()
    -- runs every frame, before the draw pass
end

function on_paint()
    -- runs every frame, render.* is only legal in here
    local w, h = render.get_screen_size()
    render.text(render.font_menu, 4, 4, "hello from lua", render.color(255, 255, 255))
end
```

## Building a menu page

```lua
local tab = gui.tab("example", "Example")
local group = gui.group("main", tab, "Main", gui.column_left)

local enabled = gui.checkbox("enabled", group, "Enabled", false)
local size = gui.slider("size", group, "Size", 1, 10, 5, "%d", true)

gui.button("reset", group, "Reset", function(control)
    size:set_value(5)
end)

function on_tick()
    if not enabled:get_value() then
        return
    end
    -- ... use size:get_value() ...
end
```

## globals.register_callback

Stack any number of subscribers on a forward name, or on a raw game event name the fixed
listener list in `EVENT::Setup()` never covered -- the listener starts tracking it lazily on
first registration.

```lua
globals.register_callback("on_tick", function()
    -- a second on_tick subscriber, independent of the classic `function on_tick()` above
end)

globals.register_callback("bomb_planted", function(event)
    print("bomb planted by player " .. event:get_int("userid"))
end)
```

## Drawing on players (esp-style loop)

```lua
function on_paint()
    local me = engine.get_local_player()
    if me == nil or not me:is_alive() then
        return
    end

    entities.for_each_player(function(entity)
        if not entity:is_valid() or entity:is_dormant() or not entity:is_alive() or not entity:is_enemy() then
            return
        end

        local head = entity:get_hitbox_position(0)
        local x, y = utils.world_to_screen(head)
        if x ~= nil then
            render.text(render.font_menu, x, y, "enemy", render.color(255, 64, 64), render.text_dropshadow)
        end
    end)
end
```

## Timers and persistence

```lua
local counter = 0

utils.new_timer(1000, function()
    counter = counter + 1
    database.save("counter", counter)
end):start()

function on_shutdown()
    fs.write("last_run.txt", utils.get_date())
end
```

## Reading a convar

```lua
function on_tick()
    local sensitivity = cvar["sensitivity"]:get_float()
end
```
