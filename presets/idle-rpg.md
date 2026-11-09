# Preset: Idle skilling RPG (kiểu Rocky Idle / Melvor Idle)

Thể loại idle/incremental: luyện kỹ năng (Mining, Woodcutting, Fishing, Farming, Crafting/Smithing),
chiến đấu tự động với quái, thu thập vật phẩm, kho đồ (bank), collection log, tiến độ offline.

Game kiểu này **chủ yếu cần icon**, rất ít animation. Mỗi vật phẩm = 1 icon vuông.

## Danh sách asset cần có

| Nhóm | Ví dụ | Số lượng ước tính | Thư mục |
|---|---|---|---|
| Icon kỹ năng | cuốc, rìu, cần câu, liềm, búa rèn, bình thuốc, kiếm, khiên | 10–15 | `ui/icons/skills/` |
| Quặng & thỏi | đồng, sắt, bạc, vàng, mithril + thỏi tương ứng | 15–25 | `sprites/items/ores/` |
| Gỗ | gỗ thường, sồi, liễu, gỗ ma thuật | 5–8 | `sprites/items/logs/` |
| Cá & đồ ăn | cá sống, cá nướng, bánh mì | 15–20 | `sprites/items/food/` |
| Nông sản & thảo dược | hạt giống, cây thu hoạch | 10–20 | `sprites/items/farming/` |
| Thuốc (potion) | nhiều màu/cấp | 10–15 | `sprites/items/potions/` |
| Trang bị | kiếm, giáp, mũ, khiên theo tier vật liệu | 40+ | `sprites/items/gear/` |
| Đá quý, tiền, rương, chìa khóa | gem, coin, chest, key | 10–20 | `sprites/items/misc/` |
| Quái vật | goblin, slime, skeleton, boss | 15–30 | `sprites/monsters/` |
| UI | panel, nút, thanh XP/HP, khung ô đồ | 1 bộ | `ui/panels/` |

## Nguồn đã kiểm tra giấy phép (2026-11-10)

| Gói | Nội dung | Giấy phép | Ghi công |
|---|---|---|---|
| [496 pixel art icons for medieval/fantasy RPG](https://opengameart.org/node/39455) (tác giả 7Soul) | Icon 34×34: vũ khí, giáp, potion, thức ăn, cá, nguyên liệu | CC0 (tác giả đã chuyển từ CC-BY 3.0 sang public domain) | Không bắt buộc |
| [0x72 DungeonTileset II](https://0x72.itch.io/dungeontileset-ii) | 16×16: quái có animation (orc, skeleton, demon, slime…), item, tileset | CC0 | Không bắt buộc |
| [game-icons.net](https://game-icons.net) | 4.000+ icon vector SVG, đổi màu tự do → hợp làm **icon kỹ năng** | CC BY 3.0 | **Bắt buộc** — ghi tên tác giả từng icon |
| [Kenney](https://kenney.nl/assets) — *Game Icons*, *UI Pack*, *UI Pack RPG Expansion* | Icon UI, panel, thanh tiến trình | CC0 | Không bắt buộc |
| OpenGameArt — bộ CC0 Ingot / Gem / Currency / Rune Icons | Thỏi kim loại, đá quý, tiền | CC0 (theo tên gói — kiểm tra lại trang gốc khi tải) | Không bắt buộc |

## Lưu ý phong cách
- Chọn **một kích thước gốc** (vd 32×32 hoặc 34×34) và scale nguyên lần (×2, ×3) trong Godot,
  bật `texture_filter = Nearest` để pixel không bị mờ.
- Trộn nhiều nguồn dễ lệch phong cách → ưu tiên 7Soul cho item, 0x72 cho quái, Kenney cho UI.
- Icon kỹ năng từ game-icons.net là vector một màu: tô theo màu chủ đạo của từng kỹ năng
  để tạo nhận diện, rồi xuất PNG cùng cỡ với item.
- Không dùng/ sao chép asset của chính Rocky Idle hay RuneScape — chỉ tham khảo thể loại.
