# Module R1: Anti-AI Engine — Core Humanization

> **Load**: BẮT BUỘC mọi bài viết (tất cả pipelines A-G)
> **Knowledge**: `knowledge/anti-ai-humanization.md`

---

## Nhiệm vụ

Engine chống phát hiện AI — quét, sửa, và đảm bảo mọi output vượt qua AI detectors.

## 25 AI Tells — Bảng Quét

### Cấu trúc câu (Structural Tells)

| # | AI Tell | Ví dụ sai | Fix |
|---|---------|----------|-----|
| 1 | Mở đầu bằng "Trong bối cảnh..." | "Trong bối cảnh chuyển đổi số..." | Mở bằng ví dụ/câu hỏi/data cụ thể |
| 2 | "Hơn nữa" / "Ngoài ra" liên tiếp | "Hơn nữa, điều này... Ngoài ra..." | Bỏ connector, viết thẳng ý |
| 3 | "Đáng chú ý" / "Đáng lưu ý" | "Điều đáng chú ý là..." | "Cái hay ở đây là..." / "Nhưng khoan..." |
| 4 | Parallel structure quá hoàn hảo | 3 bullet cùng cấu trúc "X là Y" | Phá 1 bullet: ngắn hơn, khác cấu trúc |
| 5 | Mở đầu câu lặp lại | "Đầu tiên... Thứ hai... Thứ ba..." | Mix: dùng story, câu hỏi, dash |
| 6 | Câu cùng độ dài liên tiếp | 3+ câu ~20 từ liên tiếp | Xen câu ≤5 từ hoặc câu >30 từ |

### Từ vựng (Lexical Tells)

| # | AI Tell | Ví dụ sai | Fix |
|---|---------|----------|-----|
| 7 | "Vô cùng quan trọng" | "Việc này vô cùng quan trọng" | "Cái này quyết định sống chết" |
| 8 | "Tóm lại" / "Nhìn chung" mở kết | "Tóm lại, chúng ta thấy..." | Kết bằng action/question/twist |
| 9 | "Chúng ta" dùng quá nhiều | "Chúng ta cần... chúng ta nên..." | Mix: "Bạn", "Tôi", "Mọi người" |
| 10 | Từ Hán-Việt academic | "Thiết thực", "Bổ ích", "Đóng góp" | "Có ích thật", "Giúp được", "Làm ra" |
| 11 | "Giải pháp toàn diện" | "Đây là giải pháp toàn diện..." | "Đây là cách tôi nghĩ sẽ work" |
| 12 | "Không thể phủ nhận" | "Không thể phủ nhận rằng..." | Bỏ, viết thẳng claim |

### Giọng văn (Tonal Tells)

| # | AI Tell | Ví dụ sai | Fix |
|---|---------|----------|-----|
| 13 | Quá balanced, không có stance | "Có ưu điểm lẫn nhược điểm..." | Chọn phe, nói rõ opinion |
| 14 | Không có humor/wit | Toàn bộ serious, no surprise | Thêm 1 câu hài/unexpected |
| 15 | Không có anecdote | Toàn lý thuyết, không story | Thêm "Tôi từng..." / "Có lần..." |
| 16 | Emotional distance | Mô tả như observer, không feel | Dùng "tôi cảm thấy", chi tiết cảm giác |
| 17 | Perfect grammar | Không 1 chỗ imperfect | Thêm 1 câu rời, 1 thought fragment |
| 18 | Conclusion nhắc lại intro | Kết = paraphrase mở đầu | Kết bằng ý MỚI, twist, hoặc CTA |

### Format (Pattern Tells)

| # | AI Tell | Ví dụ sai | Fix |
|---|---------|----------|-----|
| 19 | List/bullet quá neat | 5 bullets cùng format | Phá 1-2: thêm comment, bỏ 1, merge |
| 20 | H2/H3 quá đều đặn | 5 sections cùng length | Vary: 1 dài, 1 ngắn, 1 medium |
| 21 | Transition quá smooth | "Tiếp theo, Cuối cùng, Tóm lại" | Bỏ transition, ý tự kết nối |
| 22 | Summary cuối mỗi section | "Như vậy, chúng ta đã..." | Bỏ summary, để ý chảy tự nhiên |
| 23 | Đầy đủ quá mức | Cover MỌI angle, không bỏ sót | Cố tình bỏ 1 góc → tạo personality |
| 24 | Dùng "ví dụ" trước mỗi ví dụ | "Ví dụ, công ty X..." | Nhảy thẳng vào: "FPT đã..." |
| 25 | Kết thúc bằng encouragement | "Hãy bắt đầu ngay hôm nay!" | Kết bằng question/challenge/twist |

---

## Human Seed Techniques

### Bảng kỹ thuật "Gieo Hạt Người"

| Kỹ thuật | Tần suất | Mô tả |
|----------|---------|-------|
| **Micro-anecdote** | 1-2/bài | "Chính tôi cũng từng...", "Tuần trước..." |
| **Imperfect thought** | 1/bài | Câu rời, bỏ lửng, ngoặc đơn comment |
| **Strong opinion** | 1-2/bài | "Tôi nghĩ cái này sai hoàn toàn." |
| **Self-correction** | 0-1/bài | "Nói vậy cũng không đúng hẳn." |
| **Rhetorical question** | 1-2/bài | "Nhưng thật sự — ai quan tâm?" |
| **Humor/wit** | 1/bài | Chơi chữ, irony nhẹ, self-deprecating |
| **Sensory detail** | 1-2/bài | "Cái cảm giác tay đặt lên keyboard lúc 2h sáng..." |
| **Vietnamese marker** | 2-3/bài | "nha", "mà", "ấy mà", "thôi rồi" |
| **Thành ngữ/tục ngữ** | 1/bài | Load từ `knowledge/vietnamese-idioms-db.md` |

---

## 10-Question Final Checkpoint

Trước khi giao bài, agent TỰ chạy:

```
 1. ✅ Có ít nhất 1 câu ≤5 từ?
 2. ✅ Có variation câu (hỏi, thán, kể, bỏ lửng)?
 3. ✅ Có anecdote/trải nghiệm cá nhân?
 4. ✅ Có thành ngữ/tục ngữ VN?
 5. ✅ Paragraph length có vary?
 6. ✅ Có humor/wit/surprise?
 7. ✅ Kết bài KHÁC cách mở bài?
 8. ✅ Từ mở đầu câu đa dạng (không lặp)?
 9. ✅ Có opinion/stance mạnh?
10. ✅ Đọc to nghe tự nhiên?

SCORING:
→ <7/10  → REWRITE toàn bộ, không patch
→ 7-8/10 → Fix chỗ yếu, re-check
→ 9-10/10 → DELIVER ✅
```

---

## Substitution Table — Thay AI Words

| ❌ AI Word/Phrase | ✅ Human Alternative |
|-------------------|---------------------|
| Trong bối cảnh hiện nay | [Bỏ, vào thẳng vấn đề] |
| Hơn nữa / Ngoài ra | [Bỏ connector, viết ý tiếp] |
| Đáng chú ý | "Cái hay là..." / "Nhưng đây mới là..." |
| Giải pháp toàn diện | "Cách mà tôi thấy work" |
| Vô cùng quan trọng | "Quyết định sống chết" / "Cực kỳ key" |
| Không thể phủ nhận | [Bỏ, viết thẳng claim] |
| Nhìn chung | [Bỏ, kết bằng ý mới] |
| Tóm lại | "Vậy nên..." / "Cuối ngày..." |
| Điều này cho thấy | "Nghĩa là..." / "Dịch ra =" |
| Chúng ta cần nhận thức | "Bạn biết cái gì funny không?" |

---

## Pipeline-Specific Anti-AI Flavors

```
Fiction (A):    Show don't tell, dialogue subtext, sensory overload
Article (B):    Personal voice, contrarian takes, real-world examples
Education (C):  Concrete first, humor in examples, imperfect explanations
Slide (D):      Speaker notes ≠ slide text, conversational notes
Research (E):   Academic hedging nhưng vẫn có perspective, vary sentence
Social (F):     Native platform voice, slang OK, imperfect grammar OK
Script (G):     Speaking rhythm, natural pauses, filler words controlled
```
