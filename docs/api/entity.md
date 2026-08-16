# entity

> csgo build only — unavailable in `sandbox.exe`.

## Reference

| Call | Description | Source |
| --- | --- | --- |
| `entity[...]` | — | [EntityIndex](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L358) |
| `entity:get_class(...)` | entity:get_class(): string | [EntityGetClass](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L508) |
| `entity:get_eye_position(...)` | entity:get_origin() / get_eye_position(): vec3 | [EntityGetEyePosition](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L590) |
| `entity:get_hitbox_position(...)` | entity:get_hitbox_position(hitbox): vec3 | [EntityGetHitboxPosition](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L605) |
| `entity:get_index(...)` | entity:get_index() / is_valid() / is_dormant() / is_player() / is_alive() / is_enemy() | [EntityGetIndex](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L422) |
| `entity:get_origin(...)` | entity:get_origin() / get_eye_position(): vec3 | [EntityGetOrigin](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L575) |
| `entity:get_player_info(...)` | entity:get_player_info(): table \| nil | [EntityGetPlayerInfo](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L623) |
| `entity:get_pointer(...)` | entity:get_pointer(): number | [EntityGetPointer](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L645) |
| `entity:get_prop(...)` | entity:get_prop(name, element = 0): value | [EntityGetProp](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L523) |
| `entity:is_alive(...)` | entity:get_index() / is_valid() / is_dormant() / is_player() / is_alive() / is_enemy() | [EntityIsAlive](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L476) |
| `entity:is_dormant(...)` | entity:get_index() / is_valid() / is_dormant() / is_player() / is_alive() / is_enemy() | [EntityIsDormant](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L446) |
| `entity:is_enemy(...)` | entity:get_index() / is_valid() / is_dormant() / is_player() / is_alive() / is_enemy() | [EntityIsEnemy](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L491) |
| `entity:is_player(...)` | entity:get_index() / is_valid() / is_dormant() / is_player() / is_alive() / is_enemy() | [EntityIsPlayer](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L461) |
| `entity:is_valid(...)` | entity:get_index() / is_valid() / is_dormant() / is_player() / is_alive() / is_enemy() | [EntityIsValid](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L437) |
| `entity:set_prop(...)` | entity:set_prop(name, value, element = 0) | [EntitySetProp](https://github.com/malvorus-xyz/base/blob/master/base/scripts/api/entity.cpp#L548) |
