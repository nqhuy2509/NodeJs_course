# I. Basic Fundamental

## 1.Internet là gì ? TCP/IP là gì ?

**Internet** là một hệ thống toàn cầu kết nối hàng tỉ người dùng và thiết bị trên toàn thế giới

**Transmission Control Protocol (TCP):**

-   TCP là một giao thức tầng giao vận (transport layer protocol) trong mô hình OSI.
-   Nhiệm vụ chính của TCP là cung cấp một cách đáng tin cậy để truyền dữ liệu giữa các thiết bị trên mạng.
-   Nó đảm bảo rằng dữ liệu được chia thành các gói và được gửi một cách an toàn và đúng đắn. Nếu một gói bị mất hoặc bị hỏng, TCP sẽ yêu cầu gửi lại gói đó.

**Internet Protocol (IP):**

-   IP là một giao thức tầng mạng (network layer protocol) trong mô hình OSI.
-   Nhiệm vụ chính của IP là xác định cách địa chỉ của mỗi thiết bị trên mạng, gọi là địa chỉ IP.
-   Địa chỉ IP là quan trọng để định vị và liên kết dữ liệu với các thiết bị cụ thể trong mạng.
-   Nó cũng đảm bảo rằng dữ liệu được gửi đến đúng địa chỉ.

## 2. DNS là gì ? Domain là gì ?

**DNS (Domain Name System):**

-   DNS là một hệ thống dịch địa chỉ IP thành tên miền và ngược lại.Nó giúp máy tính xác định địa chỉ IP của một tên miền cụ thể
-   Chức năng chính:
    -   Dịch IP - tên miền: Khi nhập một tên miền vào trình duyệt, DNS chuyển đổi nó thành địa chỉ IP của máy chủ đó.
    -   Dịch tên miền - IP : Khi máy chủ muốn gửi dữ liệu , DNS giúp nó xác định địa chỉ IP của máy tính.

**Domain (Tên Miền):**

-   Domain là một địa chỉ nhận diện trên Internet. Nó thường được sử dụng để xác định địa chỉ của một trang web hay một nguồn tài nguyên trên mạng.
-   Cấu Trúc Tên Miền:
    -   Top-Level Domain (TLD): Phần cuối cùng của tên miền, như .com, .org, .net.
    -   Second-Level Domain (SLD): Phần nằm trước TLD, là phần tên riêng, như example trong example.com.
    -   Subdomain: Cấp phụ của SLD, được thêm vào trước SLD, ví dụ: blog.example.com.

## 3. Hosting là gì ? VPS là gì ? Cloud là gì ?

**Hosting:**

-   Hosting là dịch vụ lưu trữ website trên một máy chủ đặt tại trung tâm dữ liệu (Data Center) có đường truyền Internet tốc độ cao, ổn định, đảm bảo an toàn và bảo mật thông tin.

**VPS (Virtual Private Server):**

-   VPS là một máy chủ ảo, được tạo ra bằng cách phân chia một máy chủ vật lý thành nhiều máy chủ ảo, mỗi máy chủ ảo đều có đầy đủ tài nguyên như một máy chủ vật lý.

**Cloud:**

-   Cloud là một mô hình lưu trữ dữ liệu trên một hệ thống máy chủ ảo, được phân tán trên nhiều máy chủ vật lý, được quản lý bởi một hệ thống điều khiển trung tâm.

## 4. HTTP là gì ? HTTP Request là gì ? HTTP Response là gì ?

**HTTP (Hypertext Transfer Protocol):**

-   HTTP là một giao thức truyền tải dữ liệu trên Internet. Nó hoạt động dựa trên mô hình yêu cầu (request) và phản hồi (response).

**HTTP Request:**

-   HTTP Request là một thông điệp được gửi từ Client đến Server, yêu cầu Server thực hiện một hành động nào đó.

**HTTP Response:**

-   HTTP Response là một thông điệp được gửi từ Server đến Client, báo hiệu kết quả của một yêu cầu đã được thực hiện.

## 5. HTTP Method là gì ? GET Method là gì ? POST Method là gì ?

**HTTP Method:**

-   HTTP Method là một phương thức được sử dụng để chỉ định hành động mà Client muốn Server thực hiện.

**GET Method:**

-   GET Method được sử dụng để yêu cầu Server trả về một tài nguyên cụ thể.

**POST Method:**

-   POST Method được sử dụng để gửi dữ liệu từ Client lên Server.

## 6. HTTP Status Code là gì

**HTTP Status Code:**

-   HTTP Status Code là một mã trạng thái được trả về bởi Server cho Client, báo hiệu kết quả của một yêu cầu đã được thực hiện.

**Các loại HTTP Status Code:**

-   1xx: Informational (Thông tin)

-   2xx: Success (Thành công)

-   3xx: Redirection (Chuyển hướng)

-   4xx: Client Error (Lỗi của Client)

-   5xx: Server Error (Lỗi của Server)

**Tham khảo thêm:**

-   [HTTP Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)

## 7. HTTP Header là gì ? HTTP Body là gì ?

**HTTP Header:**

-   HTTP Header là một phần của HTTP Request hoặc HTTP Response, chứa các thông tin bổ sung về Request hoặc Response.

**HTTP Body:**

-   HTTP Body là một phần của HTTP Request hoặc HTTP Response, chứa dữ liệu được gửi đi hoặc nhận về.

## 8. HTTP Cookie là gì ? HTTP Session là gì ?

**HTTP Cookie:**

-   HTTP Cookie là một đoạn dữ liệu được lưu trữ trên máy tính của Client, được gửi từ Server đến Client thông qua HTTP Response.

**HTTP Session:**

-   HTTP Session là một đoạn dữ liệu được lưu trữ trên Server, được tạo ra khi Client gửi một HTTP Request đến Server.

## 9. HTTP Cache là gì ? HTTP Cache-Control là gì ?

**HTTP Cache:**

-   HTTP Cache là một bộ nhớ tạm trên Client, được sử dụng để lưu trữ các tài nguyên đã được truy cập trước đó.

**HTTP Cache-Control:**

-   HTTP Cache-Control là một HTTP Header, được sử dụng để kiểm soát việc lưu trữ các tài nguyên vào HTTP Cache.

## 10. HTTP Proxy là gì ? HTTP Reverse Proxy là gì ?

**HTTP Proxy:**

-   HTTP Proxy là một máy chủ trung gian, được sử dụng để truy cập Internet thông qua một máy chủ trung gian.

-   HTTP Proxy có thể được cấu hình để lưu trữ các tài nguyên vào HTTP Cache.

**HTTP Reverse Proxy:**

-   HTTP Reverse Proxy là một máy chủ trung gian, được sử dụng để truy cập Internet thông qua một máy chủ trung gian.

-   HTTP Reverse Proxy có thể được cấu hình để lưu trữ các tài nguyên vào HTTP Cache.

-   HTTP Reverse Proxy có thể được cấu hình để phân phối tải (load balancing) cho các máy chủ vật lý.

## 11. HTTP Load Balancing là gì ?

**HTTP Load Balancing:**

-   HTTP Load Balancing là một kỹ thuật được sử dụng để phân phối tải (load balancing) cho các máy chủ vật lý.

-   HTTP Load Balancing có thể được thực hiện bằng cách sử dụng một HTTP Reverse Proxy.

# II. Mô hình Client-Server

## 1. Các mô hình mạng phổ biến. Mô hình Client-Server là gì ?

### a. Các mô hình mạng phổ biến

**Mô hình mạng:**

-   Mô hình mạng là một mô hình được sử dụng để mô tả cách mà các thiết bị trong mạng giao tiếp với nhau.

-   Mô hình mạng được sử dụng để phân loại các mạng theo cách mà các thiết bị trong mạng giao tiếp với nhau.

**Các mô hình mạng phổ biến:**

-   Các mô hình mạng phổ biến bao gồm: Mô hình Client-Server, Mô hình Peer-to-Peer.

### b. Mô hình Client-Server

**Mô hình Client-Server:**

-   Mô hình Client-Server là một mô hình trong đó Client và Server giao tiếp với nhau thông qua mạng.

-   Client là một thiết bị yêu cầu dịch vụ từ Server.

-   Server là một thiết bị cung cấp dịch vụ cho Client.

## 2. Mô hình Client-Server hoạt động như thế nào ?

**_Mô hình Client-Server hoạt động như sau:_**

-   Client gửi một yêu cầu (request) đến Server.

-   Server nhận yêu cầu từ Client và thực hiện một hành động nào đó.

-   Server gửi một phản hồi (response) đến Client.

-   Client nhận phản hồi từ Server và thực hiện một hành động nào đó.

## 3. Mô hình Client-Server có những ưu điểm và nhược điểm gì ?

**_Mô hình Client-Server có những ưu điểm và nhược điểm như sau:_**

**Ưu điểm:**

-   Mô hình Client-Server cho phép Client và Server giao tiếp với nhau thông qua mạng.

-   Mô hình Client-Server cho phép Client và Server được phân tách với nhau.

-   Mô hình Client-Server cho phép Client và Server được phát triển độc lập với nhau.

**Nhược điểm:**

-   Mô hình Client-Server có thể gây ra một số vấn đề về bảo mật.

-   Mô hình Client-Server có thể gây ra một số vấn đề về hiệu năng.

## Font-end là gì ? Back-end là gì ?

**Front-end:**

-   Front-end là một phần của một ứng dụng, được sử dụng để hiển thị giao diện người dùng và tương tác với người dùng.

-   Front-end được thực hiện bằng các ngôn ngữ lập trình như HTML, CSS, JavaScript.

**Back-end:**

-   Back-end là một phần của một ứng dụng, được sử dụng để xử lý dữ liệu và tương tác với cơ sở dữ liệu.

-   Back-end được thực hiện bằng các ngôn ngữ lập trình như PHP, Java, Python, Ruby.
