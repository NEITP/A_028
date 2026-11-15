# Sổ quyết định — A028

Ghi lại các hướng xử lý được cung cấp cho các edge case trong backlog. P-001 đến P-008 đã có hướng xử lý được ghi trong QĐ-001.

## Danh sách

| Mã                | Quyết định                             | Ngày       | Xuất phát từ                           | Trạng thái |
| ----------------- | -------------------------------------- | ---------- | -------------------------------------- | ---------- |
| [QĐ-001](#qđ-001) | Hướng xử lý annotation cho P-001–P-008 | 2026-11-14 | [P-001–P-008](problem-backlog-a028.md) | Hiệu lực   |


## Tình trạng

P-001 đến P-008 đã có hướng xử lý ghi ở QĐ-001.

---

## QĐ-001

**Hướng xử lý annotation cho P-001–P-008**

- **Ngày:** 2026-11-14
- **Người tham gia:** Cả team
- **Xuất phát từ:** [P-001–P-008](problem-backlog-a028.md)
- **Bối cảnh:** Ghi lại các câu trả lời được cung cấp để áp dụng cho các trường hợp trong job 887 và các ảnh liên quan.
- **Các phương án đã cân nhắc:** Không áp dụng; ghi theo hướng xử lý đã cung cấp.
- **Quyết định:**
  - **P-001:** Có, xe đi ngược chiều cần annotation.
  - **P-002:** Có thể tự nội suy theo phần nhận diện được.
  - **P-003:** Chỉ cần tự nội suy và annotation phần nhìn thấy được.
  - **P-004:** Chỉ cần annotation phần nhìn thấy được.
  - **P-005:** Job 887, frame 64: có thể bỏ phần cầu. Frame 67: chỉ cần đánh dấu đầy đủ phần cây nhìn thấy được.
  - **P-006:** Job 887, frame 66: không cần annotation phần tuyết. *Terrain* là phần thảm cỏ thấp màu xanh; *Vegetation* là cây cao màu xanh.
  - **P-007:** Job 887, frame 69: có thể xem đây là *sidewalk*. Tự nội suy theo hình ảnh nhìn thấy được.
  - **P-008:** Không cần annotation cho vùng này nếu không có label.
- **Việc phải làm theo:**
  - [x] Áp dụng các hướng xử lý trên cho các frame tương ứng.

- **Trạng thái:** Hiệu lực