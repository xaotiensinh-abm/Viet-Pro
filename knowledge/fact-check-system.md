# R6: Fact-Check & Verification System — Knowledge Base

> **Module liên quan**: Q3 (Fact-check) — Tùy chọn, load khi có statistics/quotes/claims
> **Mục tiêu**: Xác minh mọi số liệu, trích dẫn, và tuyên bố trong bài viết

---

## 1. CRAAP Test Framework

Đánh giá độ tin cậy nguồn theo 5 tiêu chí:

| Tiêu chí | Câu hỏi | Score |
|----------|---------|-------|
| **C**urrency (Tính thời sự) | Nguồn publish khi nào? Còn cập nhật? | 1-5 |
| **R**elevance (Liên quan) | Nguồn có liên quan trực tiếp? | 1-5 |
| **A**uthority (Thẩm quyền) | Tác giả/tổ chức có uy tín? | 1-5 |
| **A**ccuracy (Chính xác) | Có bằng chứng, dữ liệu hỗ trợ? | 1-5 |
| **P**urpose (Mục đích) | Neutral hay có bias/quảng cáo? | 1-5 |

**Quy tắc**: Score < 15/25 → KHÔNG sử dụng nguồn

---

## 2. Citation Formats Cho Content VN

### 2.1 Inline Citation (Phổ biến nhất)
```
"Theo PwC (2025), 48% người tiêu dùng Việt Nam lo ngại về bất ổn kinh tế."
```

### 2.2 Numbered Citation (Cho blog/report)
```
"48% người tiêu dùng lo ngại bất ổn kinh tế [1]."

---
[1] PwC Vietnam. (2025). "Consumer Insights Survey". PwC Report.
```

### 2.3 Casual Citation (Social media)
```
"PwC vừa report: gần nửa người Việt lo về kinh tế. Nghe quen không?"
```

### 2.4 Quy Tắc Citation

| Loại content | Format | Bắt buộc? |
|-------------|--------|-----------|
| Report, whitepaper | Numbered [1] | ✅ Bắt buộc |
| Blog post | Inline hoặc hyperlink | ✅ Bắt buộc |
| Facebook post | Casual mention | 🟡 Khuyến khích |
| TikTok/Shorts | Verbal note | 🟡 Nếu claim lớn |
| Newsletter | Inline + footnote | ✅ Bắt buộc |

---

## 3. Fact-Check Workflow

### 3.1 Quy Trình 4 Bước

```
BƯỚC 1: PHÁT HIỆN CLAIMS
→ Scan bài viết, highlight mọi:
  - Số liệu (%, con số)
  - Quotes ("Ai đó nói...")
  - Tuyên bố mạnh ("X là tốt nhất", "luôn luôn", "không bao giờ")
  - So sánh ("hơn", "kém", "gấp X lần")

BƯỚC 2: XÁC MINH
→ Với mỗi claim:
  - Tìm primary source (nguồn gốc, không phải bài blog khác)
  - Cross-check với ít nhất 2 nguồn
  - Kiểm tra context: số liệu có bị cherry-pick không?

BƯỚC 3: GHI NGUỒN
→ Format citation theo platform (xem phần 2)
→ Nếu không tìm được nguồn → BỎ claim hoặc dùng hedging:
  "Một khảo sát gần đây gợi ý..." (thay vì "theo nghiên cứu...")

BƯỚC 4: VERIFY FINAL
→ Đọc lại toàn bộ: có claim nào chưa cite?
→ Kiểm tra link còn hoạt động không?
→ Số liệu có consistent trong toàn bài?
```

---

## 4. Common Misleading Patterns

| Pattern | Ví dụ | Cách fix |
|---------|-------|----------|
| **Cherry-picking** | Chọn 1 stat thuận lợi, bỏ qua ngược lại | Nêu cả 2 phía |
| **Correlation ≠ Causation** | "Đọc sách nhiều → giàu" | "Có mối liên hệ, chưa khẳng định nhân quả" |
| **Sample bias** | Survey 50 người → "Đa số người VN..." | Nêu rõ sample size |
| **Outdated data** | Dùng số liệu 2019 cho 2025 | Kiểm tra year, dùng data mới nhất |
| **Vague attribution** | "Theo nghiên cứu..." (nghiên cứu nào?) | Cite cụ thể: tên, năm, org |
| **Survivorship bias** | Chỉ kể success stories | Acknowledge failures |

---

## 5. Nguồn Tin Cậy Cho Content VN

### 5.1 Tier 1 (Rất tin cậy)
| Nguồn | Lĩnh vực |
|-------|---------|
| Tổng cục Thống kê (GSO) | Dân số, kinh tế VN |
| World Bank Vietnam | Kinh tế vĩ mô |
| PwC, McKinsey, BCG Vietnam | Business insights |
| Bộ GDĐT | Giáo dục |
| Nielsen Vietnam | Consumer behavior |

### 5.2 Tier 2 (Tin cậy với verification)
| Nguồn | Lĩnh vực |
|-------|---------|
| Brands Vietnam | Marketing trends |
| CafeF, VnExpress | Business news |
| Vietcetera | Culture, lifestyle |
| Statista | Global + VN stats |

### 5.3 Tier 3 (Cần cross-check)
| Nguồn | Lưu ý |
|-------|------|
| Blog cá nhân | Kiểm tra expertise |
| Social media posts | Verify claims |
| Wikipedia | Dùng làm starting point, cite primary source |
| AI-generated summaries | LUÔN verify |

---

## 6. Fact-Check Checklist

| # | Câu hỏi | Nếu "Không" |
|---|---------|------------|
| 1 | Mọi số liệu đều có nguồn? | Cite hoặc bỏ |
| 2 | Nguồn từ Tier 1-2? | Upgrade nguồn |
| 3 | Số liệu còn cập nhật (<2 năm)? | Tìm data mới |
| 4 | Quotes có attribution đầy đủ? | Thêm tên, chức vụ |
| 5 | Không có tuyên bố absolute? | Thêm nuance |
| 6 | Context đầy đủ (không cherry-pick)? | Thêm context |
| 7 | Link hoạt động? | Test links |

---

*Knowledge file: R6 Fact-Check & Verification System v1.0*
*Last updated: 2026-02-27*
