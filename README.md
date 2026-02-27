# 🇻🇳 Viet-Pro — Universal Vietnamese Content Studio

> Skill viết content tiếng Việt chuẩn con người — vượt qua AI detector, chạm cảm xúc, tạo dấu ấn riêng.

📖 **[User Guide đầy đủ → USERGUIDE.md](USERGUIDE.md)**

## Quick Start

```
/viet-pro     → Viết content tiếng Việt (any type)
/novel        → Viết truyện fiction (7+1 agent pipeline)
/write        → Auto-detect content type
```

## Architecture

```
Viet-Pro v3.0 — Universal Vietnamese Content Studio
├── SKILL.md              ← Main entry point, dispatch logic
├── modules/ (23 files)   ← Module stack
│   ├── Core:     Q1 Punctuation, Q2 Natural, R1 Anti-AI Engine
│   ├── Style:    V1 Emotional, V2 Advanced, V3 Technical
│   ├── Platform: H1-H8 (Facebook → Instagram)
│   ├── Pipeline: C EduWriter, D SlideWriter, E ResearchWriter
│   │             F SocialWriter, G ScriptWriter
│   ├── Support:  N1 Research, N2 Analysis, Q3 Factcheck, M1 Upgrade
│   └── anti-ai-engine.md ← R1: 25 AI Tells + Human Seed
├── knowledge/ (21 files) ← Knowledge base
│   ├── Core:     anti-ai-humanization, emotional-writing-vn, natural-language-vn, ...
│   ├── Pipeline: edu-pedagogy-bloom, presentation-design-vn, academic-writing-vn, ...
│   ├── Genre:    8 genre files (fiction: tiên hiệp → kinh dị)
│   └── Ref:      golden-samples-vn, vietnamese-idioms-db
├── novel-writer/         ← Pipeline A: Fiction Extension
│   ├── SKILL.md          ← 7+1 agent, 130đ QA, 8 thể loại
│   └── examples/
├── examples/
│   └── test-prompts.md   ← Test prompts for all pipelines
└── README.md             ← This file
```

## 7 Pipelines

| Pipeline | Trigger | Module | Mô tả |
|----------|---------|--------|-------|
| **A** | /novel, viết truyện | novel-writer/SKILL.md | Fiction: 7+1 agent, 8 thể loại |
| **B** | viết bài, content | V1/V2/V3 + H1-H8 | Article, Blog, Email, Newsletter |
| **C** | tài liệu học tập | edu-writer.md | Lesson plan, giáo trình, quiz |
| **D** | tạo slide | slide-writer.md | Presentation, speaker notes |
| **E** | nghiên cứu, luận | research-writer.md | Literature review, white paper |
| **F** | social media | social-writer.md | Multi-platform: 1 pillar → N posts |
| **G** | script video | script-writer.md | YouTube, TikTok, Podcast scripts |

## Version History

See [CHANGELOG.md](CHANGELOG.md)
