Internal Troubleshooting & Bug Report Framework
Permalink: 🛠️ Internal Troubleshooting & Bug Report Framework
Quy trình chuẩn hóa giúp nhóm giải quyết sự cố môi trường (Docker, Port Conflict...) nhanh chóng và tránh trôi thông tin.
￼
1. Bug Report Template

***Bắt buộc:*** Điền đủ **4 thành phần** trong bảng dưới đây trước khi gửi yêu cầu hỗ trợ vào nhóm chat.

### 🐛 BUG REPORT

| Thành phần | Nội dung chi tiết | Ví dụ minh họa |
| :--- | :--- | :--- |
| **CONTEXT** | Ngữ cảnh môi trường làm việc | `HĐH: Windows 11` \| `Công cụ: Docker / Node.js` \| `Nhánh Git: main` |
| **EXPECTED** | Kết quả mong muốn đạt được | Chạy container thành công và ứng dụng lắng nghe ở cổng `8080`. |
| **ACTUAL** | Kết quả thực tế xảy ra | Container bị tắt ngay lập tức và hệ thống báo lỗi cổng `8080` bị chiếm dụng. |
| **LOG / ERROR** | Mã lỗi thô hoặc ảnh chụp | `Error: Bind for 0.0.0.0:8080 failed: port is already allocated` |

---
2. Quy trình 3 bước tự tra cứu (Self-Troubleshooting)
Permalink: 2. Quy trình 3 bước tự tra cứu (Self-Troubleshooting)
Thực hiện lần lượt 3 bước để tự xử lý 80% vấn đề trước khi nhờ hỗ trợ:
[1. Smart Googling] ➔ [2. Community Search] ➔ [3. AI & Fact-Checking]
￼
🔹 Bước 1: Smart Googling
Permalink: 🔹 Bước 1: Smart Googling
• Tìm mã lỗi chính xác trong dấu ngoặc kép: "port is already allocated" Windows 11
🔹 Bước 2: Community Search (GitHub & StackOverflow)
Permalink: 🔹 Bước 2: Community Search (GitHub & StackOverflow)
• Giới hạn tra cứu trên nguồn uy tín: site:stackoverflow.com "port is already allocated" site:github.com "port is already allocated"
• Ưu tiên các câu trả lời gần đây và có nhiều tương tác (👍).
🔹 Bước 3: AI Translation & Fact-Checking
Permalink: 🔹 Bước 3: AI Translation & Fact-Checking
• Nhờ AI giải thích nguyên nhân và đưa ra hướng xử lý:
"Giải thích lỗi này và đưa ra câu lệnh khắc phục an toàn: [Mã lỗi]"
• Lưu ý: Đối chiếu câu lệnh với tài liệu chính thức trước khi dán vào Terminal để tránh hỏng hệ thống.
