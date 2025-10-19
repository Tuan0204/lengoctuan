Hướng dẫn triển khai Blog (Hugo)

Tài liệu này hướng dẫn hai cách phổ biến để triển khai site Hugo của bạn: GitHub Pages (với GitHub Actions) và Netlify.

1) GitHub Pages (CI: GitHub Actions)

- Yêu cầu:
  - Repo trên GitHub (đã push code từ local lên GitHub)
  - Workflow đã có trong `.github/workflows/deploy.yml` (đã nằm trong repo này)

- Hoạt động:
  - Khi bạn push lên nhánh `master`, GitHub Actions sẽ chạy, build site bằng Hugo và deploy thư mục `public/` lên nhánh `gh-pages`.
  - GitHub Pages có thể cấu hình để phục vụ nội dung từ nhánh `gh-pages` (Pages -> Build and deployment -> Deployment branch).

- Các bước nhanh:
  1. Push repo lên GitHub (ví dụ: `origin` remote)
     - git add .
     - git commit -m "Prepare deploy"
     - git push origin master
  2. Trên repository settings (GitHub): Settings -> Pages -> Source -> Chọn `gh-pages` branch (root)
  3. Sau khi Actions chạy xong, trang sẽ có sẵn tại `https://<username>.github.io/<repo>` hoặc custom domain nếu bạn cấu hình.

2) Netlify

- Cách nhanh:
  - Đăng nhập vào Netlify và chọn "New site from Git" -> Kết nối Git provider -> Chọn repo -> Build command: `hugo --minify` -> Publish directory: `public`
  - (Tùy chọn) thêm file `netlify.toml` trong repo để cấu hình build và redirect.

- Ví dụ `netlify.toml` (mẫu có sẵn trong repo): xem `netlify.toml`.

3) Preview local

- Cài Hugo trên máy và chạy local server để kiểm tra trước khi deploy:
  - Hugo (Windows): tải binary Hugo Extended hoặc dùng choco: `choco install hugo-extended -y`
  - Chạy local:
    - hugo server -D

4) Ghi chú và khắc phục lỗi

- Nếu Actions không chạy, kiểm tra:
  - Workflow có trong `.github/workflows/deploy.yml` và đã được push
  - Không có lỗi build (xem tab Actions để biết log)
- Nếu site trống: kiểm tra `baseURL` trong cấu hình `hugo.yaml` hoặc `config.*`.

Liên hệ nếu bạn muốn mình cấu hình thêm cho domain tùy chỉnh hoặc Netlify redirect rules.
