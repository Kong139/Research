# Cryptographic Failures
I. [Cryptographic Failures là gì?](#componentI)

II. [Một số trường hợp phổ biến dẫn đến lỗi mật mã](#componentII)
1. [Not Using Encryption (Không sử dụng mã hóa)](#component1)
2. [Insecure Cryptographic Functions (Chức năng mật mã không an toàn)](#component2)
3. [Improper Key Managemen (Quản lý khóa không đúng cách)](#component3)
## I. Cryptographic Failures là gì?<a name="componentI"></a>
Theo OWASP, Cryptographic Failures (Lỗi mật mã) là một triệu chứng chứ không phải là nguyên nhân. Bất kỳ lỗi nào gây ra lộ dữ liệu nhạy cảm và quan trọng cho một thực thể trái phép đều có thể được coi là lỗi mật mã.
## II. Một số trường hợp phổ biến dẫn đến lỗi mật mã<a name="componentII"></a>
### 1. Not Using Encryption (Không sử dụng mã hóa)<a name="component1"></a>
Các dữ liệu nhạy cảm phải luôn được mã hóa khi truyền qua mạng hoặc lưu trữ trên máy chủ.
### 2. Insecure Cryptographic Functions (Chức năng mật mã không an toàn)<a name="component2"></a>
Các chức năng mật mã có thể được triển khai không an toàn, dẫn đến lỗ hổng.
### 3. Improper Key Managemen (Quản lý khóa không đúng cách)<a name="component3"></a>
Khóa bảo mật rất quan trọng đối với bất kỳ hệ thống nào, vì vậy phải quản lý chúng đúng cách.
## III. Làm thế nào để phòng tránh các lỗi mật mã
- **Dùng các thuật toán mã hóa mạnh mẽ** - áp dụng các tiêu chuẩn mới nhất và ngành chấp nhận như AES hay RSA.
- **Thường xuyên cập nhật thư viện mật mã** - để tránh các thuật toán lỗi thời và không an toàn.
- **Quy trình quản lý khóa phù hợp** - việc tạo, lưu trữ khóa mã hóa an toàn là điều tối quan trọng.
- **Dùng các giao thức an toàn như HTTPS và TLS**
