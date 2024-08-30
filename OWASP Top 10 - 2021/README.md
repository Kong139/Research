### What is OWASP?
The Open Web Application Security Project, hay OWASP, là một tổ chức quốc tế phi lợi nhuận chuyên về bảo mật ứng dụng web. Một trong những nguyên tắc cốt lõi của OWASP là tất cả tài liệu của họ đều miễn phí và dễ dàng truy cập. Trong đó nổi tiếng nhất có lẽ là OWASP Top 10.

---
# OWASP Top 10
Là một báo cáo được cập nhật thường xuyên về 10 rủi ro bảo mật nghiêm trọng nhất đối với ứng dụng web.
## 1. Broken Access Control
(Kiểm soát truy cập bị hỏng)

Các lỗi về việc kiểm soát truy cập
## 2. Cryptographic Failures
(Lỗi mật mã)

Bất kì lỗ hổng nào liên quan đến việc sử dụng sai, hoặc không sử dụng các thuật toán mật mã để bảo vệ thông tin nhạy cảm.
## 3. Injection
(Tiêm)

Một kiểu tấn công xảy ra khi untrusted data được đưa vào trình thông dịch code từ các biểu mẫu đầu vào (form input) hoặc một số dữ liệu khác được gửi tới ứng dụng web.
## 4. Insecure Design
(Thiết kế không an toàn)

Các lỗ hổng về thiết kế có thể xuất hiện khi phát triển chương trình, ứng dụng có thiết kế kém bảo mật.
## 5. Security Misconfiguration
(Cấu hình bảo mật sai)

Các lỗi liên quan đến việc cấu hình, như cấu hình sai, cấu hình thiếu, dùng mật khẩu mặc định, thông báo lỗi chứa quá nhiều thông tin...
## 6. Vulnerable and Outdated Components
(Các thành phần dễ bị tổn thương và lỗi thời)

Các rủi ro bảo mật khi dùng các phần mềm lỗi thời, dễ bị tấn công, hoặc do không cập nhật/nâng cấp các thành phần được sử dụng như libraries, platform, frameworks, dependencies,...
## 7. Identification and Authentication Failures
(Lỗi nhận dạng và xác thực)

Các lỗ hổng về nhận dạng và xác thực như không chặn các cuộc tấn công brute force hay các dạng tấn công tự động khác, dùng mật khẩu yếu hoặc không mã hóa/mã hóa yếu...
## 8. Software and Data Integrity Failures
(Lỗi về tính toàn vẹn của phần mềm và dữ liệu)

Các lỗi liên quan đến việc code và cơ sở hạ tầng không chống lại các *vi phạm tính toàn vẹn* (integrity violations)
## 9. Security Logging and Monitoring Failures
(Lỗi ghi nhật ký và giám sát bảo mật)

Rủi ro liên quan đến việc không ghi nhật ký và giám sát các hoạt động quan trọng như đăng nhập, cảnh báo, lỗi,... đẫn đến việc không phát hiện được xâm nhập.
## 10. Server-Side Request Forgery
(Làm giả yêu cầu phía máy chủ)

Là lỗ hổng bảo mật web cho phép kẻ tấn công khiến ứng dụng phía máy chủ thực hiện yêu cầu đến một vị trí không mong muốn. Trong một cuộc tấn công SSRF thông thường, kẻ tấn công có thể khiến máy chủ kết nối với các dịch vụ chỉ dành cho nội bộ trong cơ sở hạ tầng của tổ chức.
