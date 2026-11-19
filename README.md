<p align="center">
  <img src="docs/icon.png" width="144" height="144" alt="4AppleTV-S Metallic Gold Icon" />
</p>

<h1 align="center">4AppleTV-S</h1>

<p align="center">
  <strong>Standalone 1-Slot Self-Signing Apple TV Companion & Sideloader for iPhone</strong><br/>
  Phiên bản Vàng Kim độc lập — Cài 1 lần qua USB (Windows / macOS), tự gia hạn ngay trên iPhone, chỉ chiếm đúng 1 slot Apple ID miễn phí.
</p>

---

## 📦 Tải xuống chính thức / Official Downloads (`v1.1.2` Build `5`)

> Kho công khai này chỉ phân phối file cài đặt nhị phân (`.ipa`, bộ cài USB Windows/macOS) và manifest kiểm tra cập nhật (`version.json`, `source.json`, `SHA256SUMS.txt`). Mã nguồn được bảo mật riêng tư.

| Gói tải về / Package | Hệ điều hành | SHA-256 |
|---|---|---|
| [`4AppleTV-S.ipa`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.2/4AppleTV-S.ipa) | iOS 17.0+ | `9a6a71642ba62a2ebdad48a3f00a4a0f3f69a5ff6e49523b04fa6dcb07841f6e` |
| [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.2/4appletv-s-windows.zip) | Windows 10/11 (x64) | `8a420db15a114be0c421260f5854a187bad3107af8aa288d2bc3c06e53e5d2cc` |
| [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.2/4appletv-s-macos-universal.zip) | macOS 11+ (Apple Silicon & Intel) | `3c16da0989d7007453823c51858ec58003e09f6b96fab9b31b4c73a75250bdae` |

- **Release page:** [v1.1.2](https://github.com/hongson117/4AppleTV-S/releases/tag/v1.1.2)
- **AltStore / Feather / SideStore Source (`source.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/source.json`
- **OTA Version Manifest (`version.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/version.json`

### ✨ Điểm mới trong `v1.1.2` (Build `5`)
- **Sửa dứt điểm lỗi cập nhật ứng dụng Apple TV & `LiveContainerTV` báo thành công nhưng vẫn giữ phiên bản cũ:** Khi cài/nâng cấp gói `.ipa` có version hoặc build khác bản đang cài trên TV, `4AppleTV-S` ép cài đè đầy đủ (chỉ dùng gia hạn nhanh `misagent` ~2 giây khi gia hạn 7 ngày cùng phiên bản).
- **Đồng bộ chính xác 7 ngày với `LiveContainerTV`:** Đẩy hồ sơ `.mobileprovision` qua `HouseArrest` (ngay cả khi app TV đang đóng) và cổng `:8228` (`/api/v1/sync-expiry`), kèm tự động chữa lệch ngày cũ khi kết nối lại.
- **Chụp màn hình Apple TV không dây & tự động cập nhật trong app:** Hỗ trợ chụp 4K/1080p PNG qua Wi-Fi, gia hạn nhanh `misagent` cho cả app TV & `4AppleTV-S`, tự cập nhật OTA qua LocalDevVPN `10.7.0.1` (cắm USB 1 lần duy nhất).

---

## 🚀 Hướng dẫn cài đặt 1 lần duy nhất (Tiếng Việt)

### Bước 1 — Cài từ máy tính qua cáp USB (chỉ làm 1 lần)
- **Windows 10/11:** Tải [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.2/4appletv-s-windows.zip), giải nén toàn bộ thư mục, cài **Apple Devices** hoặc **iTunes**, cắm iPhone qua USB (Tin cậy máy tính), rồi chạy **`Cai-4AppleTV-S.bat`**.
- **macOS 11+:** Tải [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.2/4appletv-s-macos-universal.zip), giải nén, cắm iPhone vào Finder & chọn **Trust**, rồi mở **`Cai-4AppleTV-S.command`**.

Công cụ sẽ tự động ký `4AppleTV-S.ipa` bằng Apple ID của bạn, cài lên iPhone (chiếm **đúng 1 slot** — không cài thêm app phụ), và nạp file ghép đôi Remote Pairing cùng khóa chứng chỉ vào app.

### Bước 2 — Kích hoạt tự gia hạn & cập nhật OTA ngay trên iPhone
1. Cài **LocalDevVPN** miễn phí từ App Store (`id6755608044`).
2. Trên iPhone, tin cậy nhà phát triển tại **Cài đặt → Cài đặt chung → VPN & Quản lý thiết bị** và bật **Chế độ nhà phát triển (Developer Mode)** nếu được hỏi.
3. Mở **4AppleTV-S**:
   - Đăng nhập đúng Apple ID vừa dùng ở Bước 1 trong tab **Account / Tài khoản** (hỗ trợ tự dò trong tối đa 3 Apple ID đã đăng nhập).
   - Nhập **mã kích hoạt TVS** để mở khóa đầy đủ điều khiển, chụp màn hình & sideload Apple TV.
   - Bật **LocalDevVPN** (`10.7.0.1`) bất cứ khi nào muốn app tự gia hạn nhanh 7 ngày hoặc tự động cập nhật OTA ngay trong app mà không cần cắm máy tính nữa.

---

## ⚙️ Quick Start (English)

1. **One-time USB setup:** Download [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.2/4appletv-s-windows.zip) (Windows) or [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.2/4appletv-s-macos-universal.zip) (macOS Universal), extract completely, connect your iPhone over USB, trust the computer, and run the launcher (`Cai-4AppleTV-S.bat` or `Cai-4AppleTV-S.command`).
2. **Standalone 1-Slot Self-Refresh:** Install **LocalDevVPN** (`id6755608044`) from the App Store, sign in with the same Apple ID in **4AppleTV-S → Account** (automatically matches across up to 3 signed-in Apple IDs), and activate your **TVS** license key.
3. **No Laptop Required Afterward:** Whenever LocalDevVPN (`10.7.0.1`) is active, **4AppleTV-S** performs ~2-second `misagent` fast 7-day renewals and automatic SHA-256 verified in-app OTA updates while occupying only **1 free Apple ID slot**, plus wireless Apple TV screenshots and TV app fast-refresh.
