# render

## Constants

- `render.font_bold`
- `render.font_flag_drop_shadow`
- `render.font_flag_none`
- `render.font_flag_outline`
- `render.font_icons`
- `render.font_menu`
- `render.font_small`
- `render.font_visual`
- `render.text_dropshadow`
- `render.text_none`
- `render.text_outline`

## Reference

| Call | Description | Source |
| --- | --- | --- |
| `render.circle(...)` | render.circle(x, y, radius, color, segments = 24, thickness = 1) | [RenderCircle](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L196) |
| `render.circle_filled(...)` | render.circle_filled(x, y, radius, color, segments = 24) | [RenderCircleFilled](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L222) |
| `render.color(...)` | render.color(r, g, b, a = 255) \| render.color(hex): table | [RenderColor](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L56) |
| `render.create_font(...)` | render.create_font(path, size, flags = 0): font | [RenderCreateFont](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L402) |
| `render.get_screen_size(...)` | render.get_screen_size(): number, number | [RenderGetScreenSize](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L341) |
| `render.get_text_size(...)` | render.get_text_size(font, text): number, number | [RenderGetTextSize](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L324) |
| `render.line(...)` | render.line(x1, y1, x2, y2, color, thickness = 1) | [RenderLine](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L172) |
| `render.pop_clip_rect(...)` | render.pop_clip_rect() | [RenderPopClipRect](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L379) |
| `render.push_clip_rect(...)` | render.push_clip_rect(x1, y1, x2, y2, intersect = true) | [RenderPushClipRect](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L356) |
| `render.rect(...)` | render.rect(x1, y1, x2, y2, color, thickness = 1, rounding = 0) | [RenderRect](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L93) |
| `render.rect_filled(...)` | render.rect_filled(x1, y1, x2, y2, color, rounding = 0) | [RenderRectFilled](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L120) |
| `render.rect_filled_multicolor(...)` | render.rect_filled_multicolor(x1, y1, x2, y2, top_left, top_right, bottom_right, bottom_left) | [RenderRectFilledMulticolor](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L144) |
| `render.text(...)` | render.text(font, x, y, text, color, flags = render.font_flag_none) | [RenderText](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L299) |
| `render.triangle(...)` | render.triangle(x1, y1, x2, y2, x3, y3, color, thickness = 1) | [RenderTriangle](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L245) |
| `render.triangle_filled(...)` | render.triangle_filled(x1, y1, x2, y2, x3, y3, color) | [RenderTriangleFilled](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/render.cpp#L272) |
