# Module D: SlideWriter — Pipeline Slide Bài Giảng

> **Load**: Khi user yêu cầu tạo slide, PowerPoint, presentation, bài thuyết trình, keynote
> **Knowledge**: `knowledge/presentation-design-vn.md`

---

## Nhiệm vụ

Dispatcher cho Pipeline D — tạo slide deck outline + speaker notes chuyên nghiệp theo narrative arc.

## SlideWriter 4-Stage Pipeline

```
[1] PRESENTATION PLANNER
    Input:  Chủ đề + audience + duration + key message
    Output: Presentation brief (audience profile, objectives, CTA)
    ↓
[2] STORYBOARD DESIGNER
    Input:  Brief từ Stage 1
    Output: Slide outline theo narrative arc
    Rules:  Chọn arc phù hợp (Standard / Workshop / Pitch / Lecture)
    ↓
[3] SLIDE CONTENT WRITER
    Input:  Storyboard structure
    Output: Content per slide (title + bullets + speaker notes)
    Rules:  Title ≤7 từ, ≤6 bullets, mỗi bullet ≤10 từ
    ↓
[4] VISUAL RECOMMENDER
    Input:  Slide content
    Output: Layout + chart type + image prompt + icon suggestions
    Rules:  Mỗi slide PHẢI có 1 visual element gợi ý
```

## Duration-to-Slides Mapping

| Thời lượng | Số slides | Pace |
|-----------|-----------|------|
| 5-min pitch | 5-8 slides | 1 slide/40s |
| 10-min talk | 8-12 slides | 1 slide/50s |
| 20-min talk | 15-20 slides | 1 slide/60s |
| 45-min lecture | 25-35 slides | 1 slide/90s |
| Workshop half-day | 15-20 content + 5-10 activity | Variable |

## Narrative Arcs

### Arc 1: Standard (Phổ biến nhất)

```
Slide 1-2:   HOOK — Tình huống/câu hỏi/số liệu gây shock
Slide 3-4:   PROBLEM — Đào sâu vấn đề, pain point
Slide 5-8:   SOLUTION — Framework/giải pháp, từng bước
Slide 9-10:  EVIDENCE — Case study, data, demo
Slide 11-12: ACTION — CTA, next steps, Q&A
```

### Arc 2: Pitch Deck (Startups, Fundraising)

```
Slide 1:  Title + Tagline
Slide 2:  Problem — pain point rõ ràng
Slide 3:  Solution — bạn giải quyết thế nào
Slide 4:  Market Size — TAM/SAM/SOM
Slide 5:  Product — demo/screenshot
Slide 6:  Business Model — cách kiếm tiền
Slide 7:  Traction — metrics, growth
Slide 8:  Team — founder profiles
Slide 9:  Financials — projection
Slide 10: Ask — vốn cần, kế hoạch dùng
```

### Arc 3: Workshop / Training

```
Phase 1 (10%): Hook + Agenda + Ground rules
Phase 2 (20%): Theory — concepts cần biết
Phase 3 (50%): Practice — activities, group work, exercises
Phase 4 (10%): Debrief — what did we learn
Phase 5 (10%): Next steps + Resources + Feedback
```

### Arc 4: Academic Lecture

```
Slide 1-2:   Review bài trước + Mục tiêu hôm nay
Slide 3-5:   Concept 1 — theory + ví dụ + practice
Slide 6-8:   Concept 2 — theory + ví dụ + practice
Slide 9-10:  Concept 3 (nếu có)
Slide 11-12: Summary + Assignment + Preview bài sau
```

## Slide Format Rules

### Mỗi Slide PHẢI Có

```
├── Title: ≤7 từ, action-oriented (KHÔNG mô tả passive)
│   ❌ "Kết quả khảo sát"
│   ✅ "Khảo sát cho thấy 73% muốn thay đổi"
│
├── Body: ≤6 bullets, mỗi bullet ≤10 từ
│   ❌ "Theo nghiên cứu của Harvard năm 2024, người tiêu dùng có xu hướng..."
│   ✅ "73% người tiêu dùng ưu tiên tốc độ"
│
├── Visual: 1 element gợi ý (chart/image/icon/diagram)
│   → Bar chart, pie chart, timeline, comparison, photo
│
└── Speaker Notes: 50-100 từ
    → Đây là phần NÓI — không đọc slide
    → Kể story, giải thích, add context
```

### Layout Types

| Layout | Khi nào dùng |
|--------|-------------|
| **Full-image** | Emotional moment, hook slide, quote |
| **Title + Bullets** | Information delivery, listicle |
| **Split (50/50)** | Before/After, comparison |
| **Big Number** | Data highlight, stat shock |
| **Quote** | Expert quote, testimonial |
| **Chart/Graph** | Data visualization |
| **Blank + 1 phrase** | Pause/emphasis moment |

## Output Format

```markdown
## Slide [N]: [Tiêu đề — ≤7 từ]

**Layout:** [Full-image / Title+Bullets / Split / Quote / Chart / Big Number]

### Content
- Bullet 1
- Bullet 2
- Bullet 3

### Visual
> [Gợi ý: line chart so sánh 2020 vs 2025 / ảnh minh họa X / icon Y]

### Speaker Notes
> [50-100 từ — nội dung cần NÓI, context, story, transition sang slide tiếp]

---
```

## SlideWriter Rules

```
1. LESS IS MORE: Mỗi slide = 1 ý duy nhất. Không nhồi.
2. TELL STORIES: Speaker notes = storytelling, slide = visual support
3. PROGRESSIVE REVEAL: Không dump info — build từ từ
4. VN EXAMPLES: Data/case study từ thị trường VN khi có thể
5. TRANSITIONS: Speaker notes phải có câu chuyển tiếp sang slide sau
6. NO WALL OF TEXT: Nếu >6 bullets → tách thành 2 slides
7. ANTI-AI: Speaker notes viết tự nhiên như đang nói — KHÔNG văn mẫu
```
