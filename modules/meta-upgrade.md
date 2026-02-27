# Module M1: Meta — Upgrade & Refinement

> **Load**: Khi user muốn nâng cấp bài viết hiện có
> **Lệnh kích hoạt**: "Nâng cấp bài này", "Viết lại cho tốt hơn", "Anti-AI hóa"

---

## Nhiệm vụ

Nhận bài viết có sẵn, phân tích điểm yếu, nâng cấp toàn diện.

## Upgrade Workflow

```
1. RECEIVE → Nhận bài gốc từ user
2. DIAGNOSE → Chạy 10-question anti-AI check
3. IDENTIFY → Liệt kê điểm yếu theo category
4. PRIORITIZE → Sắp xếp fixes theo impact
5. REWRITE → Viết lại TOÀN BỘ (không patch từng chỗ)
6. VERIFY → Re-check anti-AI score
7. COMPARE → Show before/after cho user
```

## Diagnosis Categories

| Category | Câu hỏi chẩn đoán | Fix module |
|----------|-------------------|-----------|
| AI-sound | Có patterns AI? Monotone? | Q2 Natural |
| Emotion | Có chạm cảm xúc không? | V1 Emotional |
| Structure | Có flow logic không? | N2 Analysis |
| Punctuation | Dấu câu đúng không? | Q1 Punctuation |
| Factual | Có claims chưa verify không? | Q3 Fact-check |
| Voice | Có personality riêng không? | V1 Voice Persona |
| Platform | Có phù hợp platform không? | H1 (hoặc tùy) |

## Before/After Template

```markdown
### 🔴 TRƯỚC (Score: X/10)
> [Đoạn gốc]
**Vấn đề**: [AI pattern cụ thể]

### 🟢 SAU (Score: Y/10)
> [Đoạn đã rewrite]
**Đã fix**: [Kỹ thuật áp dụng]
```

## Special: Anti-AI Conversion

Khi user gửi bài AI-generated muốn "người hóa":

```
1. Scan tất cả 25 AI Tells
2. Highlight từng tell trong bài
3. Rewrite TOÀN BỘ — bổ sung:
   - Personal anecdote (1-2 cái)
   - Vietnamese markers (2-3 cái)
   - Thành ngữ/tục ngữ (1-2 cái)
   - Sentence variety (burstiness)
   - Opinion mạnh (1-2 chỗ)
   - Humor (1 chỗ)
4. Final score ≥ 8/10 mới giao
```
