---
title: "Spring Boot REST API cơ bản"
date: 2024-02-01T10:00:00+07:00
draft: false
tags: [java, springboot, rest]
categories: [Java]
summary: "Tạo REST API cơ bản bằng Spring Boot"
image: "/images/posts/java-springboot.svg"
---

Spring Boot giúp khởi tạo ứng dụng web nhanh chóng. Ví dụ controller đơn giản:

```java
@RestController
@RequestMapping("/api/books")
public class BookController {
    @GetMapping
    public List<Book> list() { return List.of(); }
}
```

## Cấu hình

- Sử dụng Spring Initializr để bootstrap project
- Cấu hình application.properties cho port, datasource

## Bảo mật và testing

- Sử dụng Spring Security cho authentication
- Viết unit test với MockMvc

Kết luận: Spring Boot phù hợp cho REST services nhanh chóng và có hệ sinh thái phong phú.

Bước qua việc tạo project, định nghĩa endpoint, kết nối database, và đóng gói ứng dụng để triển khai.