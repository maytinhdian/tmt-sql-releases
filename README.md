# TMT SQL Tool — Releases

**TMT SQL Tool** là công cụ tích hợp dành cho phần mềm **MitaPro V1** và **TicoH+**, hỗ trợ kết nối và tải log chấm công từ các máy chấm công sử dụng firmware mới.

Công cụ chủ động kết nối máy chấm công bằng ZKTeco Standalone SDK, cho phép người dùng xem trước dữ liệu và xác nhận trước khi cập nhật vào cơ sở dữ liệu của phần mềm.

## Tải xuống

Mở trang [Releases](../../releases/latest) để tải phiên bản mới nhất.

Mỗi bản phát hành gồm:

- `TmtSqlTool-<version>-Setup.exe`: bộ cài Windows x86 (khuyến nghị)
- `TmtSqlTool-<version>-win-x86.zip`: bản portable, nếu có
- `SHA256SUMS.txt`: mã SHA-256 để xác minh tính toàn vẹn

Chức năng kiểm tra cập nhật trong phần mềm đọc phiên bản mới nhất trực tiếp từ trang Releases này.

## Xác minh SHA-256

Sau khi tải xuống, mở PowerShell tại thư mục chứa file và chạy (thay `<version>` bằng số phiên bản, ví dụ `1.0.5`):

```powershell
Get-FileHash .\TmtSqlTool-<version>-Setup.exe -Algorithm SHA256
```

Với bản portable:

```powershell
Get-FileHash .\TmtSqlTool-<version>-win-x86.zip -Algorithm SHA256
```

Đối chiếu giá trị `Hash` với dòng tương ứng trong `SHA256SUMS.txt` của cùng bản phát hành (không phân biệt chữ hoa, chữ thường).

## Cảnh báo Windows SmartScreen

Bộ cài hiện chưa có chữ ký số Authenticode nên Windows có thể hiển thị cảnh báo **Unknown publisher**. Chỉ tiếp tục cài đặt khi file được tải từ repository này và mã SHA-256 trùng khớp với bản công bố.

## Bảo mật

Repository này chỉ chứa bản phát hành dành cho khách hàng. Source code, công cụ cấp license, private key, license khách hàng và thông tin kết nối thiết bị/SQL không được công bố tại đây.