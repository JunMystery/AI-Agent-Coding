# 🛠️ Project-Specific AI Agent Standards

File này chứa các chuẩn mực, quy ước và quy tắc dành riêng cho dự án này. AI Agent bắt buộc phải tuân thủ các quy tắc trong đây, song song với các bộ tiêu chuẩn lõi (như `GEMINI.md`, `CLAUDE.md`).

> **💡 Hướng dẫn:** 
> - Hoạt động độc lập: Chỉ cần tạo/sửa file này, AI Agent sẽ tự động nhận diện.
> - **Tùy biến hoàn toàn:** Bạn có quyền tự thêm các trường thông tin mới (VD: "Người review", "Ngày áp dụng") nếu thấy cần thiết. Miễn là nó ở dạng danh sách (bullet point).
> - Sử dụng file này để định nghĩa: kiến trúc dự án, thư viện ưu tiên, quy ước đặt tên, luồng xử lý lỗi, v.v.

---

## 🏗️ Khung Mẫu (Template)

*(Copy khối dưới đây để thêm một chuẩn mực mới. Bạn có thể tự ý thêm/bớt bất kỳ trường thông tin nào tùy theo nhu cầu)*

### [Tên Chuẩn mực / Hạng mục]
- **Quy tắc (Bắt buộc):** [Mô tả rõ ràng quy tắc AI cần tuân theo]
- **Lý do (Bắt buộc):** [Giải thích ngắn gọn lý do có quy tắc này]
- **Nên làm / Ví dụ Đúng (Tùy chọn):** [Ví dụ về code/hành vi đúng]
- **Không nên / Ví dụ Sai (Tùy chọn):** [Ví dụ về code/hành vi sai]
- **Phạm vi áp dụng (Tùy chọn):** [Ví dụ: Chỉ áp dụng cho code Frontend, hoặc chỉ các file .ts]
- **Tài liệu tham chiếu (Tùy chọn):** [Link hoặc đường dẫn đến tài liệu, file design, issue...]
- **Ngoại lệ (Tùy chọn):** [Các trường hợp không cần áp dụng quy tắc này]
- **Lệnh Terminal (Tùy chọn):** [Các lệnh cần chạy, ví dụ: npm run lint]
- **Cách Kiểm thử (Tùy chọn):** [Làm sao để biết quy tắc này đã được tuân thủ?]

---

## 📋 Danh sách Chuẩn mực của Dự án (Tùy chỉnh bên dưới)

### 1. Quy ước đặt tên file cấu hình (Ví dụ mẫu - Vui lòng xóa/thay thế)
- **Quy tắc (Bắt buộc):** Tất cả các file cấu hình mới phải sử dụng `kebab-case` và có hậu tố là `.config.json`.
- **Lý do (Bắt buộc):** Đảm bảo sự đồng nhất và dễ dàng tìm kiếm cấu hình trong toàn bộ dự án.
- **Nên làm / Ví dụ Đúng (Tùy chọn):** `database-connection.config.json`
- **Không nên / Ví dụ Sai (Tùy chọn):** `DatabaseConnection.json`, `db_config.json`
- **Phạm vi áp dụng (Tùy chọn):** Chỉ áp dụng cho các file cấu hình nằm trong thư mục `/config`.
- **Ngoại lệ (Tùy chọn):** Không áp dụng cho các file cấu hình mặc định của framework (ví dụ `package.json`, `tsconfig.json`).
