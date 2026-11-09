# daohuyentrang.com: thư mục xuất bản

Website tĩnh (HTML + CSS + JS nhúng sẵn trong từng trang, không cần build, không cần server đặc biệt).
Chép **toàn bộ nội dung thư mục này** (trừ README.md) lên thư mục gốc của hosting, giữ nguyên cấu trúc.

| File | Địa chỉ trên web |
|---|---|
| `index.html` | `/` (trang chủ, tiếng Việt) |
| `en/index.html` | `/en/` (trang chủ, tiếng Anh) |
| `portfolio/index.html` | `/portfolio/` |
| `en/portfolio/index.html` | `/en/portfolio/` |
| `case-study-test/takimobile/index.html` | `/case-study-test/takimobile/` (chỉ gửi link riêng cho client; **không có link từ trang nào**; có `noindex`, không hiện trên Google) |
| `img/` | ảnh dùng chung cho mọi trang, đường dẫn `/img/...` |

## Lưu ý khi upload
- Giữ tên thư mục và tên file `index.html`: các link nội bộ đã trỏ sẵn theo bảng trên (`/`, `/portfolio/`, `/en/`...).
- Phải đặt ở **thư mục gốc của domain** (không để trong thư mục con), vì ảnh gọi theo `/img/...`.
- Mỗi trang đã có khai báo `<!doctype html>`, `lang`, `viewport`, canonical, hreflang VI/EN.
- Không cần nén/minify thêm: hosting tự gzip/brotli. Ảnh đã tối ưu sẵn.
- Phông chữ lấy từ Google Fonts (cần internet khi xem).
- Nếu đổi đường dẫn (ví dụ bỏ `/en/`), tìm và thay trong các file `index.html` các chuỗi `/en/`, `/portfolio/`, `/case-study-test/takimobile/`.
