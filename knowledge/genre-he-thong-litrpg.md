# Genre Knowledge: Hệ Thống / LitRPG

> **Tone**: Game-like + Tactical
> **Đặc thù**: Stats, quest, loot, level up notifications

---

## 1. System UI Design

### Notification Format
```
╔══════════════════════════════════════╗
║  🔔 HỆ THỐNG THÔNG BÁO              ║
║  Quest hoàn thành: [Tên quest]       ║
║  Phần thưởng: +500 EXP, +1 Skill    ║
║  ⚡ Level Up! Lv.12 → Lv.13          ║
╚══════════════════════════════════════╝
```

### Stat Screen
```
┌─── NHÂN VẬT: [Tên] ─────────────────┐
│ Level: 13          │ Class: Kiếm Sĩ  │
│ HP: 450/450        │ MP: 280/300     │
├────────────────────┼─────────────────┤
│ STR: 24 (+2)       │ AGI: 31 (+1)   │
│ INT: 18            │ VIT: 22        │
│ LCK: 7             │ CHA: 12       │
├────────────────────┴─────────────────┤
│ EXP: 2,340/5,000   ███████░░░ 47%   │
│ Skill Points: 3    │ Gold: 12,500   │
└──────────────────────────────────────┘
```

### Loot Drop
```
⚔️ CHIẾN LỢI PHẨM
├─ 🟢 [Thường] Thảo dược cấp 2 ×3
├─ 🔵 [Hiếm] Kiếm Sắt Phong — ATK +15
└─ 🟣 [Sử thi] ???  (Cần giám định)
```

## 2. Best Practices

### Mechanics Phục Vụ Plot
```
❌ TRÁNH: Stat dump mỗi trang
"HP tăng 5, MP tăng 3, STR tăng 1, AGI tăng 2..."

✅ LÀM: Stats có ý NGHĨA cho câu chuyện
"[STR chỉ 8 — Hệ thống ghi chú: 'Yếu hơn một bà cụ trung bình.']
Lâm nhìn dàn quái vật trước mặt. Chạy thôi."
```

### Notification Pacing
- Tối đa 1-2 notifications/scene
- Full stat screen: 1 lần/chapter, thường cuối chapter
- Notification PHẢI tạo reaction từ MC
- KHÔNG notification im lặng — MC luôn phản ứng

### Level Up = Satisfying Moment
```
Mỗi level up PHẢI có:
1. Physical change (MC cảm thấy gì)
2. Emotional reaction (phấn khích? sợ? bất ngờ?)
3. Story impact (mở khóa gì mới? thay đổi gì?)
```

## 3. System Types

| Loại | Đặc điểm | Ví dụ |
|------|---------|-------|
| **Hệ Thống Nhiệm Vụ** | Quest → reward → level | Hệ thống TĐTL |
| **Gacha System** | Random reward, tỷ lệ SSR | "Quay x10 nhận 9 rác 1 thần khí" |
| **Skill Tree** | Chọn build, trade-off | "ATK hay DEF? Không đủ points" |
| **Crafting** | Thu thập nguyên liệu, chế tạo | Luyện đan + forge |
| **Achievement** | Unlock hidden bonuses | "Giết 100 slime → Title: Diệt Slime Đại Sư" |

## 4. Comedy từ System

```
- System sarcastic: "Quest: Sống sót qua ngày hôm nay. Độ khó: S"
- Glitch/bug hệ thống: "Lv.999 nhưng HP = 1"
- Notification spam: "Ding ding ding ding — TẮT ĐI!"
- Hidden quest absurd: "Ăn 100 bát phở → Unlock: Phở Master"
- Pay-to-win jokes: "Nạp VND để mở khóa tính năng premium"
```

## 5. Progression Design

```
Arc 1: Levels 1-10  — Tutorial, hiểu cơ bản
Arc 2: Levels 10-30 — First major challenge, team building
Arc 3: Levels 30-50 — Plot twist, system có dark side
Arc 4: Levels 50+   — Endgame content, system origin reveal

QUAN TRỌNG: Mỗi arc PHẢI reveal thêm về BẢN CHẤT system
→ System không chỉ là tool, nó có AGENDA riêng
```
