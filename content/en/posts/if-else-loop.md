+++
author = "Hugo Authors"
title = "Câu Lệnh If-Else Trong Java"
date = "2024-12-30"
description = "Tìm hiểu cách sử dụng câu lệnh điều kiện if-else trong Java"
tags = [
    "java", "câu lệnh if-else", "lập trình"
]
+++

Trong Java, câu lệnh `if-else` là một cấu trúc điều kiện phổ biến, cho phép thực thi mã dựa trên kết quả của một điều kiện logic.

<!--more-->

### Cú pháp cơ bản của `if-else`

```java
if (điều_kiện) {
    // Khối lệnh thực thi nếu điều kiện đúng
} else {
    // Khối lệnh thực thi nếu điều kiện sai
}
```

Ví dụ:

```java
public class IfElseExample {
    public static void main(String[] args) {
        int number = 10;

        if (number > 0) {
            System.out.println("Số là số dương.");
        } else {
            System.out.println("Số là số không hoặc số âm.");
        }
    }
}
```

### Sử dụng `if-else if-else`

Bạn có thể kiểm tra nhiều điều kiện bằng cách sử dụng cấu trúc `if-else if-else`:

```java
if (điều_kiện1) {
    // Khối lệnh thực thi nếu điều kiện1 đúng
} else if (điều_kiện2) {
    // Khối lệnh thực thi nếu điều kiện2 đúng
} else {
    // Khối lệnh thực thi nếu không điều kiện nào đúng
}
```

Ví dụ:

```java
public class IfElseIfExample {
    public static void main(String[] args) {
        int number = -10;

        if (number > 0) {
            System.out.println("Số là số dương.");
        } else if (number == 0) {
            System.out.println("Số là số không.");
        } else {
            System.out.println("Số là số âm.");
        }
    }
}
```

### Các lưu ý quan trọng
1. Điều kiện trong `if` hoặc `else if` phải trả về giá trị boolean (`true` hoặc `false`).
2. Bạn có thể lồng nhiều câu lệnh `if-else`.

```java
if (điều_kiện1) {
    if (điều_kiện2) {
        // Khối lệnh thực thi nếu cả điều kiện1 và điều kiện2 đúng
    }
}
```

Sử dụng câu lệnh `if-else` hiệu quả sẽ giúp mã nguồn của bạn dễ đọc và dễ bảo trì hơn.

+++
author = "Hugo Authors"
title = "Vòng Lặp For và While Trong Java"
date = "2024-12-30"
description = "Hướng dẫn cơ bản về vòng lặp for và while trong Java"
tags = [
"java", "vòng lặp", "lập trình"
]
+++

Vòng lặp trong Java được sử dụng để thực thi một khối lệnh nhiều lần, giúp giảm thiểu việc viết mã lặp đi lặp lại.

<!--more-->

## Vòng Lặp For

### Cú pháp cơ bản của vòng lặp `for`
```java
for (khởi_tạo; điều_kiện; cập_nhật) {
    // Khối lệnh thực thi trong mỗi lần lặp
}
```

Ví dụ:

```java
public class ForLoopExample {
    public static void main(String[] args) {
        for (int i = 1; i <= 5; i++) {
            System.out.println("Giá trị của i: " + i);
        }
    }
}
```

### Vòng lặp lồng nhau
Bạn có thể sử dụng vòng lặp `for` lồng nhau:

```java
for (int i = 1; i <= 3; i++) {
    for (int j = 1; j <= 2; j++) {
        System.out.println("i: " + i + ", j: " + j);
    }
}
```

## Vòng Lặp While

### Cú pháp cơ bản của vòng lặp `while`
```java
while (điều_kiện) {
    // Khối lệnh thực thi khi điều kiện đúng
}
```

Ví dụ:

```java
public class WhileLoopExample {
    public static void main(String[] args) {
        int count = 1;

        while (count <= 5) {
            System.out.println("Đếm: " + count);
            count++;
        }
    }
}
```

### Vòng Lặp Do-While
Vòng lặp `do-while` luôn thực thi ít nhất một lần:

```java
do {
    // Khối lệnh thực thi
} while (điều_kiện);
```

Ví dụ:

```java
public class DoWhileExample {
    public static void main(String[] args) {
        int count = 1;

        do {
            System.out.println("Đếm: " + count);
            count++;
        } while (count <= 5);
    }
}
```

## So Sánh `for`, `while`, và `do-while`

| Vòng Lặp  | Khi nào sử dụng                                                                 |
|-----------|---------------------------------------------------------------------------------|
| `for`     | Khi biết trước số lần lặp                                                      |
| `while`   | Khi không biết trước số lần lặp, nhưng điều kiện kiểm tra phải đúng ngay từ đầu |
| `do-while`| Khi muốn thực thi ít nhất một lần, bất kể điều kiện ban đầu                   |

Hiểu rõ cách sử dụng vòng lặp sẽ giúp bạn tối ưu hóa mã nguồn và giải quyết các bài toán hiệu quả hơn.