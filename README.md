# Luyện Gõ Phím - bản cài máy tính

Repo này **chỉ chứa bản phát hành** (Releases) của Luyện Gõ Phím, một sản phẩm của [tsudev](https://tsudev.com).
Mã nguồn được phát triển ở repo riêng. Mọi tệp ở đây sinh tự động, đừng mở PR sửa tay.

- Chơi ngay trên trình duyệt, không cần cài: https://luyen-go-phim.tsudev.com
- Luyện gõ phím ngoại tuyến: đo WPM, độ chính xác, theo dõi tiến bộ. Dữ liệu chỉ nằm trên máy của bạn.

## Tải về

Vào mục [Releases](../../releases/latest):

| Hệ điều hành | Tệp |
| --- | --- |
| Windows 10/11 (x64) | `…-windows-x86-64-setup.exe` (bộ cài) hoặc `…-windows-x86-64.zip` (chạy liền, không cài) |
| Linux x64 | `…-linux-x86-64.AppImage` (chạy liền) hoặc `…-linux-x86-64.tar.gz` |

Ubuntu, Debian và Fedora có thể cài qua kho `pkg.tsudev.com` khi gói đã lên kho (xem [tsudev.com/apps](https://tsudev.com/apps)).

## Kiểm tra tệp tải về

Mỗi bản phát hành có `SHA256SUMS.txt`:

```bash
sha256sum -c SHA256SUMS.txt --ignore-missing
```

Windows (PowerShell): `Get-FileHash .\tệp.exe -Algorithm SHA256`, rồi so với dòng tương ứng.

Bản Windows chưa ký Authenticode nên SmartScreen có thể cảnh báo "Windows protected your PC". Hãy kiểm SHA-256
trước, rồi chọn **More info -> Run anyway**.

## Bảo mật và liên hệ

Báo lỗ hổng bảo mật: https://tsudev.com (mục Liên hệ). Đừng đăng chi tiết lỗ hổng công khai.

`packaging/package.json` là tệp khai báo gói (tên gói, tệp, phụ thuộc), dùng cho kho `pkg.tsudev.com`. Giấy phép: [MIT](LICENSE).
