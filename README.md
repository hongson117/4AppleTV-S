<p align="center">
  <img src="docs/icon.png" width="144" height="144" alt="4AppleTV-S Metallic Gold Icon" />
</p>

<h1 align="center">4AppleTV-S</h1>

<p align="center">
  <strong>Standalone 1-Slot Self-Signing Apple TV Companion & Sideloader for iPhone</strong><br/>
  Phiên bản Vàng Kim độc lập — Cài 1 lần qua USB (Windows / macOS), tự gia hạn ngay trên iPhone, chỉ chiếm đúng 1 slot Apple ID miễn phí.
</p>

---

## 📦 Tải xuống chính thức / Official Downloads (`v1.1.0` Build `3`)

> Kho công khai này chỉ phân phối file cài đặt nhị phân (`.ipa`, bộ cài USB Windows/macOS) và manifest kiểm tra cập nhật (`version.json`, `source.json`, `SHA256SUMS.txt`). Mã nguồn được bảo mật riêng tư.

| Gói tải về / Package | Hệ điều hành | SHA-256 |
|---|---|---|
| [`4AppleTV-S.ipa`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.0/4AppleTV-S.ipa) | iOS 17.0+ | `dd748290d83bf77dcc4e7294eec922a03020b3b1553fa077f351be41941da8cc` |
| [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.0/4appletv-s-windows.zip) | Windows 10/11 (x64) | `1ba385a6742c407e1652ef2f0bf99b1c7012c2e4af16ecb74a75a1f30dec396f` |
| [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.0/4appletv-s-macos-universal.zip) | macOS 11+ (Apple Silicon & Intel) | `32de00494fb090ab8283ad7fa3e0e480b32fe14ba8b94035230382e41853588a` |

- **Release page:** [v1.1.0](https://github.com/hongson117/4AppleTV-S/releases/tag/v1.1.0)
- **AltStore / Feather / SideStore Source (`source.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/source.json`
- **OTA Version Manifest (`version.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/version.json`

### ✨ Điểm mới trong `v1.1.0` (Build `3`)
- **Chụp màn hình Apple TV không dây:** Chụp ảnh 4K/1080p PNG trực tiếp từ Apple TV qua Wi-Fi, xem lại và chia sẻ/lưu vào Ảnh iPhone ngay trong **Kho ảnh chụp Apple TV**.
- **Gia hạn nhanh `misagent` (~2 giây, không cần cài lại `.ipa`):** Tự động làm mới provisioning profile 7 ngày cho cả app trên Apple TV lẫn bản thân `4AppleTV-S` trên iPhone khi không có thay đổi (tự động fallback sang ký & cài đè đầy đủ nếu cần), kèm tự hàn gắn khi ghép đôi lại Apple TV.
- **Tự động cập nhật trong app (cắm dây 1 lần duy nhất):** Tự động kiểm tra khi mở/trở lại app hoặc qua BGTask/Shortcuts, tải ngầm có xác minh SHA-256 và tự cài đè trực tiếp khi có VPN `10.7.0.1` (hoặc cập nhật tự động 1 chạm).

---

## 🚀 Hướng dẫn cài đặt 1 lần duy nhất (Tiếng Việt)

### Bước 1 — Cài từ máy tính qua cáp USB (chỉ làm 1 lần)
- **Windows 10/11:** Tải [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.0/4appletv-s-windows.zip), giải nén toàn bộ thư mục, cài **Apple Devices** hoặc **iTunes**, cắm iPhone qua USB (Tin cậy máy tính), rồi chạy **`Cai-4AppleTV-S.bat`**.
- **macOS 11+:** Tải [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.0/4appletv-s-macos-universal.zip), giải nén, cắm iPhone vào Finder & chọn **Trust**, rồi mở **`Cai-4AppleTV-S.command`**.

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

1. **One-time USB setup:** Download [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.0/4appletv-s-windows.zip) (Windows) or [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.0/4appletv-s-macos-universal.zip) (macOS Universal), extract completely, connect your iPhone over USB, trust the computer, and run the launcher (`Cai-4AppleTV-S.bat` or `Cai-4AppleTV-S.command`).
2. **Standalone 1-Slot Self-Refresh:** Install **LocalDevVPN** (`id6755608044`) from the App Store, sign in with the same Apple ID in **4AppleTV-S → Account** (automatically matches across up to 3 signed-in Apple IDs), and activate your **TVS** license key.
3. **No Laptop Required Afterward:** Whenever LocalDevVPN (`10.7.0.1`) is active, **4AppleTV-S** performs ~2-second `misagent` fast 7-day renewals and automatic SHA-256 verified in-app OTA updates while occupying only **1 free Apple ID slot**, plus wireless Apple TV screenshots and TV app fast-refresh.
