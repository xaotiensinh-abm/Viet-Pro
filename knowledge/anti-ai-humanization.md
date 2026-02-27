# R1: Anti-AI Humanization Engine — Knowledge Base

> **Module liên quan**: Q2 (Natural)
> **Mục tiêu**: Biến mọi output thành văn bản không thể bị AI detector nhận diện

---

## 1. Cách AI Detector Hoạt Động

### 1.1 Hai Metric Cốt Lõi

**Perplexity (Độ bất ngờ)**
- Đo mức độ *dễ đoán* của từng từ trong câu
- Perplexity THẤP = AI (vì AI chọn từ "an toàn", phổ biến nhất)
- Perplexity CAO = Con người (vì người viết sáng tạo, bất ngờ)
- GPTZero tính: overall text perplexity, average sentence perplexity, per-sentence perplexity

**Burstiness (Độ biến thiên)**
- Đo sự *dao động* về độ dài và phức tạp giữa các câu
- Burstiness THẤP = AI (câu đều đều, nhịp monotone)
- Burstiness CAO = Con người (xen kẽ câu ngắn-dài, đơn-phức)

### 1.2 Hệ Thống GPTZero (2025)
- 7 thành phần: Education Module, GPTZeroX, Shield, Internet Text Search, Deep Learning
- 99% accuracy với 1% false positive (pure AI vs pure human)
- 96.5% accuracy cho mixed documents
- Yếu khi text ngắn hoặc text formal/academic → dễ false positive

### 1.3 Các Detector Khác
| Detector | Đặc điểm |
|----------|----------|
| Originality.ai | Mạnh nhất cho SEO content, phân tích sâu |
| Turnitin | Chuẩn academic, khó bypass |
| Copyleaks | Đa ngôn ngữ, hỗ trợ tiếng Việt |
| Isgen | Chuyên biệt cho tiếng Việt |

---

## 2. Bảng 25 "AI Tells" — Dấu Hiệu Văn Bản AI

### 2.1 Cấu Trúc & Nhịp Điệu
| # | AI Tell | Ví dụ | Cách Fix |
|---|---------|-------|----------|
| 1 | Câu đều đều về độ dài | Mỗi câu 15-20 từ | Xen kẽ câu 5 từ & câu 30 từ |
| 2 | Cấu trúc câu lặp lại | Luôn Chủ-Vị-Bổ | Đảo ngữ, mở đầu bằng trạng ngữ |
| 3 | Paragraph length đồng đều | Mỗi đoạn 3-4 câu | Có đoạn 1 câu, có đoạn 7 câu |
| 4 | Mở đầu câu giống nhau | "Điều này...", "Việc..." | Thay đổi từ mở đầu liên tục |
| 5 | Kết luận dài, lặp ý | Tóm tắt lại hết nội dung | Kết ngắn, gợi mở, hoặc twist |

### 2.2 Từ Ngữ & Phong Cách
| # | AI Tell | Ví dụ (Tiếng Việt) | Cách Fix |
|---|---------|---------------------|----------|
| 6 | Từ ngữ trang trọng quá mức | "tối quan trọng", "vô cùng thiết yếu" | Dùng từ đời thường: "quan trọng lắm" |
| 7 | Lạm dụng từ nối | "Hơn nữa", "Ngoài ra", "Bên cạnh đó" | Bỏ bớt, dùng dấu chấm thay |
| 8 | Hedging phrases | "Cần phải lưu ý rằng...", "Nói chung..." | Nói thẳng, bỏ rào đón |
| 9 | Buzzwords AI | "đột phá", "tiên phong", "đổi mới sáng tạo" | Dùng từ cụ thể hơn |
| 10 | Từ vựng dễ đoán | Luôn chọn từ phổ biến nhất | Dùng từ ít phổ biến nhưng chính xác |
| 11 | Em dash lạm dụng | "Công nghệ — vốn là..." | Dùng ngoặc (), dấu chấm phẩy ; |

### 2.3 Nội Dung & Cảm Xúc
| # | AI Tell | Ví dụ | Cách Fix |
|---|---------|-------|----------|
| 12 | Thiếu trải nghiệm cá nhân | Chỉ có thông tin chung | Thêm "Tôi từng...", "Có lần..." |
| 13 | Ví dụ chung chung | "Ví dụ, công nghệ đang thay đổi" | Ví dụ cụ thể: tên, ngày, con số |
| 14 | Thiếu cảm xúc thật | Giọng trung tính, phẳng | Thêm surprise, frustration, humor |
| 15 | Thiếu humor | Nghiêm túc từ đầu đến cuối | Thêm pha hài, self-deprecating |
| 16 | Thiếu quan điểm cá nhân | Trình bày 2 mặt, không chọn bên | Nêu rõ: "Tôi nghĩ...", "Theo tôi..." |

### 2.4 Đặc Thù Tiếng Việt
| # | AI Tell | Ví dụ | Cách Fix |
|---|---------|-------|----------|
| 17 | Lặp từ không tự nhiên | "hỗ trợ... hỗ trợ... hỗ trợ" | Dùng đồng nghĩa: giúp, tạo điều kiện |
| 18 | Dài dòng hóa ý đơn giản | Giải thích 3 câu cho 1 concept | Nói gọn 1 câu |
| 19 | Tuyên bố chung chung | "Giáo dục là tương lai" | Cụ thể: AI tutoring giảm 40% cost |
| 20 | Thiếu thành ngữ/tục ngữ | Không có yếu tố văn hóa VN | Thêm: "đi một ngày đàng..." |
| 21 | Cú pháp hoàn hảo quá | Không lỗi chính tả, không cách nói ngẫu hứng | Cho phép imperfection tự nhiên |
| 22 | Giọng văn trang trọng đều | Formal từ đầu đến cuối | Xen kẽ formal và casual |
| 23 | Thiếu biểu cảm cá nhân | Không có dấu ấn riêng | Tạo "giọng" riêng: hóm hỉnh, sâu lắng |
| 24 | Mở rộng ngữ nghĩa dư thừa | Nói 1 ý bằng 5 cách | Nói 1 lần, đi tiếp |
| 25 | Nhịp điệu đồng đều | Thanh điệu không biến đổi | Tận dụng thanh trắc-bằng tiếng Việt |

---

## 3. Kỹ Thuật Tăng Burstiness (15+)

### 3.1 Sentence Length Variation
```
❌ AI style:
Công nghệ AI đang phát triển rất nhanh. Nhiều doanh nghiệp đã áp dụng AI. 
Điều này mang lại hiệu quả rõ rệt. Tuy nhiên cũng có nhiều thách thức.

✅ Human style:
AI đang bùng nổ.
Không phải kiểu "sẽ thay đổi thế giới trong 10 năm nữa" — mà là ngay bây giờ, 
ngay trong inbox email sáng nay của bạn. Tôi biết vì tuần trước, một email do AI 
viết suýt qua mặt cả team marketing 15 người. Chỉ một dấu phẩy lạ đã cứu họ.
```

### 3.2 Sentence Structure Mixing
| Kỹ thuật | Ví dụ |
|----------|-------|
| Câu 1 từ | "Thật." "Đúng." "Sai." |
| Câu hỏi tu từ | "Bạn có thấy điều gì lạ không?" |
| Câu bỏ lửng | "Nhưng rồi..." |
| Câu cảm thán | "Kinh! Không ngờ đúng thế!" |
| Câu đảo ngữ | "Lạ lùng thay, điều đó lại đúng." |
| Câu song hành | "Càng nhiều data, càng ít insight" |
| Câu liệt kê chèn | "Ba thứ: tiền, thời gian, và kiên nhẫn." |

### 3.3 Paragraph Rhythm Rules
- **Rule 1**: Không bao giờ 3 đoạn liên tiếp cùng độ dài
- **Rule 2**: Sau 1 đoạn dài (5+ câu), nên có đoạn siêu ngắn (1-2 câu)
- **Rule 3**: Đoạn mở đầu section nên bất ngờ (câu hỏi, quote, số liệu shock)
- **Rule 4**: Dùng "đoạn 1 câu" để tạo nhấn mạnh kịch tính

### 3.4 Vocabulary Diversification
```
❌ Lặp từ AI: "quan trọng... quan trọng... rất quan trọng"
✅ Đa dạng: "quan trọng... thiết yếu... then chốt... không thể bỏ qua"
   Thậm chí tốt hơn: "Bỏ cái này đi? Chắc chắn sập."
```

---

## 4. Kỹ Thuật Human Seed Draft

### 4.1 Nguyên Tắc
1. **Viết 2-3 câu đầu bằng tay** → thiết lập giọng, nhịp, personality
2. **Embed "dấu vân tay ngôn ngữ"**: cách dùng từ riêng, tic ngôn ngữ ("mà thôi", "nha", "ý tôi là")
3. **AI expand từ seed** → giữ giọng nhưng thêm nội dung
4. **Human review & inject** → thêm experience, humor, opinion

### 4.2 Quy Trình
```
[Human Seed] → [AI Expand] → [Human Inject Soul] → [AI Polish] → [Human Final Touch]
     20%           30%              25%                15%              10%
```

### 4.3 Ví Dụ Seed
```
Seed: "Hôm qua tôi ngồi debug 4 tiếng cho một cái lỗi mà cuối cùng hóa ra 
là thiếu dấu chấm phẩy. Bốn. Tiếng. Và tôi còn tự tin khoe với team là 
'để tôi fix nhanh nè'."

→ AI expand phần kỹ thuật, nhưng giữ giọng tự sự hài hước này
```

---

## 5. Checklist Tự Kiểm Tra Anti-AI

### Trước khi publish — chạy qua 10 câu hỏi này:

| # | Câu hỏi | Nếu "Không" → Fix |
|---|---------|-------------------|
| 1 | Có ít nhất 1 câu ≤5 từ trong mỗi 200 từ? | Thêm câu ngắn impact |
| 2 | Có variation ≥3 loại câu (hỏi, cảm thán, trần thuật)? | Thêm câu hỏi tu từ |
| 3 | Có ít nhất 1 trải nghiệm/anecdote cá nhân? | Thêm "Tôi từng..." |
| 4 | Có thành ngữ/tục ngữ hoặc slang VN? | Inject văn hóa VN |
| 5 | Đoạn paragraph có variation về độ dài? | Rebalance length |
| 6 | Có ít nhất 1 chỗ humor/wit? | Thêm pha hài nhẹ |
| 7 | Kết luận có khác biệt so với mở đầu? | Rewrite kết luận |
| 8 | Từ mở đầu câu có đa dạng? | Check & vary openers |
| 9 | Có quan điểm cá nhân rõ ràng? | Nêu opinion |
| 10 | Đọc to lên có nghe tự nhiên không? | Read aloud test |

---

## 6. Bảng Thay Thế Từ AI → Từ Người

| Từ/cụm AI hay dùng | Thay bằng |
|---------------------|-----------|
| "Điều cần lưu ý là" | (Bỏ luôn, nói thẳng) |
| "Hơn nữa" | "Còn nữa:", dấu chấm |
| "Tuy nhiên" | "Nhưng mà", "Nghe hay đấy, nhưng..." |
| "Rất quan trọng" | "Bỏ này là chết" |
| "Ngoài ra" | "À, thêm một cái..." |
| "Đáng chú ý" | "Cái này hay nè" |
| "Cần phải" | "Nên", "Phải" |
| "Có thể thấy rằng" | (Bỏ, nói thẳng nội dung) |
| "Nhìn chung" | "Gom lại thì..." |
| "Theo nghiên cứu" | "[Tên cụ thể] đã chỉ ra..." |
| "Đột phá" | "Thay đổi game", cụ thể cái gì thay đổi |
| "Tiên phong" | "Làm đầu tiên", nêu ai, khi nào |
| "Trong bối cảnh hiện nay" | (Bỏ, nói thẳng context) |

---

*Knowledge file: R1 Anti-AI Humanization Engine v1.0*
*Last updated: 2026-02-27*
