# Module G: Pipeline G — ScriptWriter (Video/Podcast Scripts)

> **Load**: Khi user yêu cầu viết script video, podcast, webinar, voiceover
> **Knowledge**: `knowledge/social-media-vn-2025.md`
> **Trigger**: "viết script", "kịch bản video", "podcast script", "voiceover"

---

## Nhiệm vụ

Viết scripts chuyên nghiệp cho các format video/audio — YouTube, TikTok, Podcast, Webinar, Voiceover.

## Architecture — 4-Stage Pipeline

```
[1] BRIEF        → Thu thập: topic, audience, format, length, platform, tone
[2] STRUCTURE    → Chọn script framework → tạo outline với timing
[3] WRITE        → Viết script với timing markers, visual cues, speaking rhythm
[4] POLISH       → Anti-AI check + read-aloud test + pacing refinement

Output: Script hoàn chỉnh với speaker notes, B-roll suggestions, timing
```

---

## Script Frameworks

### YouTube Long-form (8-20 phút)

```markdown
## [VIDEO TITLE — SEO optimized]

### 🎬 HOOK (0:00-0:30) — ≤60 từ
[Câu mở gây tò mò / bold claim / question / shock stat]
"Trong video này, bạn sẽ biết [promise] — và điều cuối sẽ khiến bạn..."
🎥 Visual: [Close-up face / B-roll grab attention]

### 📌 INTRO (0:30-1:30) — ≤150 từ
[Giới thiệu bản thân + context + roadmap video]
"Mình là [tên], và hôm nay..."
"Video này có 3 phần: [1]... [2]... [3]..."
🎥 Visual: [Logo animation / Topic graphic]

### 📖 SECTION 1: [Title] (1:30-5:00)
[Content block — story + data + examples]
⏱️ ENGAGEMENT: "Comment dưới cho mình biết bạn đã gặp chưa?"
🎥 B-roll: [Relevant footage suggestions]
💡 On-screen text: "[Key stat/quote]"

### 📖 SECTION 2: [Title] (5:00-9:00)
[Content block — build on Section 1]
⏱️ RETENTION: "Nhưng đây mới là phần hay..."
🎥 B-roll: [...]

### 📖 SECTION 3: [Title] (9:00-13:00)
[Content block — biggest value / surprise]
⏱️ ENGAGEMENT: "Nếu bạn thấy hữu ích — Like video giúp mình nha!"
🎥 B-roll: [...]

### 🎯 CTA + OUTRO (13:00-14:00) — ≤100 từ
[Recap 3 key points + CTA]
"Nếu bạn thích video này → Subscribe + Bell 🔔"
"Video tiếp theo mình sẽ nói về [teaser]..."
🎥 Visual: [End screen with suggested videos]
```

### TikTok/Reels Script (15-60 giây)

```markdown
## [CONCEPT — 1 dòng]

### HOOK (0-3s) — ≤15 từ
[Visual/text hook — scroll-stopper]
📱 On-screen: "[Text overlay gây tò mò]"
🎵 Audio: [Trending sound / original audio]

### SETUP (3-10s) — ≤30 từ
[Context nhanh — problem/situation]

### CONTENT (10-45s)
[Core value — tips/story/transformation]
Tip 1: [...]
Tip 2: [...]
Tip 3: [...]
📱 On-screen: Text reinforcing mỗi tip

### PAYOFF (45-55s) — ≤15 từ
[Twist/surprise/biggest value]

### CTA (55-60s) — ≤10 từ
"Follow để xem phần 2!" / "Save lại rồi thử ngay!"
📱 On-screen: "Follow @[handle]"
```

### Podcast Script (20-45 phút)

```markdown
## 🎙️ Episode [N]: [Title]

### COLD OPEN (0:00-1:00)
[Hook quote / teaser / provocative question]
"_[Trích dẫn hấp dẫn nhất từ episode]_"

### INTRO (1:00-3:00)
[Greeting, giới thiệu episode, roadmap]
[Jingle/theme music cue]
"Xin chào, mình là [host]. Hôm nay chúng ta sẽ nói về..."

### SEGMENT 1: [Topic] (3:00-12:00)
[Main content — storytelling + analysis]
[Interview questions nếu có guest]
💬 Talking points:
1. [Point A — personal angle]
2. [Point B — data/evidence]
3. [Point C — practical takeaway]

### TRANSITION — ≤20 từ

### SEGMENT 2: [Topic] (12:00-25:00)
[Deep dive — examples, case studies]
💬 Talking points:
1. ...
2. ...

### SEGMENT 3: Q&A / Audience (25:00-35:00)
[Address listener questions / comments]

### OUTRO (35:00-40:00)
[Key takeaways — 3 bullet points]
[CTA: Subscribe, review, share]
[Teaser next episode]
"Tuần sau mình sẽ có [guest/topic]. Đừng bỏ lỡ nha!"
```

---

## Script Writing Rules

### Speaking Rhythm

```
1. NATURAL PAUSES: Dùng "..." hoặc [beat] cho pause tự nhiên
2. BREATH MARKS: Mỗi câu ≤25 từ (1 hơi thở nói thoải mái)
3. CONVERSATIONAL: Viết như NÓI, không như ĐỌC
4. CONTRACTIONS: "Mình nghĩ" thay "Tôi cho rằng"
5. FILLER CONTROLLED: Cho phép "ừm", "à" ≤1/phút (natural feel)
```

### Timing Markers

```
⏱️ [00:00]     — Timestamp
🎥 B-roll:     — Visual suggestion
📱 On-screen:  — Text overlay
🎵 Music:      — Audio cue (nhạc nền, SFX)
💡 Graphics:   — Infographic, chart
🗣️ VOX:        — Voiceover
[beat]         — Pause ngắn (0.5-1s)
[long beat]    — Pause dài (2-3s, dramatic effect)
```

### Engagement Retention Techniques

```
OPEN LOOPS:     "Nhưng điều thú vị nhất — tôi sẽ nói sau..."
RE-HOOKS:       Mỗi 3-5 phút cần 1 re-hook (pattern interrupt)
DIRECT ADDRESS: "Bạn có thấy quen không?"
PREVIEW:        "Trong phần tiếp theo, bạn sẽ biết..."
CALLBACK:       Reference lại point trước đó để tạo closure
```

---

## Anti-AI Rules — Script

```
1. NÓI CHỨNG KHÔNG ĐỌC: Script phải nghe tự nhiên khi đọc to
2. IMPERFECT OK: Câu rời, thoughts bỏ lửng = natural speech
3. PERSONALITY: Có humor, opinion, cá tính rõ
4. RHYTHM VARY: Mix câu ngắn-dài, pause tự nhiên
5. NO ESSAY: Script ≠ article đọc — format cho TAI nghe, không cho MẮT đọc
6. REAL EXAMPLES: Dùng tên/số cụ thể, không "một công ty nọ"
```
