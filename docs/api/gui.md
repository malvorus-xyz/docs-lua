# gui

## Constants

- `gui.column_left`
- `gui.column_right`
- `gui.hotkey_hold`
- `gui.hotkey_toggle`

## Reference

| Call | Description | Source |
| --- | --- | --- |
| `gui.button(...)` | gui.button(id, container, label, callback): control | [GuiButton](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L649) |
| `gui.checkbox(...)` | gui.checkbox(id, container, label, default = false): control | [GuiCheckbox](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L492) |
| `gui.color_picker(...)` | gui.color_picker(id, container, label, default = { 255, 255, 255, 255 }): control | [GuiColorPicker](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L563) |
| `gui.combobox(...)` | gui.combobox(id, container, label, items: table, default = 0): control | [GuiCombobox](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L541) |
| `gui.find(...)` | gui.find(label...): control \| nil | [GuiFind](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L710) |
| `gui.for_each_hotkey(...)` | gui.for_each_hotkey(callback(name, key, mode, is_active)) | [GuiForEachHotkey](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L795) |
| `gui.get_control(...)` | gui.get_control(id): control \| nil | [GuiGetControl](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L745) |
| `gui.get_menu_rect(...)` | gui.get_menu_rect(): number, number, number, number | [GuiGetMenuRect](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L776) |
| `gui.group(...)` | gui.group(id, container, label, column = 0): control | [GuiGroup](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L369) |
| `gui.hotkey(...)` | gui.hotkey(id, container, label, default = 0): control | [GuiHotkey](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L632) |
| `gui.is_menu_open(...)` | gui.is_menu_open(): bool | [GuiIsMenuOpen](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L768) |
| `gui.label(...)` | gui.label(id, container, label): control | [GuiLabel](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L690) |
| `gui.multi_combobox(...)` | gui.multi_combobox(id, container, label, items: table, default = 0): control | [GuiMultiCombobox](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L552) |
| `gui.slider(...)` | gui.slider(id, container, label, min, max, default = min, format = "%.2f", integer = false): control | [GuiSlider](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L508) |
| `gui.sub_tab(...)` | gui.sub_tab(id, container, label): control | [GuiSubTab](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L413) |
| `gui.tab(...)` | gui.tab(id, label): control — top-level menu tab, returns its page | [GuiTab](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L329) |
| `gui.textbox(...)` | gui.textbox(id, container, label, default = ""): control | [GuiTextbox](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/gui.cpp#L615) |
