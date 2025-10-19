---
title: "Testing JavaScript với Jest"
date: 2024-04-10T09:00:00+07:00
draft: false
tags: [javascript, testing, jest]
categories: [JavaScript]
summary: "Hướng dẫn cơ bản viết unit test với Jest"
image: "/images/posts/js-jest.svg"
---

Jest là framework test phổ biến cho JavaScript, dễ cấu hình và tích hợp với CI.

## Ví dụ test

```js

Jest là framework test phổ biến cho JavaScript, dễ cấu hình và tích hợp với CI.

## Ví dụ test

```js
test('sum', () => {
	expect(1 + 2).toBe(3);
});
```

## Lời khuyên

- Viết test nhỏ, độc lập
- Mock dependencies khi cần

Kết luận: thêm test giúp phát hiện lỗi sớm và tăng độ tin cậy phần mềm.