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

| Call | Description |
| --- | --- |
| `render.circle(...)` | render.circle(x, y, radius, color, segments = 24, thickness = 1) |
| `render.circle_filled(...)` | render.circle_filled(x, y, radius, color, segments = 24) |
| `render.color(...)` | render.color(r, g, b, a = 255) \| render.color(hex): table |
| `render.create_font(...)` | render.create_font(path, size, flags = 0): font |
| `render.get_screen_size(...)` | render.get_screen_size(): number, number |
| `render.get_text_size(...)` | render.get_text_size(font, text): number, number |
| `render.line(...)` | render.line(x1, y1, x2, y2, color, thickness = 1) |
| `render.pop_clip_rect(...)` | render.pop_clip_rect() |
| `render.push_clip_rect(...)` | render.push_clip_rect(x1, y1, x2, y2, intersect = true) |
| `render.rect(...)` | render.rect(x1, y1, x2, y2, color, thickness = 1, rounding = 0) |
| `render.rect_filled(...)` | render.rect_filled(x1, y1, x2, y2, color, rounding = 0) |
| `render.rect_filled_multicolor(...)` | render.rect_filled_multicolor(x1, y1, x2, y2, top_left, top_right, bottom_right, bottom_left) |
| `render.text(...)` | render.text(font, x, y, text, color, flags = render.font_flag_none) |
| `render.triangle(...)` | render.triangle(x1, y1, x2, y2, x3, y3, color, thickness = 1) |
| `render.triangle_filled(...)` | render.triangle_filled(x1, y1, x2, y2, x3, y3, color) |
