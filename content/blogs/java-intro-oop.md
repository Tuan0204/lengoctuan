---
title: "Giới thiệu OOP trong Java"
date: 2024-01-02T10:00:00+07:00
draft: false
tags: [java, oop]
categories: [Java]
summary: "Những khái niệm cơ bản về lập trình hướng đối tượng trong Java"
image: "/images/posts/java-oop.svg"
---

Java là một ngôn ngữ hướng đối tượng (OOP) mạnh mẽ. Trong bài viết này chúng ta sẽ điểm qua 4 nguyên tắc chính của OOP và cách áp dụng chúng trong Java.

## 1. Lớp và đối tượng

Lớp (class) là khuôn mẫu, đối tượng (object) là thể hiện cụ thể của lớp. Ví dụ:

```java
---
title: "Giới thiệu OOP trong Java"
date: 2024-01-02T10:00:00+07:00
draft: false
tags: [java, oop]
categories: [Java]
summary: "Những khái niệm cơ bản về lập trình hướng đối tượng trong Java"
image: "/images/posts/java-oop.svg"
---

Java là một ngôn ngữ hướng đối tượng (OOP) mạnh mẽ. Trong bài viết này chúng ta sẽ điểm qua 4 nguyên tắc chính của OOP và cách áp dụng chúng trong Java.

## 1. Lớp và đối tượng

Lớp (class) là khuôn mẫu, đối tượng (object) là thể hiện cụ thể của lớp. Ví dụ:

```java
public class Person {
	private String name;

	public Person(String name) {
		this.name = name;
	}

	public String getName() {
		return name;
	}
}
```

## 2. Tính đóng gói (Encapsulation)

Ẩn dữ liệu bên trong lớp và cung cấp phương thức truy cập (getter/setter) để bảo vệ trạng thái.

---
title: "Giới thiệu OOP trong Java"
date: 2024-01-02T10:00:00+07:00
draft: false
tags: [java, oop]
categories: [Java]
summary: "Những khái niệm cơ bản về lập trình hướng đối tượng trong Java"
image: "/images/posts/java-oop.svg"
---

Java là một ngôn ngữ hướng đối tượng (OOP) mạnh mẽ. Trong bài viết này chúng ta sẽ điểm qua 4 nguyên tắc chính của OOP và cách áp dụng chúng trong Java.

## 1. Lớp và đối tượng

Lớp (class) là khuôn mẫu, đối tượng (object) là thể hiện cụ thể của lớp. Ví dụ:

```java
public class Person {
	private String name;

	public Person(String name) {
		this.name = name;
	}

	public String getName() {
		return name;
	}
}
```

## 2. Tính đóng gói (Encapsulation)

Ẩn dữ liệu bên trong lớp và cung cấp phương thức truy cập (getter/setter) để bảo vệ trạng thái.

## 3. Kế thừa (Inheritance)

Cho phép một lớp con kế thừa thuộc tính và phương thức từ lớp cha, giúp tái sử dụng mã.

## 4. Đa hình (Polymorphism)

Cho phép sử dụng cùng một interface với nhiều kiểu đối tượng khác nhau.

## Kết luận

Bắt đầu với ví dụ nhỏ, sau đó mở rộng bằng các bài tập thực tế để nắm vững OOP trong Java.