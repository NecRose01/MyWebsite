+++
draft = true
title = "Các Biến Thường Được Sử Dụng Trong Java" 
date = "2024-12-30"
description = "Tìm hiểu các loại biến phổ biến trong Java và cách sử dụng chúng."
tags = [ "Java", "Biến", "Lập trình cơ bản", ] 
+++
Trong lập trình Java, **biến** là một yếu tố quan trọng giúp lưu trữ và quản lý dữ liệu. Bài viết này sẽ giới thiệu các loại biến thường được sử dụng trong Java và cách sử dụng chúng.

---

## 1. Biến Cục Bộ (Local Variable)

### Định nghĩa:
- Là biến được khai báo bên trong một phương thức, khối mã, hoặc constructor.
- Chỉ có thể được sử dụng trong phạm vi của khối hoặc phương thức mà nó được khai báo.

### Ví dụ:
```java
public class LocalVariableExample {
    public void displayMessage() {
        int number = 10; // Biến cục bộ
        System.out.println("Số: " + number);
    }
}
```

### Lưu ý:
- Biến cục bộ phải được khởi tạo trước khi sử dụng.
- Chúng không có giá trị mặc định.

---

## 2. Biến Thành Viên (Instance Variable)

### Định nghĩa:
- Là biến được khai báo bên ngoài các phương thức nhưng bên trong một lớp.
- Biến này thuộc về một đối tượng cụ thể của lớp.

### Ví dụ:
```java
public class InstanceVariableExample {
    String name; // Biến thành viên

    public void displayName() {
        System.out.println("Tên: " + name);
    }
}
```

### Lưu ý:
- Biến thành viên có giá trị mặc định (ví dụ: `null` cho kiểu chuỗi, `0` cho kiểu số).
- Chúng tồn tại miễn là đối tượng của lớp còn tồn tại.

---

## 3. Biến Tĩnh (Static Variable)

### Định nghĩa:
- Là biến được khai báo với từ khóa `static` trong lớp.
- Biến tĩnh là thuộc tính chung của tất cả các đối tượng trong lớp (chia sẻ giá trị giữa các đối tượng).

### Ví dụ:
```java
public class StaticVariableExample {
    static int count = 0; // Biến tĩnh

    public StaticVariableExample() {
        count++;
    }

    public static void displayCount() {
        System.out.println("Số lượng đối tượng: " + count);
    }
}
```

### Lưu ý:
- Biến tĩnh được khởi tạo một lần và được lưu trữ trong bộ nhớ tĩnh (static memory).
- Có thể truy cập trực tiếp bằng tên lớp mà không cần tạo đối tượng.

---

## 4. Biến Hằng (Final Variable)

### Định nghĩa:
- Là biến được khai báo với từ khóa `final`, giá trị của nó không thể thay đổi sau khi khởi tạo.

### Ví dụ:
```java
public class FinalVariableExample {
    final int MAX_VALUE = 100; // Biến hằng

    public void displayMaxValue() {
        System.out.println("Giá trị tối đa: " + MAX_VALUE);
    }
}
```

### Lưu ý:
- Biến `final` phải được khởi tạo ngay khi khai báo hoặc trong constructor.
- Giá trị của biến này không thể bị thay đổi.

---

## 5. Biến Truyền Vào Phương Thức (Parameter Variable)

### Định nghĩa:
- Là biến được khai báo trong danh sách tham số của phương thức.
- Biến này được sử dụng để nhận giá trị truyền vào khi gọi phương thức.

### Ví dụ:
```java
public class ParameterVariableExample {
    public void printMessage(String message) { // Biến truyền vào
        System.out.println("Thông điệp: " + message);
    }
}
```

### Lưu ý:
- Giá trị của biến tham số được truyền từ đối số khi gọi phương thức.

---

## Kết luận

Biến là công cụ quan trọng để lưu trữ dữ liệu trong Java. Hiểu rõ các loại biến như biến cục bộ, biến thành viên, biến tĩnh, biến hằng, và biến tham số sẽ giúp bạn quản lý dữ liệu hiệu quả và viết mã nguồn dễ bảo trì hơn. Hãy thực hành nhiều để làm quen với cách sử dụng các loại biến này!
