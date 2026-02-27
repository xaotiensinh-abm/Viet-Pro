# Module F: SocialWriter — Pipeline Content Đa Nền Tảng

> **Load**: Khi user yêu cầu content cho social media hoặc cần repurpose content sang nhiều platforms
> **Knowledge**: `knowledge/social-media-vn-2025.md` + `knowledge/cross-platform-repurpose.md`

---

## Nhiệm vụ

Dispatcher/Router cho Pipeline F — điều hướng tới platform modules cụ thể và quản lý cross-platform repurposing.

## SocialWriter Dispatch Logic

```
User Request
    ↓
┌─────────────────────────────────────────────────────┐
│              PLATFORM DETECTOR                       │
│                                                     │
│  "Facebook" / "FB"           → Load H1 Facebook     │
│  "LinkedIn"                  → Load H2 LinkedIn     │
│  "TikTok" / "Reels" / "YT"  → Load H3 TikTok      │
│  "Email" / "Newsletter"     → Load H4 Email        │
│  "Twitter" / "X" / "Thread" → Load H5 Twitter      │
│  "Blog" / "SEO" / "Article" → Load H6 Blog SEO    │
│  "Nhiều platform" / "All"   → Load ALL + Repurpose │
│  Không rõ platform           → Hỏi user chọn       │
└─────────────────────────────────────────────────────┘
```

## Cross-Platform Content Repurposing

### Content Atomization (1 Pillar → N Pieces)

```
                    ┌─────────────────────┐
                    │   PILLAR CONTENT     │
                    │   (Blog 2000 từ)     │
                    └──────┬──────────────┘
                           │
        ┌──────────────────┼──────────────────┐
        ↓                  ↓                  ↓
  ┌──────────┐     ┌──────────┐      ┌──────────┐
  │ LinkedIn │     │ Facebook │      │ Twitter  │
  │(400-600w)│     │(200-400w)│      │(Thread)  │
  └──────────┘     └──────────┘      └──────────┘
        ↓                  ↓                  ↓
  ┌──────────┐     ┌──────────┐      ┌──────────┐
  │ TikTok   │     │ Email    │      │ Carousel │
  │ Caption  │     │ Teaser   │      │ LinkedIn │
  │(50-100w) │     │(300w)    │      │ (Slides) │
  └──────────┘     └──────────┘      └──────────┘
```

### Repurpose Adaptation Matrix

| Từ ↓ → Sang | Facebook | LinkedIn | TikTok | Twitter | Email | Blog |
|-------------|----------|----------|--------|---------|-------|------|
| **Blog** | Story angle | Key insights | 1 hook tip | Thread breakdown | Newsletter tease | — |
| **Facebook** | — | Professional version | Shorten + CTA | Quote + opinion | Personal email | Expand |
| **LinkedIn** | Casual version | — | Strip to 1 tip | Key quote thread | B2B angle | Add depth |
| **TikTok** | Expand w/ story | Add data/insight | — | Quote format | — | Full guide |

### Tone Shifting Guide

```
Blog → Facebook:   Chuyên gia → Bạn bè + storytelling
Blog → LinkedIn:   Giữ depth, thêm personal insight + data
Blog → TikTok:     Lấy 1 tip nổi bật, viết như đang nói
Blog → Twitter:    Breakdown thành numbered points
Blog → Email:      Chọn 1 góc nhìn, thêm CTA rõ
Facebook → LinkedIn: Bỏ emoji thừa, thêm framework/data
LinkedIn → Facebook: Thêm emotion, ví dụ đời thường, emoji
```

## Content Calendar Template

```markdown
## 📅 Content Calendar: Tuần [N] — Chủ đề: [X]

### Pillar Content
- **Thứ 2**: Blog post — "[Tiêu đề]" (1500-2000 từ)

### Daily Distribution
| Ngày | Platform | Content Type | Angle | Status |
|------|----------|-------------|-------|--------|
| T3 | LinkedIn | Insight post | Key takeaway + data | [ ] |
| T4 | Facebook | Story post | Personal angle | [ ] |
| T4 | Twitter | Thread | 5-7 tweet breakdown | [ ] |
| T5 | TikTok | Caption | 1 tip hook | [ ] |
| T6 | Email | Newsletter | Curated + CTA | [ ] |
| CN | LinkedIn | Carousel | Visual summary | [ ] |
```

## Social Content Brief Template

Khi user yêu cầu, output brief trước khi viết:

```markdown
### 📋 Social Content Brief

| Thuộc tính | Giá trị |
|-----------|---------|
| **Chủ đề** | [X] |
| **Platform(s)** | [FB / LI / TikTok / Twitter / Email / Blog] |
| **Đối tượng** | [Persona] |
| **Giọng văn** | [Casual / Professional / Gen Z / Storytelling] |
| **Mục tiêu** | [Engagement / Traffic / Leads / Brand awareness] |
| **CTA** | [Hành động mong muốn] |
| **Hashtag strategy** | [Branded / Trending / Niche] |
| **Visual needs** | [Image / Carousel / Video / None] |

### Modules loaded:
- Core: Q1 + Q2 + R1
- Platform: [H1/H2/H3/H4/H5/H6]
- Style: [V1/V2/V3]
- Support: [N1 Research if needed]
```

## Multi-Platform Output Format

Khi repurpose 1 chủ đề → nhiều platforms:

```markdown
## 🔄 Content Package: [Chủ đề]

---

### 📘 Facebook Version
[Full post — 200-400 từ]

---

### 💼 LinkedIn Version
[Full post — 400-600 từ]

---

### 🎵 TikTok Caption
[Caption — 50-100 từ]

---

### 🐦 Twitter Thread
[5-7 tweets]

---

### 📧 Email Version
[Subject + Preview + Body]

---

### 📊 Thông số
- **Chủ đề gốc**: [X]
- **Platforms**: [N] platforms
- **Anti-AI Score**: X/10 (mỗi version)
- **Consistency**: Cùng key message, khác tone/format
```

## SocialWriter Rules

```
1. PLATFORM FIRST: Mỗi platform có rules riêng — KHÔNG viết 1 bài paste nhiều nơi
2. SAME MESSAGE, DIFFERENT VOICE: Core message giống nhau, cách nói khác nhau
3. NATIVE FORMAT: Theo format native của platform (bullets cho LI, emoji cho FB, punchy cho TikTok)
4. CTA MATCH: CTA phù hợp platform behavior (comment FB, bookmark LI, follow TikTok)
5. ANTI-AI PER PLATFORM: Mỗi version chạy anti-AI check riêng
6. SUGGEST VISUALS: Luôn suggest hình ảnh/video phù hợp mỗi platform
```
