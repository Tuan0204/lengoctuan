---
title: "Xử lý ngoại lệ trong Java"
date: 2024-01-15T11:00:00+07:00
draft: false
tags: [java, exceptions]
categories: [Java]
summary: "Cách dùng try/catch/finally và custom exceptions trong Java"
image: "/images/posts/java-exceptions.svg"
---

Xử lý ngoại lệ giúp chương trình an toàn hơn và dễ gỡ lỗi. Sử dụng try/catch để bắt và xử lý lỗi, finally để giải phóng tài nguyên.

```java
try (BufferedReader br = new BufferedReader(new FileReader(path))) {
    // đọc file
} catch (IOException e) {
    e.printStackTrace();
}
```

Bạn có thể định nghĩa custom exception bằng cách kế thừa Exception hoặc RuntimeException.

## Lời khuyên

- Bắt các exception cụ thể thay vì Exception chung chung
- Sử dụng try-with-resources để tự động đóng tài nguyên

Kết luận: xử lý ngoại lệ tốt cải thiện độ tin cậy của ứng dụng.