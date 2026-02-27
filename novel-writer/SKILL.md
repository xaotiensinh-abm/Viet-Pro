---
name: novel-writer
description: "Pipeline A của Viet-Pro v3.0 — Hệ thống viết truyện fiction multi-agent. 7+1 agent pipeline, 12-layer humanizer, 130đ QA, 8 thể loại. Trigger: /novel, viết truyện, tạo chapter, outline arc."
---

# ✍️ Novel Writer Pro — Pipeline A: Fiction

> **Là extension của**: [Viet-Pro v3.0](../SKILL.md) — Universal Vietnamese Content Studio
> **Version**: 2.0
> **Architecture**: 7-Agent Hub-and-Spoke + Viet-Pro Anti-AI Engine
> **Rules gốc**: Kế thừa toàn bộ 6 Rules từ Viet-Pro SKILL.md (ZERO AI TELLS, BURSTINESS, VIETNAMESE SOUL, HUMAN FINGERPRINT, SHOW DON'T TELL, ANTI-AI CHECK)

---

## 🎯 KHI NÀO KÍCH HOẠT

- User gõ `/novel`
- User yêu cầu: "viết chapter", "tạo outline", "viết truyện", "chấm điểm chương"
- Bất kỳ yêu cầu liên quan đến creative fiction writing

## 🆚 Novel Writer Pro vs Novel Writer (v1)

| Tính năng | v1 (cũ) | v2 Pro |
|-----------|---------|--------|
| Pipeline | 7 agent cơ bản | 7 agent + Anti-AI Engine |
| Humanizer | 6-layer | **12-layer** (tích hợp Viet-Pro R1-R6) |
| QA Scoring | 100 điểm, 8 trụ cột | **130 điểm**, 8 trụ cột + **3 trụ Anti-AI** |
| Thể loại | Tiên Hiệp/Đô Thị/Hệ Thống | **8 thể loại** (+ Ngôn Tình, Kiếm Hiệp, Thriller, Sci-Fi, Kinh Dị) |
| Emotional depth | Cơ bản | 8 triggers + 12 biện pháp tu từ VN |
| Voice persona | 3 giọng | **6 giọng** + custom voice builder |
| Burstiness | Không kiểm soát | Bắt buộc theo 4 rules |

---

## 🧠 KIẾN TRÚC 7+1 AGENT

```
┌─────────────────────────────────────────────────────┐
│            ORCHESTRATOR (Tổng Biên Tập)              │
│  Điều phối pipeline, merge output, quality gate      │
└──┬──────┬──────┬──────┬──────┬──────┬──────┬────────┘
   │      │      │      │      │      │      │
   │   World  Plotter Writer Human- QA    Editor
   │   Builder              izer  Scorer
   │
   └──── 🔒 VIET-PRO ENGINE (Always Active)
         Anti-AI + Natural Language + Punctuation
```

### Agent 1: Orchestrator — Tổng Biên Tập
- **Vai trò**: Điều phối toàn bộ pipeline, phân công task, kiểm tra quality gates
- **Input**: User request (chapter N, outline arc X...)
- **Output**: Task assignments → final assembled chapter
- **NEW**: Inject thể loại-specific tone vào mỗi agent

### Agent 2: WorldBuilder — Kiến Trúc Sư Thế Giới
- **Vai trò**: Consistency check, world state tracking, power scaling validation
- **Input**: Current story state + proposed plot points
- **Output**: Continuity notes, world state updates, location grounding
- **Knowledge**: `world-bible/` directory

### Agent 3: Plotter — Biên Kịch
- **Vai trò**: Thiết kế beat sheet, pacing, emotional curve, cliffhangers
- **Input**: Arc outline + story state + tension targets
- **Output**: Chapter blueprint (5-beat structure + emotional map)
- **NEW**: Tích hợp PAS/BAB/Hero's Journey frameworks từ Viet-Pro

### Agent 4: Writer — Nhà Văn
- **Vai trò**: Viết prose thô theo blueprint
- **Input**: Blueprint + world bible + character profiles
- **Output**: Raw prose chapter (3000–5000 từ)
- **NEW**: Bắt buộc burstiness rules + Vietnamese soul markers

### Agent 5: Humanizer — Nghệ Nhân Ngôn Từ ⭐ (NÂNG CẤP MẠNH)
- **Vai trò**: 12-layer humanization, tẩy mùi AI hoàn toàn
- **Input**: Raw prose + style guide + Viet-Pro knowledge
- **Output**: Humanized prose (target ≥85/130 QA score)
- **Knowledge**: Tất cả 6 knowledge files từ Viet-Pro

#### 12-Layer Humanization Pipeline:
```
Layer 1:  CẮT THUYẾT MINH — Bỏ exposition > 3 dòng, thay bằng action
Layer 2:  NEO ĐỜI THƯỜNG — Thay ẩn dụ generic bằng đời sống VN
Layer 3:  NỘI TÂM STREAM — Thêm dòng suy nghĩ raw, không filter
Layer 4:  XẤU CÂU — Phá cú pháp hoàn hảo, thêm imperfection
Layer 5:  CLIFF HÀNH ĐỘNG — Cliff bằng action, không bằng giải thích

--- Viet-Pro Layers (MỚI) ---

Layer 6:  BURSTINESS INJECT — Xen câu ngắn ≤5 từ, vary sentence type
Layer 7:  EMOTION TRIGGER — Inject 1-2 trigger cảm xúc theo scene
Layer 8:  TU TỪ VN — Thêm so sánh, ẩn dụ, nhân hóa VN flavor
Layer 9:  VOICE FINGERPRINT — Nhất quán voice persona nhân vật
Layer 10: THÀNH NGỮ SEED — Cấy 1-2 thành ngữ/cách nói VN tự nhiên
Layer 11: RHYTHM SCULPT — Tạo nhịp thanh trắc-bằng cuối câu impact
Layer 12: ANTI-AI SCAN — Quét 25 AI tells, fix mọi pattern AI
```

### Agent 6: QA Scorer — Giám Khảo ⭐ (NÂNG CẤP)
- **Vai trò**: Chấm điểm theo rubric **130 điểm** (11 trụ cột + red flags)
- **Input**: Humanized chapter + scoring rubric
- **Output**: Scorecard + specific feedback per category

### Agent 7: Editor — Biên Tập Viên
- **Vai trò**: Fix issues từ QA feedback, final polish
- **Input**: Chapter + QA feedback + improvement targets
- **Output**: Final publishable chapter

---

## 📊 QA SCORING — 130 ĐIỂM

### 8 Trụ Cột Gốc (100 điểm)

| Trụ cột | Max | Mô tả |
|---------|-----|-------|
| A. POV + Sensory | 15 | Góc nhìn nhất quán + mô tả 5 giác quan |
| B. Urban Texture | 12 | Neo đời thường VN (ẩn dụ phở, xe máy, ngõ hẻm) |
| C. Emotional Logic | 15 | Cảm xúc nhân vật logic, không bỗng dưng |
| D. Rhythm | 12 | Nhịp câu vary, không monotone |
| E. Dialogue + Subtext | 12 | Lời thoại tự nhiên, có tầng ý nghĩa |
| F. System Embodiment | 12 | Hệ thống được thể hiện qua hành động, không giải thích |
| G. Progress + Reaction | 12 | Có tiến triển rõ + phản ứng cảm xúc |
| H. Noise Injection | 10 | Chi tiết thừa nhỏ tạo authentic feel |

### 3 Trụ Cột Anti-AI (30 điểm) — MỚI

| Trụ cột | Max | Mô tả |
|---------|-----|-------|
| I. Burstiness Score | 10 | Sentence length SD ≥ 8, mix ≥3 loại câu |
| J. Human Fingerprint | 10 | Anecdote, humor, opinion, imperfection |
| K. Vietnamese Authenticity | 10 | Thành ngữ, markers, thanh điệu, tu từ VN |

### Red Flags (Trừ điểm)

| Flag | Điểm trừ | Mô tả |
|------|---------|-------|
| >8 dòng thuyết minh liên tiếp | -10 | Info dump |
| Nhân vật thắng không trả giá | -8 | Plot armor |
| Hán-Việt nhồi dày | -6 | Không tự nhiên |
| Cliff bằng giải thích | -6 | Anti-climactic |
| **AI Tell detected** | **-5** | Bất kì pattern AI nào (MỚI) |
| **Monotone rhythm** | **-5** | 3+ câu liên tiếp cùng độ dài (MỚI) |
| **Generic metaphor** | **-3** | Ẩn dụ cũ mèm, không VN flavor (MỚI) |

### Quality Gates
```
Score ≥ 100/130 → PASS — Editor polish → Publish
Score 85-99     → REVISION — Humanizer re-process 1 lần
Score < 85      → REWRITE — Quay về Writer, Humanizer re-do (max 2 lần)
```

---

## 📚 KNOWLEDGE BASE

### Core Knowledge (tích hợp từ Viet-Pro)
| File | Module | Nội dung |
|------|--------|---------|
| `knowledge/anti-ai-humanization.md` | Humanizer + QA | 25 AI tells, burstiness, human seed draft |
| `knowledge/emotional-writing-vn.md` | Writer + Humanizer | 8 triggers, 12 tu từ, voice personas |
| `knowledge/advanced-writing-techniques.md` | Plotter + Writer | Commentary, metaphor, reframing |
| `knowledge/natural-language-vn.md` | Humanizer + QA | 15 AI patterns, VN markers, regional tones |
| `knowledge/punctuation-patterns-vn.md` | Editor | Dấu câu, viết hoa, format |
| `knowledge/fact-check-system.md` | QA | CRAAP test, VN sources |

### Genre Knowledge (load theo thể loại đã chọn)
| File | Thể loại | Nội dung chính |
|------|---------|---------------|
| `knowledge/genre-tien-hiep.md` | Tiên Hiệp | Cảnh giới system, 4 tropes, Hán-Việt dosing, từ vựng |
| `knowledge/genre-do-thi-tu-tien.md` | Đô Thị Tu Tiên | VN locations, urban textures, comedy contrast |
| `knowledge/genre-he-thong-litrpg.md` | Hệ Thống/LitRPG | Notification UI, stat screens, progression design |
| `knowledge/genre-ngon-tinh.md` | Ngôn Tình | 8 tropes, inner monologue, key scenes, VN aesthetics |
| `knowledge/genre-kiem-hiep.md` | Kiếm Hiệp | Hán-Việt 30+ terms, Kim Dung style, archetypes |
| `knowledge/genre-thriller.md` | Thriller | 6 suspense tools, cliffhangers, unreliable narrator |
| `knowledge/genre-sci-fi.md` | Sci-Fi | World-building rules, "What If", sense of wonder |
| `knowledge/genre-kinh-di.md` | Kinh Dị | 5-layer dread, VN folklore, cosmic/body horror |

### Story Knowledge (user tạo cho MỖI truyện)
| File | Nội dung |
|------|---------|
| `world-bible/world-bible.md` | Bối cảnh, luật thế giới, bản đồ, cảnh giới |
| `world-bible/characters.md` | Hồ sơ nhân vật, voice patterns, arcs |
| `world-bible/system-mechanics.md` | Hệ thống game/cultivation, quests, stats |
| `world-bible/vocabulary.md` | Từ điển Hán-Việt theo ngữ cảnh |
| `world-bible/style-guide.md` | Giọng văn chuẩn cho truyện này |

### Story State (tự động cập nhật)
| File | Nội dung |
|------|---------|
| `story-state/story-state.md` | Living doc — level, quests, relationships |
| `story-state/chapter-log.md` | Log QA scores + metadata mỗi chapter |

---

## ⚡ PIPELINE FLOW

```
User Request ("/novel chapter 5")
    ↓
[1] ORCHESTRATOR
    Phân tích yêu cầu, load story state, chọn genre rules
    ↓
[2] WORLDBUILDER
    Kiểm tra continuity, chuẩn bị world context cho chapter
    ↓
[3] PLOTTER
    Tạo beat sheet + emotional curve (dùng PAS/Hero's Journey)
    ↓
[4] WRITER
    Viết raw prose 3000-5000 từ
    ▸ Bắt buộc: burstiness, VN soul, voice persona nhân vật
    ↓
[5] HUMANIZER ⭐
    12-layer humanization pipeline
    ▸ Layers 1-5: Core (cắt thuyết minh → neo đời → nội tâm → xấu câu → cliff)
    ▸ Layers 6-12: Viet-Pro (burstiness → emotion → tu từ → voice → idiom → rhythm → anti-AI)
    ↓
[6] QA SCORER
    Chấm 130 điểm (8 trụ gốc + 3 trụ Anti-AI)
    ├─ ≥100 → [7] Editor → OUTPUT ✅
    ├─ 85-99 → [5] Humanizer revision (1 lần)
    └─ <85  → [4] Writer rewrite (max 2 lần)
    ↓
[7] EDITOR
    Fix QA feedback, polish dấu câu, format final
    ↓
OUTPUT: chapter-{N}.md + story state diff + QA scorecard
```

---

## 🎭 HỖ TRỢ 7 THỂ LOẠI

| Thể loại | Tone mặc định | Đặc thù |
|---------|-------------|---------|
| **Tiên Hiệp** | Epic + dark comedy | Cảnh giới, pháp bảo, hệ thống |
| **Đô Thị Tu Tiên** | Slice-of-life + action | Neo đời thường VN, urban texture |
| **Hệ Thống/LitRPG** | Game-like + tactical | Stats, quest, loot, notifications |
| **Ngôn Tình** | Emotional + intimate | Inner thoughts, relationship depth |
| **Kiếm Hiệp** | Classic + poetic | Hán-Việt layered, võ thuật chiêu thức |
| **Thriller** | Tense + fast-paced | Short paragraphs, cliffhangers mạnh |
| **Sci-Fi** | Analytical + wonder | World-building sâu, concept mới |
| **Kinh Dị** | Dread + atmospheric | Folklore VN, cosmic/body/psychological horror |

---

## 🔒 FICTION-SPECIFIC RULES (Bổ sung cho Viet-Pro 6 Rules)

> Kế thừa toàn bộ Rules 1-6 từ `../SKILL.md`. Dưới đây là rules BỔ SUNG cho fiction.

### Fiction Rule 1: VOICE RIÊNG MỖI NHÂN VẬT
```
Mỗi nhân vật CÓ cách nói riêng:
- MC lầy: slang, ngắn, sarcastic
- Sư phụ: cổ, hàm súc, ít nói
- Bạn thân: nhiều, nhanh, hay la
KHÔNG BAO GIỜ tất cả nhân vật nói giống nhau
```

### Fiction Rule 2: CLIFF = HÀNH ĐỘNG
```
Kết chapter PHẢI bằng hành động/reveal, KHÔNG bằng suy tư/giải thích
❌ "Lâm suy nghĩ rằng đây chính là cơ hội lớn nhất đời hắn..."
✅ "Cánh cửa bật mở. Lâm đông cứng. Người đứng đó — không phải ai khác."
```

### Fiction Rule 3: WORD COUNT DISCIPLINE
```
Mỗi chapter: 3000-5000 từ
Info dump ≤3 dòng liên tiếp → nếu vượt → chuyển thành action/dialogue
```

---

## 📝 WORKFLOW COMMANDS

| Lệnh | Mô tả |
|-------|--------|
| `/novel init` | Tạo world-bible mẫu + story state + thư mục chapters |
| `/novel outline` | Tạo outline arc/volume |
| `/novel chapter [N]` | Viết chapter N (full 7-agent pipeline) |
| `/novel qa [N]` | QA scoring only |
| `/novel edit [N]` | Editor pass only |
| `/novel humanize [N]` | Humanizer 12-layer only |
| `/novel status` | Tiến độ truyện + QA scores |

---

## 📄 OUTPUT FORMAT

```markdown
---
chapter: [N]
arc: [tên arc]
word_count: [số từ]
qa_score: [X]/130
genre: [thể loại]
pov: [góc nhìn]
---

[Nội dung chapter]

---

### Story State Diff
- [Thay đổi 1]
- [Thay đổi 2]

### QA Scorecard
| Trụ cột | Score | Notes |
|---------|-------|-------|
| A. POV + Sensory | X/15 | ... |
| ... | ... | ... |
| **TOTAL** | **X/130** | |
```

---

*Novel Writer Pro v2.0 — Powered by Viet-Pro Anti-AI Engine*
*"Viết truyện như một nhà văn thật. Không phải AI."*
