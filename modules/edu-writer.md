# Module C: EduWriter — Pipeline Tài Liệu Học Tập

> **Load**: Khi user yêu cầu soạn giáo trình, tài liệu học, bài giảng, lesson plan, quiz, handout, workbook
> **Knowledge**: `knowledge/edu-pedagogy-bloom.md`

---

## Nhiệm vụ

Dispatcher cho Pipeline C — tạo tài liệu học tập chuyên nghiệp theo chuẩn sư phạm, tích hợp Viet-Pro Engine.

## EduWriter 5-Stage Pipeline

```
[1] CURRICULUM ANALYZER
    Input:  Chủ đề + đối tượng + mục tiêu học tập
    Output: Learning objectives (SMART), target level, scope
    ↓
[2] STRUCTURE DESIGNER
    Input:  Objectives từ Stage 1
    Output: Bloom's Taxonomy mapping → Module/Lesson/Topic hierarchy
    Rules:  Mỗi lesson PHẢI cover ≥3 tầng Bloom
    ↓
[3] CONTENT WRITER (Viet-Pro Engine)
    Input:  Structure + writing style
    Output: Nội dung theo pedagogical patterns
    Rules:  Load V1/V2/V3 tùy tone + Anti-AI luôn active
    ↓
[4] ENGAGEMENT LAYER
    Input:  Draft content
    Output: Content + examples + exercises + quiz + mnemonics
    Rules:  Mỗi 500 từ ≥1 điểm tương tác
    ↓
[5] QUALITY CHECK
    Input:  Final draft
    Output: Verified document
    Check:  Accuracy, progression, accessibility, anti-AI score
```

## Learning Document Types & Templates

### 1. Giáo Trình (Textbook)

```markdown
# [Tên môn học/chủ đề]

## Thông tin chung
- **Đối tượng**: [Học sinh/Sinh viên/Chuyên gia]
- **Thời lượng**: [X giờ/X tuần]
- **Mục tiêu tổng quát**: [2-3 objectives]

---

## Chương [N]: [Tên chương]

### Mục tiêu chương
Sau chương này, người học có thể:
1. [Bloom L1-2: Nhớ/Hiểu] — ...
2. [Bloom L3: Vận dụng] — ...
3. [Bloom L4-5: Phân tích/Đánh giá] — ...

### [N.1] Tình huống mở đầu
[Case study VN / Câu chuyện thực tế → dẫn vào lý thuyết]

### [N.2] Nội dung chính
[Lý thuyết, chia theo sub-sections]
[Xen kẽ: ví dụ VN, bảng, sơ đồ]

### [N.3] Ví dụ minh họa
[2-3 ví dụ từ đơn giản → phức tạp]

### [N.4] Bài tập
#### Nhóm A: Hiểu & Nhớ
[Câu hỏi trắc nghiệm, điền khuyết]
#### Nhóm B: Vận dụng
[Bài tập tình huống]
#### Nhóm C: Phân tích & Sáng tạo
[Dự án nhỏ, debate, thiết kế]

### Tóm tắt chương
[Key takeaways dạng bullet]
[Mindmap/Diagram tóm tắt]
```

### 2. Handout (1-2 trang)

```markdown
# 📋 [Chủ đề] — Handout

## Key Points
1. [Điểm chính 1 — ≤2 câu]
2. [Điểm chính 2]
3. [Điểm chính 3]

## Visual Summary
[Bảng/Sơ đồ/Infographic gợi ý]

## Quick Practice
- Câu hỏi 1: ...
- Câu hỏi 2: ...

## Remember
> [1 câu đọng lại / mnemonic device]
```

### 3. Workbook (Bài tập)

```markdown
# 📝 Workbook: [Chủ đề]

## Hướng dẫn
[Cách sử dụng workbook, thời gian, tự chấm]

## Phần 1: Warm-up (Bloom L1-2)
[5-10 câu nhớ/hiểu]

## Phần 2: Practice (Bloom L3)
[3-5 bài vận dụng]

## Phần 3: Challenge (Bloom L4-6)
[1-2 bài phân tích/sáng tạo]

## Tự đánh giá
| Tiêu chí | ✅ Đạt | ⚠️ Cần cải thiện |
|----------|-------|-----------------|
| [Tiêu chí 1] | | |
| [Tiêu chí 2] | | |

## Đáp án & Giải thích
[Đáp án + WHY — quan trọng hơn đáp số]
```

### 4. Quiz / Test

```markdown
# 📊 Quiz: [Chủ đề] — [Thời gian: X phút]

## Phần I: Trắc nghiệm (X điểm)
1. [Câu hỏi] (Bloom L1-2)
   A. ...  B. ...  C. ...  D. ...

## Phần II: Đúng/Sai + Giải thích (X điểm)
1. [Phát biểu] → Đúng / Sai
   Giải thích: ___

## Phần III: Tự luận ngắn (X điểm)
1. [Câu hỏi vận dụng/phân tích]

## Rubric chấm điểm
| Mức | Mô tả | Điểm |
|-----|-------|------|
| Xuất sắc | [Tiêu chí] | 9-10 |
| Khá | [Tiêu chí] | 7-8 |
| Đạt | [Tiêu chí] | 5-6 |
| Chưa đạt | [Tiêu chí] | <5 |
```

### 5. Lesson Plan

```markdown
# 📅 Lesson Plan: [Chủ đề]

| Thông tin | Chi tiết |
|----------|---------|
| **Thời lượng** | X phút/giờ |
| **Đối tượng** | [Level + đặc điểm] |
| **Phòng/Setup** | [Online/Offline, thiết bị] |

## Mục tiêu bài học
SWBAT (Students Will Be Able To):
1. ...
2. ...
3. ...

## Tiến trình bài học

| Thời gian | Hoạt động | Phương pháp | Tài liệu |
|-----------|----------|------------|----------|
| 0-5' | Warm-up / Hook | [Game/Quiz/Video] | [Link/File] |
| 5-20' | Giới thiệu nội dung | [Lecture/Demo] | [Slide/Handout] |
| 20-35' | Thực hành | [Nhóm/Cá nhân] | [Workbook] |
| 35-45' | Wrap-up + Assessment | [Q&A/Exit ticket] | [Quiz] |

## Differentiation
- **Nâng cao**: [Activity cho học sinh giỏi]
- **Hỗ trợ**: [Scaffold cho học sinh yếu]

## Reflection (Sau buổi học)
- Điều gì hiệu quả?
- Điều gì cần cải thiện?
- Học sinh nào cần hỗ trợ thêm?
```

### 6. Case Study

```markdown
# 🔍 Case Study: [Tên tình huống]

## Bối cảnh
[Narrative: công ty/tổ chức VN, bối cảnh cụ thể]

## Vấn đề
[Dilemma/Challenge cần giải quyết]

## Dữ liệu
[Bảng số liệu, timeline, stakeholders]

## Câu hỏi thảo luận
1. [Phân tích: Nguyên nhân gốc là gì?]
2. [Đánh giá: Phương án nào tối ưu?]
3. [Sáng tạo: Bạn sẽ làm gì khác?]

## Hướng dẫn thảo luận (cho giảng viên)
[Key points, possible answers, debate angles]
```

## EduWriter Rules Bất Khả Xâm Phạm

```
1. CONCRETE FIRST: Luôn bắt đầu bằng ví dụ/tình huống → rồi mới lý thuyết
2. VN CONTEXT: Ví dụ PHẢI từ bối cảnh Việt Nam (DN VN, pháp luật VN, văn hóa VN)
3. ACTIVE LEARNING: Mỗi 500 từ phải có ≥1 điểm tương tác (câu hỏi/bài tập/reflection)
4. PROGRESSIVE: Từ đơn giản → phức tạp, KHÔNG nhảy cóc
5. VISUAL AIDS: Suggest table/diagram/flowchart ở MỌI khái niệm phức tạp
6. BLOOM COVERAGE: Mỗi lesson PHẢI cover ≥3 tầng Bloom's Taxonomy
7. ANTI-AI: Viet-Pro Engine LUÔN active — viết tài liệu cũng phải tự nhiên
```
