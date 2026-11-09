# Game Asset Library

Thư viện tổng hợp nguồn asset 2D **miễn phí** để dùng lại cho các game Godot 4.x
(LAST HAVEN, Lonely Immortality và các dự án sau).

> Nguyên tắc: ưu tiên **CC0** (không cần ghi công). Asset CC-BY/MIT/Unlicense được phép
> nhưng phải ghi vào [`LICENSES.md`](LICENSES.md) trước khi đưa vào game.

## Cấu trúc thư mục

```
sprites/
  characters/   # nhân vật, NPC, quái
  zombies/      # dành cho LAST HAVEN
  effects/      # hiệu ứng, particle, phép thuật
  items/        # vật phẩm, vũ khí, đan dược
tilesets/
  topdown/
  platformer/
ui/
  icons/
  panels/
audio/
  sfx/
  music/
fonts/
```

Mỗi gói asset đặt trong thư mục riêng: `<loại>/<tác-giả>_<tên-gói>/`, kèm file
`SOURCE.txt` ghi link gốc + giấy phép.

## Danh mục nguồn

### Kho tổng hợp (ưu tiên số 1)
| Nguồn | Giấy phép | Phù hợp |
|---|---|---|
| [Kenney](https://kenney.nl/assets) | CC0 | Mọi thể loại: top-down, platformer, UI, icon, âm thanh |
| [OpenGameArt](https://opengameart.org) — lọc CC0 | Nhiều loại | Icon RPG, tileset, sfx |
| [OpenGameArt — "good CC0 stuff"](https://opengameart.org/content/good-cc0-stuff) | CC0 | Bộ tuyển chọn |
| [itch.io — CC0 sprites](https://itch.io/game-assets/assets-cc0/tag-sprites) | CC0 | Gói từ cộng đồng |

### Tác giả itch.io đáng theo dõi
| Tác giả | Gói tiêu biểu | Giấy phép |
|---|---|---|
| [Ansimuz](https://ansimuz.itch.io) | 2D Platform, Metroidvania, 16-bit pixel | Kiểm tra từng gói (nhiều gói CC0) |
| [0x72](https://0x72.itch.io) | µFantasy Tileset, Dungeon Tileset | Kiểm tra từng gói |
| [Pixel Frog](https://pixelfrog-assets.itch.io) | Pixel Adventure, Treasure Hunters | Kiểm tra từng gói |
| [VEXED](https://v3x3d.itch.io) | Deep Night, Bit Bonanza, Retro Lines | CC0 |

### Repo GitHub
| Repo | Giấy phép | Ghi chú |
|---|---|---|
| [gdquest/game-sprites](https://github.com/gdquest/game-sprites) | Xem repo | Asset dành cho prototype |
| [pigdevstudio/assets](https://github.com/pigdevstudio/assets) | Unlicense | Sprite, spritesheet, âm thanh dùng sẵn cho Godot |
| [godotengine/godot-demo-projects](https://github.com/godotengine/godot-demo-projects) | MIT | Tham khảo cấu trúc scene/code |
| [gdquest-demos/godot-open-rpg](https://github.com/gdquest-demos/godot-open-rpg) | Xem repo | RPG 2D mẫu |

## Gợi ý theo dự án

**LAST HAVEN (zombie survival, mobile 2D)**
- Kenney: *Top-down Shooter*, *Zombie*-themed character packs, *Particle Pack*, *UI Pack*
- 0x72: Dungeon Tileset II (bối cảnh hầm/khu tàn tích)

**Lonely Immortality (tu tiên)**
- OpenGameArt: bộ icon RPG CC0 (rune, gem, ingot, currency) → làm đan dược, linh thạch
- Kenney: *Fantasy UI Borders*, *Game Icons*

**Idle skilling RPG (kiểu Rocky Idle / Melvor Idle)**
- Xem preset chi tiết: [`presets/idle-rpg.md`](presets/idle-rpg.md)
- Item: 7Soul 496 RPG icons (CC0) · Quái: 0x72 DungeonTileset II (CC0)
- Icon kỹ năng: game-icons.net (CC BY 3.0 — phải ghi công) · UI: Kenney (CC0)

## Quy trình thêm asset

1. Kiểm tra giấy phép trên trang gốc (không tin vào mô tả bên thứ ba).
2. Tải về, giải nén vào đúng thư mục theo quy ước tên.
3. Tạo `SOURCE.txt` (link, tác giả, giấy phép, ngày tải).
4. Nếu không phải CC0 → thêm dòng vào `LICENSES.md`.
5. Commit: `add: <loại>/<tác-giả>_<tên-gói>`.
