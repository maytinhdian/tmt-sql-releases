# MitaproSql Tool — Releases

Đây là repository công khai dùng để phân phối các bản phát hành chính thức của **MitaproSql Tool**.

## Tải xuống

Mở trang [Releases](../../releases/latest) để tải phiên bản mới nhất.

Mỗi bản phát hành dự kiến gồm:

- Bộ cài Windows x86 (`.exe`)
- Gói portable (`.zip`) nếu có
- `latest.json` dành cho chức năng kiểm tra cập nhật
- `SHA256SUMS.txt` để xác minh tính toàn vẹn

## Xác minh SHA-256

Sau khi tải xuống, mở PowerShell tại thư mục chứa file và chạy:

```powershell
Get-FileHash .\TmtSqlTool-Setup-<version>.exe -Algorithm SHA256
```

Đối chiếu kết quả với `SHA256SUMS.txt` trong cùng bản phát hành.

## Cảnh báo Windows SmartScreen

Bộ cài hiện chưa có chữ ký số Authenticode nên Windows có thể hiển thị cảnh báo **Unknown publisher**. Chỉ tiếp tục cài đặt khi file được tải từ repository này và mã SHA-256 trùng khớp với bản công bố.

## Bảo mật

Repository này chỉ chứa bản phát hành dành cho khách hàng. Source code, công cụ cấp license, private key, license khách hàng và thông tin kết nối thiết bị/SQL không được công bố tại đây.