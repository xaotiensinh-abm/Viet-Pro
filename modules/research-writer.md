# Module E: ResearchWriter — Pipeline Tài Liệu Nghiên Cứu

> **Load**: Khi user yêu cầu viết luận, nghiên cứu, báo cáo phân tích, white paper, literature review, policy brief
> **Knowledge**: `knowledge/academic-writing-vn.md`

---

## Nhiệm vụ

Dispatcher cho Pipeline E — tạo tài liệu nghiên cứu/academic chất lượng cao, có citation, chuẩn học thuật nhưng vẫn readable.

## ResearchWriter 5-Stage Pipeline

```
[1] RESEARCH SCOPING
    Input:  Chủ đề + research question + scope
    Output: Research brief (question, methodology, boundaries, target journal/outlet)
    ↓
[2] LITERATURE REVIEW
    Input:  Research brief
    Tools:  Perplexity + Web search + User-provided sources
    Output: Source matrix (20-50 sources organized by theme)
    ↓
[3] ANALYSIS ENGINE
    Input:  Sources + data
    Output: Synthesized findings, gap analysis, argument structure
    Methods: Thematic analysis, comparative, SWOT, causal
    ↓
[4] WRITER (Academic Viet-Pro)
    Input:  Analysis + structure
    Output: Draft document theo chuẩn academic
    Rules:  Load V2 Advanced + Anti-AI (academic flavor)
    ↓
[5] CITATION CHECK
    Input:  Draft
    Output: Verified document + formatted references
    Check:  Source accuracy, citation format, logical consistency
```

## Research Document Types & Templates

### 1. Literature Review (2000-5000 từ)

```markdown
# [Tiêu đề: Tổng quan nghiên cứu về X]

## Tóm tắt (150-250 từ)
[Mục đích, phạm vi, phương pháp, kết quả chính, kết luận]

## 1. Giới thiệu
[Bối cảnh chủ đề]
[Tại sao review này cần thiết]
[Phạm vi và mục tiêu]
[Cấu trúc bài viết]

## 2. Phương pháp tổng quan
[Chiến lược tìm kiếm: databases, keywords, criteria]
[Tiêu chí chọn lọc: inclusion/exclusion]
[Số lượng nguồn: screened → selected → analyzed]

## 3. Chủ đề 1: [Theme từ literature]
[Tổng hợp findings từ 5-10 nguồn]
[So sánh & contrasts giữa các nghiên cứu]
[Đánh giá gaps/limitations]

## 4. Chủ đề 2: [Theme]
...

## 5. Chủ đề 3: [Theme]
...

## 6. Thảo luận
[Synthesis across themes]
[Research gaps identified]
[Implications cho thực tiễn VN]

## 7. Kết luận & Hướng nghiên cứu tương lai
[Key findings]
[Limitations of this review]
[Recommended future research]

## Tài liệu tham khảo
[Formatted citations — APA 7th / Harvard adapted VN]
```

### 2. White Paper (3000-6000 từ)

```markdown
# [Tiêu đề: Vấn đề + Giải pháp value proposition]

## Tóm tắt điều hành (300-500 từ)
[Key findings + recommendation — đọc riêng phần này đủ hiểu]

## 1. Vấn đề
[Pain point rõ ràng, data-backed]
[Impact: chi phí, rủi ro, cơ hội mất]

## 2. Bối cảnh & Xu hướng
[Industry landscape]
[VN market context]
[Global trends affecting VN]

## 3. Phân tích giải pháp
### 3.1 Phương án A
[Mô tả, ưu/nhược, evidence]
### 3.2 Phương án B
...
### 3.3 So sánh các phương án
[Comparison table/matrix]

## 4. Giải pháp đề xuất
[Detailed recommendation]
[Implementation roadmap]
[ROI projection]

## 5. Case Study
[1-2 case study thực tế — ưu tiên VN]

## 6. Kết luận & Khuyến nghị
[Action items cho decision makers]

## Phụ lục
[Data tables, methodology details, glossary]

## Tài liệu tham khảo
```

### 3. Policy Brief (1000-2000 từ)

```markdown
# [Tiêu đề: Vấn đề chính sách]

## Tóm tắt điều hành (100-200 từ)

## Bối cảnh vấn đề
[Tình hình hiện tại, data, stakeholders]

## Phân tích chính sách
### Phương án 1: [Tên]
- Ưu điểm: ...
- Nhược điểm: ...
- Chi phí ước tính: ...

### Phương án 2: [Tên]
...

## Khuyến nghị
[Phương án tối ưu + lý do]
[Implementation steps]
[Timeline]

## Tài liệu tham khảo
```

### 4. Case Analysis (2000-4000 từ)

```markdown
# [Tiêu đề: Phân tích tình huống X]

## Tóm tắt
## 1. Bối cảnh (Background)
## 2. Phương pháp nghiên cứu (Methodology)
## 3. Phát hiện (Findings)
## 4. Thảo luận (Discussion)
## 5. Hàm ý & Khuyến nghị (Implications)
## Tài liệu tham khảo
```

### 5. Báo Cáo Nghiên Cứu (3000-10000 từ)

```markdown
# [Tiêu đề báo cáo]

## Tóm tắt điều hành
## Mục lục
## 1. Giới thiệu
  1.1 Bối cảnh  |  1.2 Mục tiêu  |  1.3 Phạm vi  |  1.4 Phương pháp
## 2. Tổng quan tài liệu
## 3. Phương pháp nghiên cứu
## 4. Kết quả
## 5. Thảo luận
## 6. Kết luận & Khuyến nghị
## Tài liệu tham khảo
## Phụ lục
```

## Citation Formats

### APA 7th (Phổ biến nhất)

```
In-text: (Nguyễn, 2024) hoặc (Nguyễn & Trần, 2024)
Reference: Nguyễn, V. A. (2024). Tiêu đề bài báo. Tên Tạp Chí, 15(2), 45-67.

Multi-author: (Nguyễn et al., 2024) khi ≥3 tác giả
Website: Tên tổ chức. (2024, tháng 3, 15). Tiêu đề. URL
```

### Harvard (Adapted VN)

```
In-text: (Nguyễn 2024) hoặc (Nguyễn và Trần 2024)
Reference: Nguyễn, V.A., 2024. Tiêu đề bài báo. Tên Tạp Chí, 15(2), tr.45-67.
```

### Numbered [1] [2] [3] (Cho white paper, báo cáo)

```
In-text: Theo nghiên cứu gần đây [1], kết quả cho thấy... [2]
Reference:
[1] Nguyễn V.A. (2024). Tiêu đề...
[2] Trần B.C. (2023). Tiêu đề...
```

## Academic Writing Rules

```
1. CLAIM = EVIDENCE: Mọi claim phải có citation hoặc data hỗ trợ
2. BALANCED: Trình bày multiple perspectives trước khi đưa kết luận
3. PRECISE: Ngôn ngữ chính xác, không mơ hồ, không phóng đại
4. HEDGING: Dùng hedging language tự nhiên:
   ✅ "Kết quả cho thấy..." / "Có thể nhận định..."
   ❌ "Chắc chắn rằng..." / "Không thể phủ nhận..."
5. STRUCTURED: Heading hierarchy rõ ràng (H1→H2→H3)
6. VN CONTEXT: Ưu tiên sources và case studies Việt Nam
7. TRANSITIONS: Signal phrases giữa sections (Tuy nhiên, Mặt khác, Do đó)
8. ANTI-AI: Vẫn áp dụng burstiness + human fingerprint (academic flavor)
   — Vary câu, inject perspective cá nhân khi thảo luận
   — KHÔNG robot-style monotone
```

## Source Quality Tiers

```
Tier 1 (Ưu tiên): Peer-reviewed journals, official statistics (GSO, WB, IMF)
Tier 2 (Chấp nhận): Reputable reports (McKinsey, Deloitte), major news (VnExpress, Tuổi Trẻ)
Tier 3 (Bổ sung): Industry blogs, expert interviews, company reports
Tier 4 (Tránh): Wikipedia, random blogs, unverified social media
```
