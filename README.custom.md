<!--
  README for the custom fork of Termora.
  For the original project see: https://www.termora.app
-->

# Termora Custom

A Windows‑focused custom build of the open‑source **[Termora](https://www.termora.app)** ([plugins](https://www.termora.app/plugins)) terminal & file‑transfer app.

The upstream Termora is fully preserved. This fork only **adds** the features listed below.

> 🇻🇳 Bản tiếng Việt bên dưới.

---

## ✨ What this fork adds

- **In‑process RDP embedding** — RDP tabs are hosted inside Termora itself; Termora no longer freezes when multiple RDP sessions are open, and login is automatic.
- **RDP Reconnect button** — when a session drops (e.g. server idle timeout), a *Reconnect* button appears in the middle of the tab.
- **Custom session icons** — pick from a set of OS logos (Windows / Linux / Ubuntu / Debian / Fedora / AlmaLinux…) or colored symbols; **works for folders too**; bulk‑apply to many hosts at once. Tab icons follow the session icon.
- **Duplicate‑tab prevention** — opening a host that is already open just switches to the existing tab and notifies you.
- **Security bundle**
  - **PIN + Auto‑lock** (idle timer, *Lock now* button).
  - **Master password** that encrypts saved passwords / SSH private keys / proxy passwords with AES‑256‑GCM; unlock prompt on startup.
  - **Auto‑clear clipboard** after copying secrets (30 s).
  - **Early cleanup** of the Windows Credential Manager `TERMSRV/…` entry as soon as RDP is connected.
- **Two‑way SFTP drag & drop**
  - **Explorer → remote panel** — drop anywhere in the remote pane (works on empty folders too).
  - **Remote panel → Explorer / Desktop** — download starts as soon as you begin dragging.
- **Export / Import sessions** — one `.termora` file (optionally passphrase‑protected) contains all hosts, folders, SSH keys and tags for moving to another machine.
- **PuTTY `.ppk` private keys** — imported directly in the Key Manager (v2 & v3, with or without passphrase).
- **Search box on the sidebar** — filter sessions live by name / host / username / remark; ↑↓ to select, Enter to open.

---

## 📥 Get it running

- **Installer** (recommended): `termora-custom.exe`
- **Portable ZIP**: extract and run `Termora.exe`

Requires Windows 10/11 x64. No Java install needed (JRE is bundled).

App data is stored under `%USERPROFILE%\.termora`. For a **true portable** setup, create an empty folder named `data` next to `Termora.exe` — all data will then live inside the app folder.

---

## 🏷 Attribution

Based on the excellent open‑source **[Termora](https://www.termora.app)** project — all core terminal, SSH/SFTP, transfer, plugin and UI features are the work of the upstream authors and contributors.

Please respect the upstream license (see [`LICENSE`](LICENSE) and [`THIRDPARTY`](THIRDPARTY)). Changes in this fork are shared under the same license unless a file states otherwise.

- Upstream project: https://www.termora.app
- Upstream plugins: https://www.termora.app/plugins

## Download: 
https://drive.google.com/drive/folders/1zCRUIKqL8WhTRi2vzx9SchWXnYXoGufL?usp=drive_link
---
---

# Termora Custom

Bản Windows tuỳ biến dựa trên phần mềm mã nguồn mở **[Termora](https://www.termora.app)** ([danh sách plugin](https://www.termora.app/plugins)) — terminal & truyền file đa giao thức.

Toàn bộ tính năng của Termora gốc được giữ nguyên. Bản này chỉ **bổ sung thêm** các tính năng dưới đây.

## ✨ Tính năng cải tiến

- **Nhúng RDP trong tiến trình** — tab RDP chạy ngay trong Termora, mở nhiều phiên RDP không còn treo, tự đăng nhập.
- **Nút Reconnect cho RDP** — khi phiên bị ngắt (idle timeout…), hiện nút *Reconnect* ở giữa tab để kết nối lại.
- **Icon phiên tuỳ chỉnh** — chọn từ bộ icon OS (Windows / Linux / Ubuntu / Debian / Fedora / AlmaLinux…) hoặc icon đơn sắc có màu tuỳ ý; **áp dụng được cho cả folder**; đổi hàng loạt cho nhiều host cùng lúc. Icon tab đồng bộ theo icon session.
- **Chống mở trùng tab** — mở host đã có tab sẽ chuyển sang tab đó và thông báo thay vì mở phiên mới.
- **Bộ tính năng bảo mật**
  - **PIN + Auto‑lock** (khoá khi idle, nút *Lock now*).
  - **Master password** mã hoá mật khẩu / SSH private key / mật khẩu proxy bằng AES‑256‑GCM; hỏi khi mở app.
  - **Tự xoá clipboard** sau khi copy secret (30 giây).
  - **Dọn credential `TERMSRV/…`** ngay khi phiên RDP kết nối thành công.
- **Kéo/thả 2 chiều SFTP**
  - **Explorer → panel remote** — thả vào bất kỳ vị trí nào của pane remote (kể cả folder rỗng).
  - **Panel remote → Explorer / Desktop** — tải xuống ngay khi bắt đầu kéo.
- **Export / Import phiên** — một file `.termora` (có thể đặt mật khẩu) chứa toàn bộ host, folder, SSH key và tag để chuyển sang máy khác.
- **Hỗ trợ private key PuTTY `.ppk`** — nhập trực tiếp trong Key Manager (v2/v3, có/không passphrase).
- **Thanh tìm kiếm ở sidebar** — lọc phiên theo tên / host / username / remark ngay khi gõ; ↑↓ để chọn, Enter để mở.

## 📥 Cài đặt

- **Installer** (khuyến nghị): `termora-custom.exe`
- **Portable ZIP**: giải nén và chạy `Termora.exe`

Yêu cầu Windows 10/11 x64. Không cần cài Java (JRE đã được đóng kèm).

Dữ liệu app lưu tại `%USERPROFILE%\.termora`. Muốn **portable thật sự** (dữ liệu đi kèm folder app), tạo thư mục rỗng tên `data` cạnh `Termora.exe` — mọi thứ sẽ được lưu bên trong folder app.

## 🏷 Đóng góp

Dựa trên dự án mã nguồn mở **[Termora](https://www.termora.app)** — toàn bộ phần lõi terminal, SSH/SFTP, truyền file, plugin và UI đều là công sức của các tác giả và cộng đồng upstream.

Vui lòng tuân thủ license upstream (xem [`LICENSE`](LICENSE) và [`THIRDPARTY`](THIRDPARTY)). Các thay đổi trong bản này chia sẻ theo cùng license, trừ khi file cụ thể ghi khác.

## Download: 
https://drive.google.com/drive/folders/1zCRUIKqL8WhTRi2vzx9SchWXnYXoGufL?usp=drive_link