# ban84vn.com

BẢN84 — kênh phân tích & góc nhìn về kinh tế, chính sách và AI ứng dụng cho người trẻ Việt Nam. Không phải cơ quan báo chí.

Trang tĩnh, phát hành qua GitHub Pages tại **https://ban84vn.com** (tên miền đặt qua tệp `CNAME`). Không cần hosting hay cơ sở dữ liệu:
video nhúng từ Fanpage BẢN84, tìm kiếm chạy trong trình duyệt từ `data/search.json`.

## DNS (Squarespace Domains)
- `@` A → 185.199.108.153 · 185.199.109.153 · 185.199.110.153 · 185.199.111.153
- `www` CNAME → ban84vn.github.io
- Giữ nguyên MX `smtp.google.com` và TXT SPF của Google Workspace (email Infor@ban84vn.com).

## Cấu trúc
- `index.html`, `video.html`, `chu-de/*.html` — trang chủ, video, chủ đề
- `bai/<slug>.html` — mỗi bài: ảnh dẫn (Pexels, ghi tác giả), video, điểm chính, câu hỏi mở, toàn văn, số liệu đã kiểm & nguồn, chia sẻ
- `gioi-thieu.html`, `nguyen-tac.html` — về BẢN84; nguyên tắc nội dung & đính chính
- `tim-kiem.html` + `data/search.json` — tìm kiếm; `data/posts.json` — dữ liệu bài
- `feed.xml` (RSS), `sitemap.xml`, `robots.txt`, `manifest.webmanifest`, `404.html`
- `img/cover` (ảnh bìa 1200×675, `s/` = 640w), `img/photo` (ảnh dẫn 1600×900, `s/` = 800w), icon & OG mặc định

## Thêm bài mới
Trang được sinh bằng `news/build.py` (trong kho dựng của BẢN84) từ `published.json` + `stories/<key>.json` + `photos/photos.json`.
Thêm bài = thêm story đã phát + chọn ảnh Pexels (id, tác giả) → chạy `python3 build.py` → tải thư mục `out/` lên đây.
