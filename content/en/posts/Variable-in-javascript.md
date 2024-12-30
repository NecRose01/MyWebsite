+++
author = "Hugo Authors"
title = "Các Phương Thức Cơ Bản Trong JavaScript"
date = "2024-12-30"
description = "Tìm hiểu về các phương thức cơ bản trong JavaScript giúp bạn thao tác với chuỗi, mảng và đối tượng hiệu quả hơn."
tags = [
    "javascript", "phương thức", "lập trình web"
]
+++

JavaScript cung cấp rất nhiều phương thức để thao tác với các kiểu dữ liệu khác nhau, từ chuỗi, mảng đến đối tượng. Việc nắm vững các phương thức cơ bản sẽ giúp bạn viết mã nhanh chóng và hiệu quả hơn.

<!--more-->

### **1. Phương Thức Chuỗi (String Methods)**

JavaScript cung cấp nhiều phương thức hữu ích để làm việc với chuỗi văn bản.

#### `charAt(index)`

Phương thức `charAt()` trả về ký tự tại vị trí chỉ định trong chuỗi.

```javascript
let text = "Hello, World!";
console.log(text.charAt(0)); // Kết quả: "H"
```
#### **toUpperCase()** và **toLowerCase()**
Phương thức toUpperCase() chuyển tất cả ký tự trong chuỗi thành chữ hoa, trong khi toLowerCase() chuyển thành chữ thường.

```javascript
let text = "Hello, World!";
console.log(text.toUpperCase()); // Kết quả: "HELLO, WORLD!"
console.log(text.toLowerCase()); // Kết quả: "hello, world!"
```
#### **substring(start, end)**
Phương thức substring() trả về một phần của chuỗi từ chỉ số start đến chỉ số end (không bao gồm chỉ số end).

```javascript
let text = "Hello, World!";
console.log(text.substring(0, 5)); // Kết quả: "Hello"
```
#### **replace(searchValue, newValue)**
Phương thức replace() thay thế một phần của chuỗi bằng một chuỗi khác.

```javascript
let text = "Hello, World!";
console.log(text.replace("World", "JavaScript")); // Kết quả: "Hello, JavaScript!"
```
### **2. Phương Thức Mảng (Array Methods)**
Mảng là một trong những kiểu dữ liệu quan trọng trong JavaScript, và có rất nhiều phương thức hữu ích để thao tác với mảng.

**push()**
Phương thức push() thêm một hoặc nhiều phần tử vào cuối mảng và trả về độ dài mới của mảng.

```javascript
let arr = [1, 2, 3];
arr.push(4);
console.log(arr); // Kết quả: [1, 2, 3, 4]
```
**pop()**
Phương thức pop() loại bỏ phần tử cuối cùng trong mảng và trả về phần tử đó.

```javascript
let arr = [1, 2, 3];
let lastElement = arr.pop();
console.log(lastElement); // Kết quả: 3
console.log(arr); // Kết quả: [1, 2]
```
**shift()**
Phương thức shift() loại bỏ phần tử đầu tiên trong mảng và trả về phần tử đó.

```javascript
let arr = [1, 2, 3];
let firstElement = arr.shift();
console.log(firstElement); // Kết quả: 1
console.log(arr); // Kết quả: [2, 3]
```
**map()**
Phương thức map() tạo ra một mảng mới bằng cách áp dụng một hàm cho mỗi phần tử trong mảng.

```javascript
let arr = [1, 2, 3];
let newArr = arr.map(x => x * 2);
console.log(newArr); // Kết quả: [2, 4, 6]
```
**filter()**
Phương thức filter() tạo ra một mảng mới chỉ chứa những phần tử thoả mãn điều kiện mà bạn chỉ định.

```javascript
let arr = [1, 2, 3, 4, 5];
let evenNumbers = arr.filter(x => x % 2 === 0);
console.log(evenNumbers); // Kết quả: [2, 4]
```
### **3. Phương Thức Đối Tượng (Object Methods)**
Các đối tượng trong JavaScript cũng có nhiều phương thức hữu ích giúp bạn thao tác với các thuộc tính của đối tượng.

**Object.keys()**
Phương thức Object.keys() trả về một mảng chứa tất cả các khóa (keys) của đối tượng.

```javascript
let obj = { name: "John", age: 30 };
console.log(Object.keys(obj)); // Kết quả: ["name", "age"]
```
**Object.values()**
Phương thức Object.values() trả về một mảng chứa tất cả các giá trị (values) của đối tượng.

```javascript
let obj = { name: "John", age: 30 };
console.log(Object.values(obj)); // Kết quả: ["John", 30]
```
**Object.assign()**
Phương thức Object.assign() sao chép giá trị của tất cả các thuộc tính từ đối tượng nguồn sang đối tượng đích.

```javascript
let obj1 = { name: "John" };
let obj2 = { age: 30 };
let obj3 = Object.assign({}, obj1, obj2);
console.log(obj3); // Kết quả: { name: "John", age: 30 }
```
### **4. Phương Thức Toán Học (Math Methods)**
JavaScript cung cấp một số phương thức toán học hữu ích.

**Math.round()**
Phương thức Math.round() làm tròn số về gần nhất.

```javascript
console.log(Math.round(4.5)); // Kết quả: 5
console.log(Math.round(4.4)); // Kết quả: 4
```
**Math.random()**
Phương thức Math.random() trả về một số ngẫu nhiên trong khoảng từ 0 (bao gồm) đến 1 (không bao gồm).

```javascript
console.log(Math.random()); // Kết quả: một số ngẫu nhiên từ 0 đến 1
```
**Math.max() và Math.min()**
Phương thức Math.max() trả về giá trị lớn nhất trong các tham số, còn Math.min() trả về giá trị nhỏ nhất.

```javascript
console.log(Math.max(1, 2, 3)); // Kết quả: 3
console.log(Math.min(1, 2, 3)); // Kết quả: 1
```
## **Kết luận**
Nắm vững các phương thức cơ bản trong JavaScript sẽ giúp bạn viết mã hiệu quả hơn và dễ dàng thao tác với các kiểu dữ liệu phổ biến như chuỗi, mảng và đối tượng. Hãy thử nghiệm các phương thức này trong các dự án của bạn để cải thiện kỹ năng lập trình JavaScript!x