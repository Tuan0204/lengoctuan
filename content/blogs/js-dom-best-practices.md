---
title: "DOM Best Practices"
date: 2024-03-20T09:00:00+07:00
draft: false
tags: [javascript, dom]
categories: [JavaScript]
summary: "Thực hành tốt khi thao tác DOM: tránh reflow, batch updates, event delegation"
image: "/images/posts/js-dom.svg"
---

Khi thao tác DOM trực tiếp, hãy chú ý hiệu năng: giảm số lần reflow và repaints.

## Mẹo

- Sử dụng DocumentFragment khi chèn nhiều phần tử
- Sử dụng event delegation thay vì gắn nhiều listener
- Cập nhật class/attribute một lần thay vì nhiều lần

Kết luận: tối ưu thao tác DOM giúp cải thiện trải nghiệm người dùng, đặc biệt trên thiết bị yếu.

Hướng dẫn về truy vấn phần tử, event delegation, batch DOM updates và tránh các anti-pattern gây chậm.