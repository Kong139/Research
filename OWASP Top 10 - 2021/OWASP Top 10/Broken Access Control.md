# Broken Access Control
I. [Broken Access Control là gì?](#componentI)

II. [Các kiểu tấn công Broken Access Control](#componentII)
1. [URL Manipulation (Thao tác URL)](#component1) 
2. [Exploiting Endpoints (Khai thác điểm cuối)](#component2)
3. [Elevating User Privilege (Leo thang đặc quyền)](#component3)
4. [Insecure Direct Object References (IDOR) (Tham chiếu đối tượng trực tiếp không an toàn)](#component4)
## I. Broken Access Control là gì? <a name="componentI"></a>
Broken Access Control (Kiểm soát truy cập bị hỏng) là lỗi về việc kiểm soát truy cập, cho phép attacker bỏ qua bước xác thực và truy cập vào các dữ liệu nhạy cảm hay thực hiện các tác vụ mà chúng không được phép.
## II. Các kiểu tấn công Broken Access Control<a name="componentII"></a>
### 1. URL Manipulation (Thao tác URL)<a name="component1"></a>
Là một phương pháp đơn giản được attacker sử dụng để khai thác lỗ hổng Broken Access Control. Bằng cách thay đổi URL, attacker có khả năng truy cập vào các thông tin hay chức năng nhạy cảm của trang web.
> Ví dụ: thay đổi username trong URL để xem thông tin của user khác nếu trang web được cấu hình không chính xác:
> 
> https://app.com/user01 :arrow_right: https://app.com/user02
### 2. Exploiting Endpoints (Khai thác điểm cuối)<a name="component2"></a>
- Điểm cuối là điểm tương tác giữa ứng dụng và phần còn lại của hệ thống. Chúng có thể là API, microservices, hoặc bất kỳ dịch vụ nào khác mà ứng dụng dựa vào. Nếu các điểm cuối này không được bảo mật đúng cách, kẻ tấn công có thể sử dụng chúng để vượt qua kiểm soát truy cập.
- Attacker có thể phát hiện endpoints không được bảo vệ qua nhiều cách khác nhau, chẳng hạn như scan network, phân tích code của ứng dụng hoặc thậm chí đoán URL của endpoints.
### 3. Elevating User Privilege (Leo thang đặc quyền)<a name="component3"></a>
Là phương pháp tấn công liên quan đến quyền người dùng. Attacker sẽ chiếm một tài khoản cấp thấp trước, sau đó tìm cách truy cập vào các tài khoản cấp cao hơn chẳng hạn như tài khoản admin.
### 4. Insecure Direct Object References (IDOR) (Tham chiếu đối tượng trực tiếp không an toàn)<a name="component4"></a>
Là một loại lỗ hổng trong đó ứng dụng hiển thị các tham chiếu trực tiếp đến các đối tượng trong nội bộ, như database keys, đường dẫn tệp hay bất cứ tham chiếu nội bộ nào khác. Nếu attacker có thể đoán hoặc brute-force các tham chiếu này, họ có thể bỏ qua kiểm soát truy cập và truy cập vào các dữ liệu nhạy cảm.
> Ví dụ: bạn truy cập vào tài khoản ngân hàng của mình trên trang wed, sau khi đăng nhập thì bạn được đưa đến trang web này https://bank.thm/account?id=111111. Nhìn có vẻ rất bình thường.
> 
![](/img/1.png)
> 
> Tuy nhiên, có một vấn đề rất lớn ở đây là ai cũng có thể thay đổi thông số id từ 111111 thành 222222 hoặc bất kỳ số nào, và nếu trang web được cấu hình không chính xác thì họ có thể truy cập vàp thông tin ngân hàng của người khác mà không cần xác thực.
> 
![](/img/2.png)
