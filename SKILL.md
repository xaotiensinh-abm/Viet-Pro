---
name: Viet-Pro
description: "Universal Vietnamese Content Studio — 6 pipelines (Fiction, Article, Education, Presentation, Research, Social Media) + Anti-AI Engine + 20 modules. Auto-kích hoạt cho mọi tác vụ viết content tiếng Việt. Trigger: /viet-pro, /novel, /write, viết bài, viết truyện, tạo slide, soạn tài liệu."
---

# 🇻🇳 Viet-Pro — Universal Vietnamese Content Studio

> **Version**: 3.0
> **Architecture**: Adaptive Multi-Pipeline + Swarm Orchestrator (20 Modules)
> **Mục tiêu**: Viết MỌI loại content tiếng Việt mà **không ai** — kể cả AI detector — biết là AI viết

---

## 🎯 TỰ ĐỘNG KÍCH HOẠT KHI

| Trigger | Ví dụ |
|---------|-------|
| Viết truyện | "viết chapter", "viết truyện", "tạo outline" |
| Viết bài / content | "viết bài về...", "tạo bài đăng...", "viết content" |
| Tài liệu học tập | "soạn giáo trình", "tạo lesson plan", "viết bài giảng" |
| Slide / Presentation | "tạo slide", "soạn bài thuyết trình" |
| Nghiên cứu | "viết luận", "literature review", "white paper" |
| Social media | "đăng Facebook", "viết post LinkedIn", "caption TikTok" |
| Email | "viết email marketing", "soạn newsletter" |
| SEO / Blog | "viết bài SEO", "blog post" |
| Lệnh trực tiếp | `/viet-pro`, `/novel`, `/write` |

---

## 🧠 ADAPTIVE DISPATCH — PHÂN LOẠI TỰ ĐỘNG

### Bước 1: Content Type Router

```
User Request
    ↓
┌──────────────────────────────────────────────────────────┐
│                 CONTENT TYPE ROUTER                       │
│                                                          │
│  📖 FICTION        → Pipeline A: Novel Writer (7+1 agent) │
│  📝 ARTICLE/BLOG   → Pipeline B: Viet-Pro Swarm (11 mod) │
│  📚 LEARNING       → Pipeline C: EduWriter               │
│  🎤 PRESENTATION   → Pipeline D: SlideWriter             │
│  🔬 RESEARCH       → Pipeline E: ResearchWriter          │
│  📱 SOCIAL MEDIA   → Pipeline F: SocialWriter            │
│  🎬 VIDEO SCRIPT   → Pipeline G: ScriptWriter            │
│  📧 EMAIL          → Pipeline B + H4 Email Module        │
└──────────────────────────────────────────────────────────┘
```

### Bước 2: Thu thập thông tin (THÔNG MINH)

Hỏi user TỐI THIỂU — chỉ những gì chưa biết:

```
1. CHỦ ĐỀ: Viết về gì? (auto-detect từ request)
2. LOẠI CONTENT: Auto-detect → confirm nếu ambiguous
3. ĐỐI TƯỢNG: Gen Z / Millennials / Chuyên gia / Học sinh-SV / Đại chúng
4. PLATFORM/FORMAT: Facebook / LinkedIn / Blog / Slide / Word / PDF
5. GIỌNG VĂN: Thân thiện / Chuyên gia / Storytelling / Học thuật / Hóm hỉnh
6. ĐỘ DÀI: Ngắn / Vừa / Dài / Để tôi quyết định
```

### Bước 3: Load Module Stack

```
┌─────────────────┐
│  LUÔN LOAD (3)  │  Q1 Punctuation · Q2 Natural · R1 Anti-AI Engine
└────────┬────────┘
         ↓
┌────────────────────────────────────────────┐
│           DISPATCH THEO PIPELINE           │
│                                            │
│  Pipeline A  → novel-writer/SKILL.md       │
│  Pipeline B  → V1/V2/V3 + H1-H8 + N1/N2  │
│  Pipeline C  → C: EduWriter module         │
│  Pipeline D  → D: SlideWriter module       │
│  Pipeline E  → E: ResearchWriter module    │
│  Pipeline F  → F: SocialWriter router      │
│  Pipeline G  → G: ScriptWriter module      │
│                                            │
│  OPTIONAL ADDITIONS:                       │
│  Có số liệu/claim → Q3 Fact-check         │
│  Cần research      → N1 Research           │
│  Long-form         → N2 Analysis           │
│  Nâng cấp bài cũ   → M1 Meta-Upgrade      │
└────────────────────────────────────────────┘
```

---

## 📦 MODULE REGISTRY — 23 Modules

### Core (LUÔN LOAD)

| Module | File | Knowledge |
|--------|------|-----------|
| **Q1** | `modules/quality-punctuation.md` | `knowledge/punctuation-patterns-vn.md` |
| **Q2** | `modules/quality-natural.md` | `knowledge/natural-language-vn.md` + `knowledge/anti-ai-humanization.md` |
| **R1** | `modules/anti-ai-engine.md` | `knowledge/anti-ai-humanization.md` |

### Style (Load theo giọng văn)

| Module | File | Knowledge |
|--------|------|-----------|
| **V1** | `modules/style-emotional.md` | `knowledge/emotional-writing-vn.md` |
| **V2** | `modules/style-advanced.md` | `knowledge/advanced-writing-techniques.md` |
| **V3** | `modules/style-technical.md` | — |

### Platform (Load theo target)

| Module | File | Knowledge |
|--------|------|-----------|
| **H1** | `modules/platform-facebook.md` | `knowledge/emotional-writing-vn.md` |
| **H2** | `modules/platform-linkedin.md` | `knowledge/social-media-vn-2025.md` |
| **H3** | `modules/platform-tiktok.md` | `knowledge/social-media-vn-2025.md` |
| **H4** | `modules/platform-email.md` | `knowledge/social-media-vn-2025.md` |
| **H5** | `modules/platform-twitter.md` | `knowledge/social-media-vn-2025.md` |
| **H6** | `modules/platform-blog-seo.md` | `knowledge/advanced-writing-techniques.md` |
| **H7** | `modules/platform-zalo.md` | `knowledge/social-media-vn-2025.md` |
| **H8** | `modules/platform-instagram.md` | `knowledge/social-media-vn-2025.md` |

### Pipeline Dispatchers

| Module | File | Knowledge |
|--------|------|-----------|
| **C** | `modules/edu-writer.md` | `knowledge/edu-pedagogy-bloom.md` |
| **D** | `modules/slide-writer.md` | `knowledge/presentation-design-vn.md` |
| **E** | `modules/research-writer.md` | `knowledge/academic-writing-vn.md` |
| **F** | `modules/social-writer.md` | `knowledge/cross-platform-repurpose.md` |
| **G** | `modules/script-writer.md` | `knowledge/social-media-vn-2025.md` |

### Support

| Module | File | Knowledge |
|--------|------|-----------|
| **N1** | `modules/content-research.md` | — |
| **N2** | `modules/content-analysis.md` | — |
| **Q3** | `modules/quality-factcheck.md` | `knowledge/fact-check-system.md` |
| **M1** | `modules/meta-upgrade.md` | — |

---

## 📚 KNOWLEDGE BASE — 21 Files

### Core (Luôn sẵn sàng)
| File | Nội dung |
|------|---------|
| `knowledge/anti-ai-humanization.md` | 25 AI tells, burstiness, human seed |
| `knowledge/emotional-writing-vn.md` | 8 triggers, 12 tu từ, voice personas |
| `knowledge/advanced-writing-techniques.md` | Commentary, metaphor, reframing |
| `knowledge/natural-language-vn.md` | 15 AI patterns, VN markers |
| `knowledge/punctuation-patterns-vn.md` | Dấu câu chuẩn NĐ 30/2020 |
| `knowledge/fact-check-system.md` | CRAAP test, source tiers VN |
| `knowledge/vietnamese-idioms-db.md` | 500+ thành ngữ theo chủ đề |
| `knowledge/golden-samples-vn.md` | Bài mẫu hay phân tích |

### Pipeline-Specific
| File | Pipeline |
|------|---------|
| `knowledge/edu-pedagogy-bloom.md` | C: EduWriter |
| `knowledge/presentation-design-vn.md` | D: SlideWriter |
| `knowledge/academic-writing-vn.md` | E: ResearchWriter |
| `knowledge/social-media-vn-2025.md` | B + F: Social |
| `knowledge/cross-platform-repurpose.md` | F: SocialWriter |

### Genre (Fiction — Pipeline A)
8 files: `genre-tien-hiep.md` ... `genre-kinh-di.md`

> **Knowledge Resolution Order:**
> 1. Workspace: `.agent/skills/novel-writer/knowledge/`
> 2. Global Skill: `D:\AntigravityWorkspace\Skill\Viet-Pro\knowledge/`
> 3. Global Skill Modules: `D:\AntigravityWorkspace\Skill\Viet-Pro\modules/`

---

## 🔒 QUY TẮC TUYỆT ĐỐI (MỌI Pipeline)

### Rule 1: ZERO AI TELLS
```
Humanizer/R1 PHẢI quét 25 AI tells. Phát hiện → fix NGAY.
❌ "Trong bối cảnh hiện nay..." | "Hơn nữa..." | "Điều đáng chú ý..."
✅ Viết như ĐANG NÓI CHUYỆN với người thông minh
```

### Rule 2: BURSTINESS BẮT BUỘC
```
- Ít nhất 1 câu ≤5 từ mỗi 200 từ
- Ít nhất 3 loại câu (hỏi, thán, kể, bỏ lửng)
- Paragraph length KHÔNG đồng đều
- Từ mở đầu câu KHÔNG lặp lại
```

### Rule 3: VIETNAMESE SOUL
```
MỌI bài viết PHẢI có:
- Ít nhất 1 thành ngữ/tục ngữ/cách nói VN
- Ít nhất 1 ví dụ cụ thể (tên, ngày, con số thật)
- Dấu câu CHUẨN tiếng Việt (NĐ 30/2020)
```

### Rule 4: HUMAN FINGERPRINT
```
MỌI bài viết PHẢI có:
- Ít nhất 1 anecdote/trải nghiệm
- Quan điểm cá nhân rõ ràng
- Chi tiết cảm xúc cụ thể
- Ít nhất 1 chỗ humor/wit/surprise
```

### Rule 5: SHOW DON'T TELL (Fiction)
```
❌ "Lâm cảm thấy tức giận."
✅ "Hàm Lâm nghiến lại. Mắt hắn đỏ. Móng tay cắm vào lòng bàn tay."
```

### Rule 6: ANTI-AI FINAL CHECK
```
TRƯỚC KHI giao bài, tự chạy 10 câu hỏi:
1. Câu ≤5 từ? 2. Variation câu? 3. Anecdote? 4. Thành ngữ VN?
5. Paragraph vary? 6. Humor? 7. Kết≠Mở? 8. Opener vary?
9. Opinion mạnh? 10. Đọc to tự nhiên?
→ <7/10 → REWRITE | ≥7/10 → Deliver
```

---

## 📝 OUTPUT FORMAT CHUNG

```markdown
## 📝 [Tiêu đề]

[Nội dung]

---

### 📊 Thông số
- **Loại**: [Fiction/Article/Learning/Slide/Research/Social/Script]
- **Độ dài**: X từ
- **Framework**: [PAS/BAB/AIDA/Bloom's/Academic/...]
- **Giọng văn**: [Emotional/Advanced/Technical/Academic]
- **Anti-AI Score**: X/10
- **Platform**: [Facebook/LinkedIn/Blog/Slide/...]

### 💡 Gợi ý
- [CTA, hashtag, hình ảnh, cross-platform repurpose]
```

---

## 🔄 RECURSIVE IMPROVEMENT

Nếu user feedback "chưa tự nhiên" hoặc "giống AI":
1. Load R1 Anti-AI Engine + Q2 Natural
2. Identify cụ thể chỗ nào bị AI-sound
3. Apply fix từ bảng 25 AI Tells
4. Rewrite TOÀN BỘ (không patch)
5. Re-check 10 câu hỏi
6. Giao lại

---

*Viet-Pro v3.0 — Universal Vietnamese Content Studio*
*"Viết như người. Nghĩ như người. Chạm như người."*
