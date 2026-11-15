# Problem backlog — A028

Nguồn: reportT1.md và bản export `cvat-jobs-2026-11-13.csv`. Task 207 có tên `W1-SEG-G4-T1`; export xác nhận các job/frame range bên dưới. Các mã ảnh B/S được nối với frame/job tương ứng. Hướng xử lý P-001–P-008 được ghi tại [QĐ-001](so-quyet-dinh-a028.md#qđ-001).


| Job | Frame range | Assignee trong export | Link                                                    |
| --- | -----------: | --------------------- | ------------------------------------------------------- |
| 884 | 0–19        | 2A202603137           | [Mở Job 884](https://cvat.edufun.ai/tasks/207/jobs/884) |
| 885 | 20–39       | 2A202603028           | [Mở Job 885](https://cvat.edufun.ai/tasks/207/jobs/885) |
| 886 | 40–59       | 2A202603161           | [Mở Job 886](https://cvat.edufun.ai/tasks/207/jobs/886) |
| 887 | 60–79       | 2A202603168           | [Mở Job 887](https://cvat.edufun.ai/tasks/207/jobs/887) |
| 888 | 80–99       | 2A202603121           | [Mở Job 888](https://cvat.edufun.ai/tasks/207/jobs/888) |


## Danh sách


| Mã    | Tóm tắt                                            | Loại                   | Mục guideline | Trạng thái             | Kết quả      |
| ----- | -------------------------------------------------- | ---------------------- | ------------- | ---------------------- | ------------ |
| P-001 | Xe đi ngược chiều G04\_B067 có cần annotate?       | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Cần annotation |
| P-002 | Ranh giới phần đường G04\_B073 không rõ            | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Có hướng xử lý |
| P-003 | Phần đường có thể rẽ nhưng bị xe đỗ ở G04\_B074    | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Có hướng xử lý |
| P-004 | Boundary bị lóa đèn giao thông G04\_B004.jpg       | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Có hướng xử lý |
| P-005 | Building bị cây che và ảnh mờ G04\_S064, G04\_S067 | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Có hướng xử lý |
|       |                                                    |                        |               |                        |              |
| P-006 | Phân biệt Terrain/Vegetation tại G04\_S066         | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Có hướng xử lý |
| P-007 | Bê tông trắng nhỏ ở G04\_S069 có phải Sidewalk?    | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Có hướng xử lý |
| P-008 | Boundary Road khi đường phủ tuyết không rõ         | Guideline chưa nói tới | Chưa xác định | ✅ Đã chốt → QĐ-001 | Có hướng xử lý |


**Loại:** Guideline chưa nói tới · Guideline mơ hồ · Guideline mâu thuẫn · Pain point công cụ
**Trạng thái:** 🔴 Mở · 🗣️ Đang bàn · ↗️ Hỏi reviewer/mentor · ✅ Đã chốt (trỏ sang QĐ) · 🛠️ Làm tool · ⚪ Bỏ (ghi lý do)

## Chi tiết edge case

Các mục dưới đây ghi lại edge case và câu trả lời/hướng xử lý đã nhận được; xem [QĐ-001](so-quyet-dinh-a028.md#qđ-001). URL frame dùng số trong mã ảnh và job theo frame range hiển thị trên task page.

### P-001 — Xe đi ngược chiều G04_B067

Có cần annotate xe đi ngược chiều không? Đối chiếu phạm vi class trong BBox guideline. [Job 887, frame 67](https://cvat.edufun.ai/tasks/207/jobs/887?frame=67).

**Câu trả lời đã xác nhận:** Có, xe đi ngược chiều cần annotation.

### P-002 — Phần đường G04_B073

Phần đường đi được không rõ; báo cáo ghi hiện chưa annotate. Cần xác nhận bỏ qua hay vẽ theo phần nhận diện được. [Job 887, frame 73](https://cvat.edufun.ai/tasks/207/jobs/887?frame=73).

**Câu trả lời đã xác nhận:** Có thể tự nội suy theo phần nhận diện được.

### P-003 — Phần đường bị xe đỗ che G04_B074

Cần xác nhận chỉ annotate phần đường nhìn thấy hay có quy tắc khác cho phần bị che. [Job 887, frame 74](https://cvat.edufun.ai/tasks/207/jobs/887?frame=74).

**Câu trả lời đã xác nhận:** Chỉ cần tự nội suy và annotation phần nhìn thấy được.

### P-004 — Lóa đèn G04_B004.jpg

Ánh sáng  gây khó xác định boundary. Cần thống nhất cách vẽ theo phần quan sát được; không tự nội suy vùng không nhìn thấy. [Job 884, frame 4](https://cvat.edufun.ai/tasks/207/jobs/884?frame=4).

**Câu trả lời đã xác nhận:** Chỉ cần annotation phần nhìn thấy được.

### P-005 — Building bị che G04_S064, G04_S067

Nhà bị cây che, địa hình phức tạp, ảnh mờ. Cần xác nhận phạm vi mask Building và cách xử lý vùng khuất/mờ. [Job 887, frame 64](https://cvat.edufun.ai/tasks/207/jobs/887?frame=64) · [frame 67](https://cvat.edufun.ai/tasks/207/jobs/887?frame=67).

**Câu trả lời đã xác nhận:** Job 887, frame 64: có thể bỏ phần cầu. Frame 67: chỉ cần đánh dấu đầy đủ phần cây nhìn thấy được.

### P-006 — Terrain hay Vegetation G04_S066

Cần xác nhận cách phân loại cỏ và cây, cùng ranh giới giữa hai class. [Job 887, frame 66](https://cvat.edufun.ai/tasks/207/jobs/887?frame=66).

**Câu trả lời đã xác nhận:** Job 887, frame 66: không cần annotation phần tuyết. Terrain là phần thảm cỏ thấp màu xanh; Vegetation là cây cao màu xanh.

### P-007 — Sidewalk G04_S069

Vùng bê tông màu trắng nhỏ, chưa rõ có phải Sidewalk. Cần xác nhận tiêu chí nhận diện/ngưỡng áp dụng. [Job 887, frame 69](https://cvat.edufun.ai/tasks/207/jobs/887?frame=69).

**Câu trả lời đã xác nhận:** Job 887, frame 69: có thể xem đây là sidewalk. Tự nội suy theo hình ảnh nhìn thấy được.

### P-008 — Road phủ tuyết

Ranh giới Road với khu vực xung quanh khó thấy. Cần thống nhất cách xác định boundary khi tuyết che phủ.

**Câu trả lời đã xác nhận:** Không cần annotation cho vùng này nếu không có labels 