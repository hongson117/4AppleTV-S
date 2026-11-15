<p align="center">
  <img src="docs/icon.png" width="144" height="144" alt="4AppleTV-S Metallic Gold Icon" />
</p>

<h1 align="center">4AppleTV-S</h1>

<p align="center">
  <strong>Standalone 1-Slot Self-Signing Apple TV Companion & Sideloader for iPhone</strong><br/>
  Phiên bản Vàng Kim độc lập — Cài 1 lần qua USB (Windows / macOS), tự gia hạn ngay trên iPhone, chỉ chiếm đúng 1 slot Apple ID miễn phí.
</p>

---

## 📦 Tải xuống chính thức / Official Downloads (`v1.0.0` Build `1`)

> Kho công khai này chỉ phân phối file cài đặt nhị phân (`.ipa`, bộ cài USB Windows/macOS) và manifest kiểm tra cập nhật (`version.json`, `source.json`, `SHA256SUMS.txt`). Mã nguồn được bảo mật riêng tư.

| Gói tải về / Package | Hệ điều hành | SHA-256 |
|---|---|---|
| [`4AppleTV-S.ipa`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.0.0/4AppleTV-S.ipa) | iOS 17.0+ | `c1547a54cbd443e8ae1a327d803c379fe95451579404ebf264367b094bbb378f` |
| [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.0.0/4appletv-s-windows.zip) | Windows 10/11 (x64) | `dedaa4e42ab8b128d9af118f59d58d544590782dba562e9bc4f028f2a6eae1cc` |
| [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.0.0/4appletv-s-macos-universal.zip) | macOS 11+ (Apple Silicon & Intel) | `51c362e841ccfbdcb088f3ea6de571ea7a9efffca7264f994b96bb5a5aaaff0c` |

- **Release page:** [v1.0.0](https://github.com/hongson117/4AppleTV-S/releases/tag/v1.0.0)
- **AltStore / Feather / SideStore Source (`source.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/source.json`
- **OTA Version Manifest (`version.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/version.json`

---

## 🚀 Hướng dẫn cài đặt 1 lần duy nhất (Tiếng Việt)

### Bước 1 — Cài từ máy tính qua cáp USB (chỉ làm 1 lần)
- **Windows 10/11:** Tải [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.0.0/4appletv-s-windows.zip), giải nén toàn bộ thư mục, cài **Apple Devices** hoặc **iTunes**, cắm iPhone qua USB (Tin cậy máy tính), rồi chạy **`Cai-4AppleTV-S.bat`**.
- **macOS 11+:** Tải [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.0.0/4appletv-s-macos-universal.zip), giải nén, cắm iPhone vào Finder & chọn **Trust**, rồi mở **`Cai-4AppleTV-S.command`**.

Công cụ sẽ tự động ký `4AppleTV-S.ipa` bằng Apple ID của bạn, cài lên iPhone (chiếm **đúng 1 slot** — không cài thêm app phụ), và nạp file ghép đôi Remote Pairing cùng khóa chứng chỉ vào app.

### Bước 2 — Kích hoạt tự gia hạn ngay trên iPhone
1. Cài **LocalDevVPN** miễn phí từ App Store (`id6755608044`).
2. Trên iPhone, tin cậy nhà phát triển tại **Cài đặt → Cài đặt chung → VPN & Quản lý thiết bị** và bật **Chế độ nhà phát triển (Developer Mode)** nếu được hỏi.
3. Mở **4AppleTV-S**:
   - Đăng nhập đúng Apple ID vừa dùng ở Bước 1 trong tab **Account / Tài khoản**.
   - Nhập **mã kích hoạt TVS** để mở khóa đầy đủ điều khiển & sideload Apple TV.
   - Bật **LocalDevVPN** (`10.7.0.1`) bất cứ khi nào muốn app tự gia hạn 7 ngày hoặc cập nhật OTA 1 chạm trực tiếp mà không cần máy tính nữa.

---

## ⚙️ Quick Start (English)

1. **One-time USB setup:** Download [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.0.0/4appletv-s-windows.zip) (Windows) or [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.0.0/4appletv-s-macos-universal.zip) (macOS Universal), extract completely, connect your iPhone over USB, trust the computer, and run the launcher (`Cai-4AppleTV-S.bat` or `Cai-4AppleTV-S.command`).
2. **Standalone 1-Slot Self-Refresh:** Install **LocalDevVPN** (`id6755608044`) from the App Store, sign in with the same Apple ID in **4AppleTV-S → Account**, and activate your **TVS** license key.
3. **No Laptop Required Afterward:** Whenever LocalDevVPN (`10.7.0.1`) is active, **4AppleTV-S** renews its own 7-day certificate and supports verified 1-tap OTA self-updates directly inside the app while occupying only **1 free Apple ID slot**.
