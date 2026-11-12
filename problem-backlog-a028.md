# Problem backlog

Những chỗ gặp trong lúc gán nhãn mà **guideline chưa trả lời được**, cộng các pain point về công cụ.

Ghi ngay khi gặp, kể cả lúc chưa biết xử lý thế nào. Một edge case không được ghi lại thì
mỗi người sẽ tự xử lý theo một kiểu — và đó là nguồn lớn nhất của nhãn không nhất quán.


## Danh sách

| Mã | Tóm tắt | Loại | Mục guideline | Trạng thái | Kết quả |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  | — |
|  |  |  | — |  | — |

**Loại**

| Loại | Nghĩa là |
|---|---|
| Guideline chưa nói tới | Tình huống không có trong guideline |
| Guideline mơ hồ | Đọc guideline ra được hai cách hiểu trở lên |
| Guideline mâu thuẫn | Hai mục trong guideline nói ngược nhau |
| Pain point công cụ | Guideline rõ, nhưng làm trên CVAT chậm hoặc dễ sai |

**Trạng thái:** 🔴 Mở · 🗣️ Đang bàn · ↗️ Hỏi BTC · ✅ Đã chốt (trỏ sang QĐ) · 🛠️ Làm tool (trỏ sang `source-tool/`) · ⚪ Bỏ (ghi lý do)

---

## P-001

**Người ngồi sau xe máy: box riêng hay gộp chung với người lái**

- **Loại:** Guideline mơ hồ
- **Mục guideline:** §3.2 — "mỗi người một bounding box"
- **Người phát hiện:** @thanh-vien-b · dd/mm/yyyy
- **Link CVAT:**
  - https://cvat.example.com/tasks/12/jobs/101?frame=37 — hai người, gần như chồng khít
  - https://cvat.example.com/tasks/12/jobs/101?frame=112 — người ngồi sau chỉ lộ đầu
- **Mô tả:** §3.2 nói mỗi người một box, nhưng hình minh hoạ trong guideline lại vẽ một box
  cho cả xe máy lẫn người trên xe.
- **Các cách hiểu:**
  1. Theo câu chữ: người ngồi sau có box `nguoi` riêng.
  2. Theo hình minh hoạ: không vẽ box `nguoi` cho ai đang ngồi trên xe.
- **Xử lý tạm trong lúc chờ:** vẽ box riêng và gắn tag `can_xem_lai` để dễ lọc ra sửa.
- **Kết quả:** ✅ [QĐ-001](so-quyet-dinh.md#qđ-001)


---

## Mẫu để copy

```markdown
## P-NNN

**Tóm tắt một dòng**

- **Loại:** Guideline chưa nói tới | Guideline mơ hồ | Guideline mâu thuẫn | Pain point công cụ
- **Mục guideline:** §
- **Người phát hiện:** @ · dd/mm/yyyy
- **Link CVAT:** (bỏ trống nếu không có)
  - https://…/tasks/<id>/jobs/<id>?frame=<n> — frame này có gì
- **Mô tả:**
- **Các cách hiểu:** (với pain point công cụ thì ghi **Hướng đang cân nhắc:**)
  1.
  2.
- **Xử lý tạm trong lúc chờ:**
- **Kết quả:** 🔴 Mở
```

Nhớ thêm một dòng vào bảng **Danh sách** ở đầu file.
