# 📖 USERGUIDE — Viet-Pro v3.0 Universal Vietnamese Content Studio

> **Phiên bản**: 3.0 | **Cập nhật**: 2026-02-27
> **Một câu**: Viết MỌI loại content tiếng Việt — không ai biết là AI viết.

---

## Mục lục

1. [Giới thiệu](#-giới-thiệu)
2. [Cách kích hoạt](#-cách-kích-hoạt)
3. [7 Pipelines — Viết gì cũng được](#-7-pipelines--viết-gì-cũng-được)
4. [Hướng dẫn từng Pipeline](#-hướng-dẫn-từng-pipeline)
5. [Platforms hỗ trợ](#-platforms-hỗ-trợ)
6. [Anti-AI Engine — Vượt mọi detector](#-anti-ai-engine--vượt-mọi-detector)
7. [Nâng cấp bài viết có sẵn](#-nâng-cấp-bài-viết-có-sẵn)
8. [Hệ thống Knowledge](#-hệ-thống-knowledge)
9. [FAQ & Tips nâng cao](#-faq--tips-nâng-cao)

---

## 🎯 Giới thiệu

**Viet-Pro** là skill viết content tiếng Việt chuyên nghiệp, được thiết kế để:

- ✅ Viết **7 loại content** khác nhau (truyện, bài viết, tài liệu, slide, nghiên cứu, social media, script video)
- ✅ Hỗ trợ **8 nền tảng** (Facebook, LinkedIn, TikTok, Twitter, Email, Blog, Zalo, Instagram)
- ✅ Vượt qua **mọi AI detector** nhờ Anti-AI Engine 25 lớp kiểm tra
- ✅ Giọng văn **chuẩn người Việt** — thành ngữ, tục ngữ, cảm xúc thật

### Ai nên dùng?

| Người dùng | Dùng Viet-Pro để |
|-----------|-----------------|
| Content Creator | Viết bài Facebook, LinkedIn, Blog nhanh gấp 5x |
| Marketer | Email marketing, social media calendar, ads copy |
| Giảng viên | Soạn lesson plan, giáo trình, slide bài giảng |
| Nghiên cứu sinh | Literature review, white paper, policy brief |
| Nhà văn | Viết truyện fiction 8 thể loại (tiên hiệp → kinh dị) |
| YouTuber/TikToker | Script video, podcast outline |

---

## 🚀 Cách kích hoạt

### Cách 1: Gõ lệnh trực tiếp

```
/viet-pro     → Mở Viet-Pro, hỏi bạn muốn viết gì
/novel        → Vào thẳng Pipeline A: Viết truyện
/write        → Auto-detect loại content từ yêu cầu
```

### Cách 2: Nói tự nhiên (auto-detect)

Viet-Pro tự kích hoạt khi bạn yêu cầu bất kỳ tác vụ viết tiếng Việt nào:

```
"Viết bài Facebook về AI trong kinh doanh"     → Pipeline B + H1
"Soạn lesson plan marketing digital"             → Pipeline C
"Tạo slide pitch startup 10 slides"             → Pipeline D
"Viết literature review chuyển đổi số"           → Pipeline E
"Viết 1 chủ đề thành 5 bài cho 5 platform"      → Pipeline F
"Viết script YouTube 10 phút"                    → Pipeline G
"Viết chapter 1 truyện đô thị tu tiên"           → Pipeline A
```

### Bước đầu tiên khi kích hoạt

Viet-Pro sẽ hỏi bạn **tối đa 6 câu** (chỉ hỏi những gì chưa biết):

```
1. CHỦ ĐỀ:     Viết về gì?
2. LOẠI:        Bài viết / Slide / Nghiên cứu / ...? (auto-detect)
3. ĐỐI TƯỢNG:  Gen Z / Chuyên gia / Học sinh / Đại chúng?
4. PLATFORM:    Facebook / LinkedIn / Blog / Slide / ...?
5. GIỌNG VĂN:  Thân thiện / Chuyên gia / Storytelling / Học thuật?
6. ĐỘ DÀI:     Ngắn / Vừa / Dài / Tùy bạn quyết định?
```

> 💡 **Tip**: Cung cấp càng nhiều thông tin trong yêu cầu ban đầu → Viet-Pro hỏi ít hơn, giao bài nhanh hơn.

---

## 📊 7 Pipelines — Viết gì cũng được

```
┌──────────────────────────────────────────────────────────┐
│                    VIET-PRO v3.0                          │
│                                                          │
│  📖 A: Novel Writer    → Truyện fiction (tiên hiệp, ...)  │
│  📝 B: Viet-Pro Swarm  → Bài viết, blog, email           │
│  📚 C: EduWriter       → Tài liệu học tập, lesson plan   │
│  🎤 D: SlideWriter     → Slide, thuyết trình              │
│  🔬 E: ResearchWriter  → Nghiên cứu, luận văn            │
│  📱 F: SocialWriter    → Social media đa nền tảng         │
│  🎬 G: ScriptWriter    → Script video, podcast            │
└──────────────────────────────────────────────────────────┘
```

---

## 📘 Hướng dẫn từng Pipeline

### Pipeline A: Novel Writer — Viết truyện Fiction

**Trigger**: `/novel`, "viết truyện", "viết chapter"

**8 thể loại hỗ trợ**:
Tiên Hiệp · Đô Thị Tu Tiên · Hệ Thống/LitRPG · Ngôn Tình · Kiếm Hiệp · Thriller · Sci-Fi · Kinh Dị

**Các lệnh**:

| Lệnh | Mô tả |
|-------|--------|
| `/novel init` | Tạo world-bible, story state, thư mục chapters |
| `/novel outline` | Tạo outline arc/volume |
| `/novel chapter [N]` | Viết chapter N (full 7-agent pipeline) |
| `/novel qa [N]` | Chấm điểm chapter theo 130đ |
| `/novel edit [N]` | Chỉ chạy Editor polish |
| `/novel humanize [N]` | Chạy 12-layer humanization |
| `/novel status` | Xem tiến độ + QA scores |

**Ví dụ sử dụng**:

```
User: /novel init
→ Thể loại: Đô Thị Tu Tiên
→ MC: Nguyễn Lâm, 25 tuổi, IT, Sài Gòn
→ Hệ thống: Tu Luyện App (giấu trên điện thoại)

User: /novel chapter 1
→ Output: Chapter 3000-5000 từ + QA scorecard 130 điểm
```

**Chất lượng đảm bảo**: 7 agent pipeline (Orchestrator → WorldBuilder → Plotter → Writer → Humanizer → QA Scorer → Editor). Mỗi chapter được chấm 130 điểm, dưới 85 → rewrite.

---

### Pipeline B: Viet-Pro Swarm — Bài viết & Content

**Trigger**: "viết bài", "viết content", "tạo bài đăng"

**Framework hỗ trợ**: PAS · BAB · AIDA · Hero's Journey

**Ví dụ sử dụng**:

```
User: Viết bài Facebook 500 từ về "Tại sao SME cần chuyển đổi số ngay"
      Audience: Chủ DN, tone chuyên gia nhưng thân thiện

→ Output:
  - Bài 500 từ, framework PAS
  - Anti-AI Score: 8/10
  - Gợi ý: CTA, hashtag, hình ảnh
```

---

### Pipeline C: EduWriter — Tài liệu học tập

**Trigger**: "soạn giáo trình", "lesson plan", "tạo quiz", "viết workbook"

**6 loại tài liệu**: Lesson Plan · Giáo Trình · Workbook · Quiz/Assessment · Study Guide · Bài Giảng

**Đặc biệt**: Dùng Bloom's Taxonomy 6 cấp để thiết kế mục tiêu học tập.

**Ví dụ sử dụng**:

```
User: Soạn lesson plan "Content Marketing cơ bản"
      Đối tượng: SV Marketing năm 3
      Thời lượng: 90 phút

→ Output:
  - Lesson plan theo BOPPPS model
  - Mục tiêu: Bloom verbs (phân tích, áp dụng, đánh giá)
  - Activities: Case study, role-play, quiz nhanh
  - Assessment rubric
```

---

### Pipeline D: SlideWriter — Slide & Thuyết trình

**Trigger**: "tạo slide", "soạn bài thuyết trình", "presentation"

**4 Narrative arcs**: Problem-Solution · Minto Pyramid · Teaching Arc · TED-Style

**Ví dụ sử dụng**:

```
User: Tạo slide deck pitch startup EdTech, 10 slides
      Audience: Nhà đầu tư Angel VN

→ Output:
  - 10 slides markdown (1 ý/slide, ≤6 dòng/slide)
  - Speaker notes conversational style
  - Visual recommendations (chart type, image suggestions)
  - Narrative arc: Problem → Solution → Market → Traction → Ask
```

---

### Pipeline E: ResearchWriter — Tài liệu nghiên cứu

**Trigger**: "viết luận", "literature review", "white paper", "policy brief"

**5 loại tài liệu**: Literature Review · Research Paper · White Paper · Policy Brief · Case Study

**Ví dụ sử dụng**:

```
User: Viết literature review 2000 từ
      Chủ đề: Chuyển đổi số DNNVV Việt Nam
      Citation format: APA 7th

→ Output:
  - Literature review cấu trúc IMRaD
  - Citations APA 7th (≥10 sources Tier 1-2)
  - Hedging language chuẩn học thuật VN
  - CRAAP-verified sources
```

---

### Pipeline F: SocialWriter — Content đa nền tảng

**Trigger**: "viết cho 5 platform", "content calendar", "cross-platform"

**Chiến lược**: 1 Pillar Content → N Social Posts (Content Atomization)

**Ví dụ sử dụng**:

```
User: Chủ đề "5 xu hướng AI Marketing 2026"
      Tạo bộ content cho 5 platforms

→ Output:
  1. LinkedIn: Thought leadership 400 từ (data + insight)
  2. Facebook: Story post 300 từ (personal angle)
  3. TikTok: Caption 80 từ (scroll-stopper)
  4. Twitter: Thread 5 tweets (breakdown từng xu hướng)
  5. Email: Newsletter 500 từ (curated + CTA)
  + Content Calendar tuần gợi ý
```

> 💡 **Mỗi version có tone/format KHÁC nhau** — không copy-paste. Anti-AI check riêng cho từng version.

---

### Pipeline G: ScriptWriter — Script Video & Podcast

**Trigger**: "viết script", "kịch bản video", "podcast script"

**3 format**: YouTube Long-form (8-20 phút) · TikTok/Reels (15-60 giây) · Podcast (20-45 phút)

**Ví dụ sử dụng**:

```
User: Viết script YouTube 10 phút
      Chủ đề: "Hành trình startup từ 0 đến 1 tỷ"
      Style: Storytelling + data

→ Output:
  - Script với timing markers (⏱️ 00:00)
  - B-roll suggestions (🎥)
  - On-screen text cues (📱)
  - Engagement hooks mỗi 3-5 phút
  - Speaking rhythm tự nhiên
```

---

## 🌐 Platforms hỗ trợ

| # | Platform | Module | Đặc thù |
|---|----------|--------|---------|
| H1 | **Facebook** | `platform-facebook.md` | Storytelling, emoji, 150-500 từ |
| H2 | **LinkedIn** | `platform-linkedin.md` | Professional, data-driven, 200-800 từ |
| H3 | **TikTok** | `platform-tiktok.md` | Gen Z, scroll-stopper, 50-150 từ |
| H4 | **Email** | `platform-email.md` | Subject line formula, 300-800 từ |
| H5 | **Twitter/X** | `platform-twitter.md` | Thread architecture, ≤280/tweet |
| H6 | **Blog SEO** | `platform-blog-seo.md` | SEO checklist, 1000-3000 từ |
| H7 | **Zalo OA** | `platform-zalo.md` | Broadcast, formal-friendly, ≤500 từ |
| H8 | **Instagram** | `platform-instagram.md` | Visual-first, carousel, 15-25 hashtags |

> 💡 **Chỉ cần nói platform** — Viet-Pro tự load module tương ứng và viết đúng format.

---

## 🔒 Anti-AI Engine — Vượt mọi detector

Mọi bài viết đều chạy qua **Anti-AI Engine (R1)** trước khi giao cho bạn.

### Hoạt động thế nào?

```
Bài viết draft
    ↓
[Quét 25 AI Tells] → Phát hiện pattern AI → Fix ngay
    ↓
[Human Seed Injection] → Thêm anecdote, humor, thành ngữ VN
    ↓
[10-Question Final Check] → Chấm điểm
    ↓
Score ≥7/10 → ✅ DELIVER
Score <7/10 → 🔄 REWRITE toàn bộ
```

### 6 Rules bất khả xâm phạm

| Rule | Nội dung | Ví dụ |
|------|---------|-------|
| **1. Zero AI Tells** | Không bao giờ có pattern AI | ❌ "Trong bối cảnh hiện nay..." |
| **2. Burstiness** | Xen câu ngắn-dài, vary paragraph | Câu 5 từ → Câu 25 từ → Câu 8 từ |
| **3. Vietnamese Soul** | Thành ngữ, tục ngữ, cách nói VN | "Nước đến chân mới nhảy" |
| **4. Human Fingerprint** | Anecdote, opinion, humor | "Nói thật, tôi cũng fail cái này" |
| **5. Show Don't Tell** | Hành động thay mô tả (fiction) | ❌ "buồn" → ✅ "mắt cay cay" |
| **6. Final Check 10 câu** | Tự chấm trước khi giao | Score ≥7 → ship, <7 → rewrite |

---

## ✨ Nâng cấp bài viết có sẵn

Bạn có bài viết cũ hoặc bài AI-generated muốn "người hóa"? Dùng **Module M1**:

```
User: [Paste bài viết] + "Anti-AI hóa bài này"

→ Output:
  🔴 TRƯỚC (Score: 3/10)
  > "Trong bối cảnh hiện nay, việc chuyển đổi số..."
  Vấn đề: AI pattern, monotone, no personality

  🟢 SAU (Score: 9/10)
  > "Tuần trước sếp tôi hỏi: 'Chuyển đổi số là gì?' Tôi cười..."
  Đã fix: Storytelling, personal voice, burstiness, VN soul
```

---

## 📚 Hệ thống Knowledge

Viet-Pro có **21 knowledge files** — bạn KHÔNG cần đọc, chúng tự động load theo context:

### Core (luôn hoạt động)

| File | Chức năng |
|------|----------|
| `anti-ai-humanization.md` | 25 AI tells, bảng thay thế từ |
| `emotional-writing-vn.md` | 8 emotion triggers, 12 tu từ |
| `natural-language-vn.md` | 15 AI patterns cần tránh |
| `punctuation-patterns-vn.md` | Dấu câu chuẩn NĐ 30/2020 |
| `fact-check-system.md` | CRAAP test, source tiers VN |
| `vietnamese-idioms-db.md` | 90+ thành ngữ theo 9 chủ đề |
| `golden-samples-vn.md` | 5 bài mẫu với phân tích WHY |

### Pipeline-specific (load theo yêu cầu)

| File | Pipeline |
|------|---------|
| `edu-pedagogy-bloom.md` | C: Bloom's Taxonomy, BOPPPS, 5E |
| `presentation-design-vn.md` | D: Slide design, narrative arcs |
| `academic-writing-vn.md` | E: Citation APA/Harvard/IEEE |
| `social-media-vn-2025.md` | B+F: Demographics, algorithm VN |
| `cross-platform-repurpose.md` | F: Atomization, tone shifting |

### Genre (fiction — Pipeline A)

8 files: Tiên Hiệp · Đô Thị · Hệ Thống · Ngôn Tình · Kiếm Hiệp · Thriller · Sci-Fi · Kinh Dị

---

## 💡 FAQ & Tips nâng cao

### Bài viết vẫn giống AI — làm sao?

```
Nói: "Bài này vẫn giống AI, viết lại tự nhiên hơn"
→ Viet-Pro sẽ: reload R1 Anti-AI → identify chỗ AI → rewrite TOÀN BỘ
```

### Muốn giọng văn custom?

```
Mô tả chi tiết: "Giọng như anh Dũng TQ — chuyên gia nhưng hài hước, 
hay kể chuyện cá nhân, dùng ẩn dụ đời thường"
→ Viet-Pro sẽ tạo voice persona riêng cho bạn
```

### Viết nhanh hơn — ít câu hỏi hơn?

```
Cung cấp đầy đủ trong 1 câu:
"Viết bài LinkedIn 500 từ về AI marketing cho CEO startup, 
tone chuyên gia storytelling, có data McKinsey, CTA comment"

→ Viet-Pro skip hỏi, viết thẳng
```

### Muốn viết content calendar cả tháng?

```
Nói: "Tạo content calendar tháng 3/2026 cho startup EdTech.
4 pillars, mỗi tuần 1 pillar → 5 platform posts"

→ Pipeline F: SocialWriter + Content Calendar template
→ Output: 4 pillars × 5 posts = 20 bài/tháng
```

### Viết truyện dài — giữ consistency?

```
Bước 1: /novel init → tạo world-bible
Bước 2: Mỗi chapter → Viet-Pro tự cập nhật story-state
Bước 3: WorldBuilder agent kiểm tra continuity tự động
→ Nhân vật, sức mạnh, mối quan hệ luôn nhất quán
```

### Dùng thành ngữ tự nhiên hơn?

```
Viet-Pro có thư viện 90+ thành ngữ theo 9 chủ đề.
Nói: "Thêm nhiều thành ngữ/tục ngữ VN hơn" → agent sẽ cấy thêm.
Hoặc: "Dùng giọng Nam bộ" → markers như "quá xá hay", "ấy mà"
```

---

## 📝 Output Format

Mọi bài viết đều đi kèm **bảng thông số** giúp bạn kiểm tra nhanh:

```
---
📊 Thông số
- Loại:         [Fiction/Article/Learning/Slide/Research/Social/Script]
- Độ dài:       X từ
- Framework:    [PAS/BAB/AIDA/Bloom's/IMRaD/...]
- Giọng văn:    [Emotional/Advanced/Technical/Academic]
- Anti-AI Score: X/10
- Platform:     [Facebook/LinkedIn/Blog/...]

💡 Gợi ý
- [CTA, hashtag, hình ảnh, cross-platform repurpose]
```

---

## 🗂️ Cấu trúc thư mục

```
Viet-Pro/
├── SKILL.md              ← Entry point, dispatch logic
├── README.md             ← Project overview
├── USERGUIDE.md          ← 📖 File này
├── CHANGELOG.md          ← Version history
│
├── modules/ (23 files)
│   ├── Core:      quality-punctuation, quality-natural, anti-ai-engine
│   ├── Style:     style-emotional, style-advanced, style-technical
│   ├── Platform:  platform-facebook → platform-instagram (8 files)
│   ├── Pipeline:  edu-writer, slide-writer, research-writer,
│   │              social-writer, script-writer
│   └── Support:   content-research, content-analysis,
│                  quality-factcheck, meta-upgrade
│
├── knowledge/ (21 files)
│   ├── Core:      anti-ai-humanization, emotional-writing-vn, ...
│   ├── Pipeline:  edu-pedagogy-bloom, academic-writing-vn, ...
│   ├── Genre:     8 genre files (tiên hiệp → kinh dị)
│   └── Reference: golden-samples-vn, vietnamese-idioms-db
│
├── novel-writer/          ← Pipeline A: Fiction Extension
│   ├── SKILL.md           ← 7+1 agent, 130đ QA
│   └── examples/
│
└── examples/
    └── test-prompts.md    ← Test prompts tất cả pipelines
```

---

*Viet-Pro v3.0 — Universal Vietnamese Content Studio*
*"Viết như người. Nghĩ như người. Chạm như người."*
