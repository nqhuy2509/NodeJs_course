# Backend fundamental
## What is the Internet ? TCP/IP? HTTP?
**Internet** là một hệ thống toàn cầu kết nối hàng tỉ người dùng và thiết bị trên toàn thế giới

**Transmission Control Protocol (TCP):**
-  TCP là một giao thức tầng giao vận (transport layer protocol) trong mô hình OSI.
- Nhiệm vụ chính của TCP là cung cấp một cách đáng tin cậy để truyền dữ liệu giữa các thiết bị trên mạng.
- Nó đảm bảo rằng dữ liệu được chia thành các gói và được gửi một cách an toàn và đúng đắn. Nếu một gói bị mất hoặc bị hỏng, TCP sẽ yêu cầu gửi lại gói đó.

**Internet Protocol (IP):**
- IP là một giao thức tầng mạng (network layer protocol) trong mô hình OSI.
- Nhiệm vụ chính của IP là xác định cách địa chỉ của mỗi thiết bị trên mạng, gọi là địa chỉ IP.
- Địa chỉ IP là quan trọng để định vị và liên kết dữ liệu với các thiết bị cụ thể trong mạng.

**HTTP / HTTPS:**
-  HTTP (Hypertext Transfer Protocol) : là một giao thức truyền tải dữ liệu trên Internet. Nó hoạt động dựa trên mô hình yêu cầu (request) và phản hồi (response).
- HTTPS (Hypertext Transfer Protocol Secure): HTTPS là phiên bản an toàn của HTTP sử dụng SSL/TLS để bảo vệ dữ liệu truyền tải.Dữ liệu giữa máy khách và máy chủ được mã hóa.
## What is DNS ? Domain

**DNS (Domain Name System):**
- DNS là một hệ thống dịch địa chỉ IP thành tên miền và ngược lại.Nó giúp máy tính xác định địa chỉ IP của một tên miền cụ thể
- Chức năng chính: 
    - Dịch IP - tên miền:  Khi nhập một tên miền vào trình duyệt, DNS chuyển đổi nó thành địa chỉ IP của máy chủ đó.
    - Dịch tên miền - IP : Khi máy chủ muốn gửi dữ liệu , DNS giúp nó xác định địa chỉ IP của máy tính.

**Domain (Tên Miền):**
- Domain là một địa chỉ nhận diện trên Internet. Nó thường được sử dụng để xác định địa chỉ của một trang web hay một nguồn tài nguyên trên mạng.
- Cấu Trúc Tên Miền:
    - Top-Level Domain (TLD): Phần cuối cùng của tên miền, như .com, .org, .net.
    - Second-Level Domain (SLD): Phần nằm trước TLD, là phần tên riêng, như example trong example.com.
    - Subdomain: Cấp phụ của SLD, được thêm vào trước SLD, ví dụ: blog.example.com.
