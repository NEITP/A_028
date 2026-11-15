# Nhật ký tuần 01 — A028

**Lead tuần này:** Đinh Quốc Tiến
**Dữ liệu / task CVAT:** Ảnh giao thông đô thị — [task 207](https://cvat.edufun.ai/tasks/207)

## Thành viên và phân công

| Thành viên | Vị trí | Phân công tuần này |
|---|---|---|
| Đinh Quốc Tiến | Lead · Reviewer · Annotator | Chốt edge case, Job 885, Review 886  |
| Nguyễn Đăng Khoa | Reviewer · Annotator | Job 887, Review 888 |
| Trịnh Xuân Toàn | Reviewer · Annotator | Job 888, Review 884 |
| Phạm Văn Hùng | Reviewer · Annotator | Job 886, Review 887 |
| Lê Đức Lượng | Reviewer · Annotator | Job 884, Review 885 |


## Công việc

| #   | Nội dung công việc          | Annotator        | Reviewer         | Hoàn thành | Ghi chú                     |
| --- | --------------------------- | ---------------- | ---------------- | ---------- | --------------------------- |
| 1   | Job 884 — 20 ảnh, cùng nhãn | LÊ ĐỨC LƯỢNG     | TRỊNH XUÂN TOÀN  | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 2   | Job 885 — 20 ảnh, cùng nhãn | ĐINH QUỐC TIẾN   | LÊ ĐỨC LƯỢNG     | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 3   | Job 886 — 20 ảnh, cùng nhãn | PHẠM VĂN HÙNG    | ĐINH QUỐC TIẾN   | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 4   | Job 887 — 20 ảnh, cùng nhãn | NGUYỄN ĐĂNG KHOA | PHẠM VĂN HÙNG    | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |
| 5   | Job 888 — 20 ảnh, cùng nhãn | TRỊNH XUÂN TOÀN  | NGUYỄN ĐĂNG KHOA | 🟡 90%     | Một số ảnh chưa gán nhãn đủ |


Mức hoàn thành: ✅ xong **và đã qua review** · 🟡 đang làm (ghi %) · ⛔ bị chặn (ghi lý do) · ⬜ chưa bắt đầu

## Tổng kết

- Đã gán: 90 / 100 ảnh (90%)
- Qua review lần đầu: 90% (trả lại 10 ảnh)
- Edge case mới: 8 mục (P-001–P-008), ghi tại [problem-backlog-a028.md](../problem-backlog-a028.md).
- Quyết định mới: [sổ quyết định A028](../so-quyet-dinh-a028.md).

## Hướng xử lý edge case

- Các câu trả lời P-001–P-008 đã được ghi tại [QĐ-001 trong sổ quyết định A028](../so-quyet-dinh-a028.md#qđ-001), với từng trường hợp được mô tả trong [backlog](../problem-backlog-a028.md).
- Xe đi ngược chiều cần annotation. Các trường hợp khác áp dụng theo phần nhìn thấy/nhận diện được và hướng dẫn cụ thể về Building, cây, Terrain, Vegetation, Sidewalk và vùng không có label.
- Đường phủ tuyết không cần annotation nếu vùng đó không có label.
## Kế hoạch tuần 02

- Tiếp tục annotation/review các job 884–888 theo phân công.
- Rà soát mask AI lỗi tại Job 888 và ảnh thiếu nhãn tại Job 887.
- Áp dụng các hướng xử lý P-001–P-008 và cập nhật annotation tương ứng trong các job.
- Rà soát các frame liên quan và kiểm tra annotation đã theo QĐ-001.
