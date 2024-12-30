+++
author = "Hugo Authors"
title = "Cách Cài Java và JavaScript"
date = "2024-12-30"
description = "Hướng dẫn chi tiết cách cài đặt Java và JavaScript trên hệ điều hành Windows, macOS và Linux."
tags = [
    "java", "javascript", "cài đặt", "lập trình"
]
+++

Để bắt đầu lập trình với **Java** và **JavaScript**, bạn cần cài đặt các công cụ cần thiết. Dưới đây là hướng dẫn chi tiết về cách cài đặt Java và JavaScript trên các hệ điều hành phổ biến: Windows, macOS và Linux.

<!--more-->

### 1. Cài Đặt Java

Java là một ngôn ngữ lập trình phổ biến được sử dụng rộng rãi trong phát triển ứng dụng, đặc biệt là ứng dụng web và di động. Để cài đặt Java, bạn cần cài đặt **Java Development Kit (JDK)**.

#### Cài Đặt Java trên Windows

1. Truy cập trang web chính thức của Oracle để tải JDK:
    - Link: [Download JDK](https://www.oracle.com/java/technologies/javase-jdk14-downloads.html)

2. Tải về phiên bản JDK mới nhất phù hợp với hệ điều hành Windows của bạn (32-bit hoặc 64-bit).

3. Chạy tệp cài đặt và làm theo hướng dẫn trên màn hình.

4. Sau khi cài đặt, bạn cần cấu hình **JAVA_HOME** và thêm Java vào biến môi trường `PATH`:
    - Vào **Control Panel > System and Security > System > Advanced System Settings**.
    - Chọn **Environment Variables**.
    - Trong phần **System variables**, nhấn **New** và thêm `JAVA_HOME` với giá trị là thư mục cài đặt JDK (ví dụ: `C:\Program Files\Java\jdk-14`).
    - Chỉnh sửa biến `Path` và thêm đường dẫn tới thư mục `bin` của JDK (ví dụ: `C:\Program Files\Java\jdk-14\bin`).

5. Kiểm tra cài đặt Java bằng cách mở Command Prompt và gõ:
   ```bash
   java -version
Nếu cài đặt thành công, bạn sẽ thấy thông tin phiên bản Java.
#### Cài Đặt Java trên macOS
1. Truy cập trang web Oracle để tải JDK hoặc cài đặt qua Homebrew:

```bash
brew install openjdk@17
```
2. Đặt biến môi trường JAVA_HOME bằng cách thêm dòng sau vào file ~/.bash_profile hoặc ~/.zshrc:

```bash
export JAVA_HOME=$(/usr/libexec/java_home -v 17)
```
3. Kiểm tra cài đặt bằng lệnh:

```bash
java -version
```
#### Cài Đặt Java trên Linux
1. Mở Terminal và sử dụng lệnh sau để cài đặt OpenJDK:

```bash
sudo apt update
sudo apt install openjdk-17-jdk
```
2. Kiểm tra cài đặt bằng lệnh:

```bash
java -version
```
### 2. Cài Đặt JavaScript
JavaScript là ngôn ngữ kịch bản phổ biến được sử dụng trong phát triển web. Để bắt đầu viết JavaScript, bạn không cần phải cài đặt một công cụ biên dịch như Java. Tuy nhiên, bạn cần cài đặt Node.js nếu muốn chạy JavaScript trên máy tính của mình thay vì chỉ chạy trên trình duyệt.

**Cài Đặt JavaScript (Node.js) trên Windows**
1. Truy cập trang web chính thức của Node.js:

- Link: [Download Node.js](https://nodejs.org/fr)
2. Tải về phiên bản LTS (Long-Term Support) của Node.js cho Windows.

3. Chạy tệp cài đặt và làm theo hướng dẫn trên màn hình.

4. Kiểm tra cài đặt bằng cách mở Command Prompt và gõ:

```bash
node -v
```
Nếu cài đặt thành công, bạn sẽ thấy phiên bản Node.js.

### Cài Đặt JavaScript (Node.js) trên macOS
1. Cài đặt Homebrew (nếu chưa cài):

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
2. Cài đặt Node.js qua Homebrew:

```bash
brew install node
```
3. Kiểm tra cài đặt bằng cách chạy lệnh:

```bash
node -v
```
### Cài Đặt JavaScript (Node.js) trên Linux
1. Cài đặt Node.js từ NodeSource repository:

```bash
curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
sudo apt install -y nodejs
```
2. Kiểm tra cài đặt bằng lệnh:

```bash
node -v
```
### 3. Cài Đặt Trình Biên Dịch (IDE) cho Java và JavaScript
Để lập trình hiệu quả hơn, bạn cần cài đặt một IDE (Integrated Development Environment) hoặc Text Editor hỗ trợ cả Java và JavaScript.

#### IDE cho Java
- IntelliJ IDEA: Một IDE mạnh mẽ cho Java với nhiều tính năng hỗ trợ phát triển ứng dụng Java. Link tải: IntelliJ IDEA
- Eclipse: Một IDE phổ biến cho phát triển Java. Link tải: Eclipse IDE
#### IDE cho JavaScript
- Visual Studio Code: Một text editor mạnh mẽ cho JavaScript và nhiều ngôn ngữ khác. Link tải: VS Code
- WebStorm: Một IDE chuyên dụng cho JavaScript, HTML và CSS. Link tải: WebStorm
## Kết luận
Với Java, bạn cần cài đặt JDK và cấu hình môi trường để có thể lập trình, trong khi JavaScript chỉ cần cài đặt Node.js để chạy mã JavaScript ngoài trình duyệt. Hãy cài đặt các công cụ và IDE phù hợp để tạo ra một môi trường lập trình hiệu quả. Chúc bạn lập trình thành công!