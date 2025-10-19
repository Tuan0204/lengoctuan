---
title: "Async / Await trong JavaScript"
date: 2024-03-10T09:00:00+07:00
draft: false
tags: [javascript, async]
categories: [JavaScript]
summary: "Sử dụng async/await để làm việc với Promise một cách tuần tự và rõ ràng"
image: "/images/posts/js-async-await.svg"
---

Async/await giúp viết mã bất đồng bộ trông như đồng bộ, làm cho luồng xử lý dễ hiểu hơn.

```js
async function fetchData() {
  ---
  title: "Async / Await trong JavaScript"
  date: 2024-03-10T09:00:00+07:00
  draft: false
  tags: [javascript, async]
  categories: [JavaScript]
  summary: "Sử dụng async/await để làm việc với Promise một cách tuần tự và rõ ràng"
  image: "/images/posts/js-async-await.svg"
  ---

  Async/await giúp viết mã bất đồng bộ trông như đồng bộ, làm cho luồng xử lý dễ hiểu hơn.

  ```js
  async function fetchData() {
    try {
      const res = await fetch('/api/data');
      const json = await res.json();
      return json;
    } catch (e) {
      console.error(e);
    }
  }
  ```

  ## Lưu ý

  - Luôn bắt lỗi với try/catch
  - Tránh chạy nhiều await tuần tự nếu có thể dùng Promise.all

  Kết luận: async/await là công cụ mạnh cho mã bất đồng bộ, nhưng cần chú ý hiệu năng khi chạy tuần tự.