# I. Git cơ bản

## 1. Git là gì ?

-   Git là một hệ thống quản lý phiên bản phân tán (Distributed Version Control System - DVCS) được tạo ra bởi Linus Torvalds năm 2005, nhằm quản lý mã nguồn của Linux Kernel.

## 2. Tại sao lại cần Git ?

-   Git giúp quản lý mã nguồn một cách hiệu quả, đồng thời giúp các lập trình viên làm việc cùng nhau trên cùng một dự án mà không cần phải ghi nhớ nhiều phiên bản khác nhau của mã nguồn.

## 3. GitHub là gì ?

-   GitHub là một dịch vụ cung cấp kho lưu trữ mã nguồn Git miễn phí, cho phép người dùng tạo các kho chứa mã nguồn công khai hoặc riêng tư, cũng như là một nền tảng mạng xã hội cho các lập trình viên.

## 4. Các khái niệm cơ bản trong Git

-   **Repository (kho chứa)**: là nơi lưu trữ tất cả các phiên bản của mã nguồn, có thể coi là một thư mục chứa toàn bộ dữ liệu của dự án.

-   **Commit (phiên bản)**: là một bản chụp của mã nguồn tại một thời điểm nhất định, có thể xem như một bản sao lưu của mã nguồn tại thời điểm đó.

-   **Branch (nhánh)**: là một phiên bản của mã nguồn được tách ra từ phiên bản gốc, có thể thay đổi mà không ảnh hưởng đến phiên bản gốc.

-   **Merge (hợp nhất)**: là quá trình kết hợp hai nhánh lại với nhau.

-   **Pull request (yêu cầu kéo)**: là một yêu cầu được tạo ra để hợp nhất các thay đổi từ một nhánh đến nhánh khác.

-   **Fork (bản sao)**: là một bản copy của một repository, cho phép người dùng thay đổi mã nguồn mà không ảnh hưởng đến repository gốc.

-   **Clone (nhân bản)**: là một bản copy của một repository, cho phép người dùng thay đổi mã nguồn và đẩy lên repository gốc.

## 5. Cài đặt Git

-   **Windows**: Tải Git tại [đây](https://git-scm.com/download/win) và cài đặt.

-   **Linux**: Mở Terminal và chạy lệnh sau:

```bash
sudo apt-get install git
```

-   **Mac**: Tải Git tại [đây](https://git-scm.com/download/mac) và cài đặt.

# II. Các lệnh cơ bản trong Git

## 1. Khởi tạo một repository

-   Để khởi tạo một repository, ta sử dụng lệnh sau:

```bash

git init

```

-   Sau khi khởi tạo, một thư mục `.git` sẽ được tạo ra, chứa toàn bộ dữ liệu của repository.

## 2. Thêm file vào repository

-   Để thêm một file vào repository, ta sử dụng lệnh sau:

```bash

git add <tên file>

```

-   Để thêm tất cả các file vào repository, ta sử dụng lệnh sau:

```bash

git add .

```

## 3. Commit

-   Để tạo một phiên bản, ta sử dụng lệnh sau:

```bash

git commit -m "<nội dung commit>"

```

-   Trong đó, `<nội dung commit>` là nội dung của phiên bản.

## 4. Xem danh sách các phiên bản

-   Để xem danh sách các phiên bản, ta sử dụng lệnh sau:

```bash

git log

```

## 5. Xem sự thay đổi của một phiên bản

-   Để xem sự thay đổi của một phiên bản, ta sử dụng lệnh sau:

```bash

git show <mã phiên bản>

```

-   Trong đó, `<mã phiên bản>` là mã của phiên bản cần xem.

## 6. Xem sự thay đổi của một file

-   Để xem sự thay đổi của một file, ta sử dụng lệnh sau:

```bash

git diff <tên file>

```

-   Trong đó, `<tên file>` là tên của file cần xem.

## 7. Xóa file

-   Để xóa một file, ta sử dụng lệnh sau:

```bash

git rm <tên file>

```

-   Sau khi xóa, ta cần commit lại để lưu thay đổi.

## 8. Đổi tên file

-   Để đổi tên một file, ta sử dụng lệnh sau:

```bash

git mv <tên file cũ> <tên file mới>

```

-   Sau khi đổi tên, ta cần commit lại để lưu thay đổi.

## 9. Đẩy lên repository

-   Để đẩy lên repository, ta sử dụng lệnh sau:

```bash

git push

```

**Lưu ý**: Để đẩy lên repository, ta cần phải đăng nhập vào GitHub trước.

Các tùy chọn:

-   `-u`: Để lưu thông tin đăng nhập.

-   `-f`: Để đẩy lên repository khi có xung đột.

## 10. Lấy về repository

-   Để lấy về repository, ta sử dụng lệnh sau:

```bash

git pull

```

## 11. Tạo nhánh (branch)

-   Để tạo một nhánh mới, ta sử dụng lệnh sau:

```bash

git branch <tên nhánh>

```

-   Sau khi tạo nhánh, ta cần chuyển sang nhánh đó để làm việc.

## 12. Chuyển nhánh

-   Để chuyển sang một nhánh khác, ta sử dụng lệnh sau:

```bash

git checkout <tên nhánh>

```

## 13. Xóa nhánh

-   Để xóa một nhánh, ta sử dụng lệnh sau:

```bash

git branch -d <tên nhánh>

```

## 14. Hợp nhất nhánh

-   Để hợp nhất một nhánh vào nhánh hiện tại, ta sử dụng lệnh sau:

```bash

git merge <tên nhánh>

```

## 15. Tạo phiên bản từ một nhánh

-   Để tạo một phiên bản từ một nhánh, ta sử dụng lệnh sau:

```bash

git checkout -b <tên nhánh>

```

# III. Các lệnh nâng cao trong Git

## 1. Tạo một repository trên GitHub

-   Để tạo một repository trên GitHub, ta làm theo các bước sau:

1. Đăng nhập vào GitHub.

2. Nhấn vào biểu tượng `+` ở góc trên bên phải và chọn `New repository`.

3. Đặt tên cho repository.

4. Chọn `Public` hoặc `Private`.

5. Chọn `Initialize this repository with a README`.

6. Nhấn `Create repository`.

## 2. Clone một repository

-   Để clone một repository, ta sử dụng lệnh sau:

```bash

git clone <đường dẫn>

```

-   Trong đó, `<đường dẫn>` là đường dẫn của repository.

## 3. Fork một repository

-   Fork một repository có nghĩa là tạo một bản sao của repository đó, cho phép người dùng thay đổi mã nguồn mà không ảnh hưởng đến repository gốc.

-   Để fork một repository, ta làm theo các bước sau:

1. Đăng nhập vào GitHub.

2. Vào repository cần fork.

3. Nhấn vào nút `Fork` ở góc trên bên phải.

## 4. Pull request

-   Pull request là một yêu cầu được tạo ra để hợp nhất các thay đổi từ một nhánh đến nhánh khác.

-   Để tạo một pull request, ta làm theo các bước sau:

1. Đăng nhập vào GitHub.

2. Vào repository cần tạo pull request.

3. Nhấn vào nút `New pull request`.

4. Chọn nhánh cần tạo pull request.

5. Nhấn `Create pull request`.
