# ban84.vn — trang web BẢN84

Trang tĩnh (HTML + ảnh), không cần máy chủ. Thư mục này có thể đưa thẳng lên GitHub Pages, Netlify, Vercel, Cloudflare Pages hoặc bất kỳ hosting nào.

## Cách 1 · GitHub Pages (miễn phí, có HTTPS)
1. Tạo repo mới trên GitHub (ví dụ `ban84.vn`), chọn Public.
2. Tải toàn bộ thư mục này lên nhánh `main` (index.html, CNAME, img/).
3. Settings → Pages → Build and deployment: Source = Deploy from a branch, Branch = main / (root) → Save.
4. Settings → Pages → Custom domain: nhập `ban84.vn` → Save → bật "Enforce HTTPS" (sau khi DNS đã trỏ xong, GitHub cấp chứng chỉ trong vài phút đến vài giờ).

## DNS tại nhà đăng ký tên miền (.vn)
| Loại  | Tên  | Giá trị                     |
|-------|------|-----------------------------|
| A     | @    | 185.199.108.153             |
| A     | @    | 185.199.109.153             |
| A     | @    | 185.199.110.153             |
| A     | @    | 185.199.111.153             |
| CNAME | www  | `<tên-github>.github.io`    |

Email đang dùng (@ban84vn.com) không bị ảnh hưởng vì nằm ở tên miền khác.

## Cách 2 · Netlify / Vercel / Cloudflare Pages
Kéo thả thư mục này vào trang deploy của dịch vụ, rồi thêm tên miền `ban84.vn` theo hướng dẫn của dịch vụ (họ sẽ cho bản ghi DNS tương ứng).
