# Bài 3: xây dựng không gian cộng tác doanh nghiệp
## Phần 1: Sơ đồ kiến trúc kênh

| Channel | Nội dung | Quy định |
|---|---|---|
| `#thong-bao` | Deadline, quyết định chung, lịch họp | Chỉ trưởng nhóm đăng; thành viên reply trong thread |
| `#ky-thuat-cam-bien` | Thảo luận kỹ thuật về cảm biến, lỗi, kiến trúc | Chỉ nội dung kỹ thuật; mỗi vấn đề một thread |
| `#tien-do-task` | Cập nhật tiến độ, giao việc, deadline | Mỗi việc ghi rõ người phụ trách và hạn |
| `#hoi-dap` | Hỏi nhanh ngoài chuyên môn | Ghi rõ câu hỏi và ngữ cảnh |
| `#tan-gau` | Meme, chuyện ngoài lề | Chỉ chuyện giải trí, được tắt thông báo |

Tách riêng `#tan-gau` để meme không đè lên thông báo kỹ thuật và deadline.

## Phần 2: Reply in Thread

- Mỗi vấn đề kỹ thuật chỉ có **một tin gốc** trong kênh, mọi trao đổi tiếp theo trả lời trong thread của tin đó.
- Khung chat chính chỉ còn tin gốc, dễ quét và không bị trôi.
- Khi xong việc, ghi kết luận cuối thread để tìm lại sau này.

## Phần 3: Bản quy ước giao tiếp, 3 quy tắc vàng

1. **Không No-Hello:** nhắn một tin đủ ngữ cảnh (việc gì, cần gì, hạn khi nào), không nhắn "có ai không" rồi chờ.
2. **Không spam @all:** tag đích danh người cần xử lý. Chỉ trưởng nhóm được dùng @all trong `#thong-bao` khi việc thật sự liên quan cả nhóm.
3. **Đúng kênh, đúng thread, đúng giờ:** nội dung nào kênh đó; trả lời trong thread; tin ngoài giờ làm việc dùng Schedule Send để gửi vào sáng hôm sau.

## Phần 4: Xử lý bẫy (ép rep ngay làm lập trình viên mất tập trung)

- **Nguyên nhân:** coi chat như gọi điện, kỳ vọng trả lời ngay.
- **Giải pháp theo Asynchronous Communication:**
  - Thống nhất thời gian phản hồi hợp lý, ví dụ trong vòng 2-4 giờ làm việc, không cần rep ngay.
  - Lập trình viên bật chế độ **Do Not Disturb** khi code, chỉ đọc tin vào các khung giờ cố định.
  - Người gửi viết đủ ngữ cảnh và nêu hạn, để người nhận trả lời một lần là xong.
  - Việc thật sự khẩn (hệ thống sập) thì gọi trực tiếp hoặc tag đích danh kèm chữ "KHẨN", không dùng chat thường.