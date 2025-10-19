---
title: "Java Streams API"
date: 2024-01-10T09:00:00+07:00
draft: false
tags: [java, streams]
categories: [Java]
summary: "Sử dụng Streams để xử lý dữ liệu theo phong cách chức năng trong Java"
image: "/images/posts/java-streams.svg"
---

Java Streams API cho phép xử lý tập hợp dữ liệu theo cách khai báo và có thể tận dụng song song (parallel).

## Khởi tạo Stream

```java
List<String> items = List.of("apple","banana","cherry");
items.stream()
	.filter(s -> s.length() > 5)
	.map(String::toUpperCase)
	.forEach(System.out::println);
```

## Các operation chính

- intermediate: map, filter, sorted
- terminal: collect, forEach, reduce

## Lời khuyên

- Tránh trạng thái bên ngoài khi dùng stream
- Sử dụng parallelStream cẩn trọng

Kết hợp Streams với Optional và collectors sẽ giúp mã ngắn gọn và dễ đọc.

Bài viết mô tả cách sử dụng Streams để filter, map, reduce, và xử lý song song dữ liệu một cách hiệu quả.