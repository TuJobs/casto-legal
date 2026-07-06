# Casto — Trang pháp lý (legal site)

Thư mục này là **repo git RIÊNG** (`TuJobs/casto-legal`), tự động deploy lên
**https://casto-legal.netlify.app/** (Netlify theo dõi GitHub repo này — KHÔNG phải repo app).

> Được `.gitignore` khỏi repo app (`/legal/`) nên không lồng repo. Đổi vị trí thư mục
> trên máy không ảnh hưởng deploy — Netlify chỉ theo GitHub remote.

## Sửa & deploy (3 bước)

1. Sửa file `.html` / `style.css` ngay trong thư mục này.
2. Xem thử: `npm run legal:open` (hoặc mở file `.html` bằng trình duyệt).
3. Deploy: từ gốc project chạy
   ```bash
   npm run legal:deploy -- "mô tả thay đổi"
   ```
   → commit + push nhánh `main` → Netlify build ~1–2 phút.

Lệnh phụ: `npm run legal:status` (xem thay đổi chưa deploy).

## Các trang & URL

| File | URL |
|---|---|
| `index.html` | https://casto-legal.netlify.app/ |
| `privacy.html` | https://casto-legal.netlify.app/privacy.html |
| `terms.html` | https://casto-legal.netlify.app/terms.html |
| `delete-account.html` | https://casto-legal.netlify.app/delete-account.html |

Các URL này được khai trong **App Store Connect** và **Google Play Console**
(Privacy policy + Delete account URL).

## Lưu ý

- Mọi trang dùng chung `style.css`.
- `docs/*.html` trong repo app chỉ là **bản copy cũ, KHÔNG deploy** — luôn sửa ở ĐÂY.
- Đơn vị vận hành ghi trong nội dung: **Nguyễn Văn Tú** · email `casto.support@gmail.com`.
