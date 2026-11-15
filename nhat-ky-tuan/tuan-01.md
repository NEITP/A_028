# Nhật ký tuần 01 — A028

**Lead tuần này:**
- **Lê Đức Lượng** (`2A202603137`) — Phụ trách Bounding Box
- **Đinh Quốc Tiến** (`2A202603028`) — Phụ trách Segmentation

**Dữ liệu / task CVAT:**
- **Bounding Box:** Ảnh giao thông đô thị — [Task 67](https://cvat.edufun.ai/tasks/67) *(Jobs 182–186)*
- **Segmentation:** Ảnh giao thông đô thị — [task 207](https://cvat.edufun.ai/tasks/207) *(Jobs 884–888)*

## Thành viên và phân công

| Thành viên | Mã học viên (User ID) | Vị trí | Phân công tuần này |
|---|---|---|---|
| Lê Đức Lượng  | `2A202603137` | **Lead (BBox)** · Reviewer · Annotator | Điều phối & tổng hợp BBox; **BBox:** Job 182, Review 185; **Seg:** Job 884, Review 885 |
| Đinh Quốc Tiến | `2A202603028` | **Lead (Seg)** · Reviewer · Annotator | Chốt edge case; **BBox:** Job 183, Review 186; **Seg:** Job 885, Review 886 |
| Phạm Văn Hùng | `2A202603161` | Reviewer · Annotator | **BBox:** Job 184, Review 182; **Seg:** Job 886, Review 887 |
| Nguyễn Đăng Khoa | `2A202603168` | Reviewer · Annotator | **BBox:** Job 185, Review 183; **Seg:** Job 887, Review 888 |
| Trịnh Xuân Toàn | `2A202603121` | Reviewer · Annotator | **BBox:** Job 186, Review 184; **Seg:** Job 888, Review 884 |


## Công việc

### 1. Phần Bounding Box — Jobs 182–186 (Lead: Lê Đức Lượng)

| #   | Nội dung công việc                   | Annotator        | Reviewer         | Hoàn thành | Ghi chú                                 |
| --- | ------------------------------------ | ---------------- | ---------------- | ---------- | --------------------------------------- |
| 1   | Job 182 — Gán nhãn Bounding Box      | LÊ ĐỨC LƯỢNG     | PHẠM VĂN HÙNG    | ✅ 100%    | Đã hoàn thành gán nhãn & qua review chéo |
| 2   | Job 183 — Gán nhãn Bounding Box      | ĐINH QUỐC TIẾN   | NGUYỄN ĐĂNG KHOA | ✅ 100%    | Đã hoàn thành gán nhãn & qua review chéo |
| 3   | Job 184 — Gán nhãn Bounding Box      | PHẠM VĂN HÙNG    | TRỊNH XUÂN TOÀN  | ✅ 100%    | Đã hoàn thành gán nhãn & qua review chéo |
| 4   | Job 185 — Gán nhãn Bounding Box      | NGUYỄN ĐĂNG KHOA | LÊ ĐỨC LƯỢNG     | ✅ 100%    | Đã hoàn thành gán nhãn & qua review chéo |
| 5   | Job 186 — Gán nhãn Bounding Box      | TRỊNH XUÂN TOÀN  | ĐINH QUỐC TIẾN   | ✅ 100%    | Đã hoàn thành gán nhãn & qua review chéo |

### 2. Phần Segmentation — Task 207 (Lead: Đinh Quốc Tiến)

| #   | Nội dung công việc          | Annotator        | Reviewer         | Hoàn thành | Ghi chú                     |
| --- | --------------------------- | ---------------- | ---------------- | ---------- | --------------------------- |
| 1   | Job 884 — 20 ảnh, cùng nhãn | LÊ ĐỨC LƯỢNG     | TRỊNH XUÂN TOÀN  | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 2   | Job 885 — 20 ảnh, cùng nhãn | ĐINH QUỐC TIẾN   | LÊ ĐỨC LƯỢNG     | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 3   | Job 886 — 20 ảnh, cùng nhãn | PHẠM VĂN HÙNG    | ĐINH QUỐC TIẾN   | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 4   | Job 887 — 20 ảnh, cùng nhãn | NGUYỄN ĐĂNG KHOA | PHẠM VĂN HÙNG    | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 5   | Job 888 — 20 ảnh, cùng nhãn | TRỊNH XUÂN TOÀN  | NGUYỄN ĐĂNG KHOA | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |


Mức hoàn thành: ✅ xong **và đã qua review** · 🟡 đang làm (ghi %) · ⛔ bị chặn (ghi lý do) · ⬜ chưa bắt đầu

## Tổng kết

- **Phần Bounding Box (Jobs 182–186):**
  - Đã hoàn thành: 5 / 5 jobs (100%)
  - Qua review chéo: 100% các job (182–186) đã hoàn tất gán nhãn và duyệt chéo theo phân công
- **Phần Segmentation (Jobs 884–888):**
  - Đã gán: 90 / 100 ảnh (90%)
  - Qua review lần đầu: 90% (trả lại 10 ảnh)
- **Edge case & Quyết định:**
  - Edge case mới: 8 mục (P-001–P-008), ghi tại [problem-backlog-a028.md](../problem-backlog-a028.md).
  - Quyết định mới: [sổ quyết định A028](../so-quyet-dinh-a028.md).

## Hướng xử lý edge case

- Các câu trả lời P-001–P-008 đã được ghi tại [QĐ-001 trong sổ quyết định A028](../so-quyet-dinh-a028.md#qđ-001), với từng trường hợp được mô tả trong [backlog](../problem-backlog-a028.md).
- Xe đi ngược chiều cần annotation. Các trường hợp khác áp dụng theo phần nhìn thấy/nhận diện được và hướng dẫn cụ thể về Building, cây, Terrain, Vegetation, Sidewalk và vùng không có label.
- Đường phủ tuyết không cần annotation nếu vùng đó không có label.

## Kế hoạch tuần 02

- Nghiệm thu toàn bộ phần Bounding Box (Jobs 182–186) đã hoàn thành 100%.
- Tiếp tục hoàn thiện annotation/review các job Segmentation 884–888 theo phân công.
- Rà soát mask AI lỗi tại Job 888 và ảnh thiếu nhãn tại Job 887.
- Áp dụng các hướng xử lý P-001–P-008 và cập nhật annotation tương ứng trong các job.
- Rà soát các frame liên quan và kiểm tra annotation đã theo QĐ-001.
