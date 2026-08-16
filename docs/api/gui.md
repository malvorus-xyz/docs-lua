# gui

## Constants

- `gui.column_left`
- `gui.column_right`
- `gui.hotkey_hold`
- `gui.hotkey_toggle`

## Reference

| Call | Description |
| --- | --- |
| `gui.button(...)` | gui.button(id, container, label, callback): control |
| `gui.checkbox(...)` | gui.checkbox(id, container, label, default = false): control |
| `gui.color_picker(...)` | gui.color_picker(id, container, label, default = { 255, 255, 255, 255 }): control |
| `gui.combobox(...)` | gui.combobox(id, container, label, items: table, default = 0): control |
| `gui.find(...)` | gui.find(label...): control \| nil |
| `gui.for_each_hotkey(...)` | gui.for_each_hotkey(callback(name, key, mode, is_active)) |
| `gui.get_control(...)` | gui.get_control(id): control \| nil |
| `gui.get_menu_rect(...)` | gui.get_menu_rect(): number, number, number, number |
| `gui.group(...)` | gui.group(id, container, label, column = 0): control |
| `gui.hotkey(...)` | gui.hotkey(id, container, label, default = 0): control |
| `gui.is_menu_open(...)` | gui.is_menu_open(): bool |
| `gui.label(...)` | gui.label(id, container, label): control |
| `gui.multi_combobox(...)` | gui.multi_combobox(id, container, label, items: table, default = 0): control |
| `gui.slider(...)` | gui.slider(id, container, label, min, max, default = min, format = "%.2f", integer = false): control |
| `gui.sub_tab(...)` | gui.sub_tab(id, container, label): control |
| `gui.tab(...)` | gui.tab(id, label): control — top-level menu tab, returns its page |
| `gui.textbox(...)` | gui.textbox(id, container, label, default = ""): control |
