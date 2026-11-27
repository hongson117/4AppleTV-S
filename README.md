<p align="center">
  <img src="docs/icon.png" width="144" height="144" alt="4AppleTV-S Metallic Gold Icon" />
</p>

<h1 align="center">4AppleTV-S</h1>

<p align="center">
  <strong>Standalone 1-Slot Self-Signing Apple TV Companion & Sideloader for iPhone / iPad</strong><br/>
  Phiên bản Vàng Kim độc lập — Cài trực tiếp không cần máy tính qua Open Minis (iOS 27+) hoặc cài 1 lần qua USB (Windows / macOS), tự gia hạn ngay trên iPhone, chỉ chiếm đúng 1 slot Apple ID miễn phí.
</p>

---

## 📦 Tải xuống chính thức / Official Downloads (`v1.1.4` Build `7`)

> Kho công khai này phân phối file cài đặt nhị phân (`.ipa`, bộ cài mồi `tvs-boot-aarch64` cho Open Minis, bộ cài USB Windows/macOS), tài liệu AI Playbook và manifest kiểm tra cập nhật (`version.json`, `source.json`, `SHA256SUMS.txt`). Mã nguồn được bảo mật riêng tư.

| Gói tải về / Package | Hệ điều hành | SHA-256 |
|---|---|---|
| [**Cài 1 lệnh không cần PC (`install.sh` · `OPEN-MINIS.md`)**](OPEN-MINIS.md) | **iOS / iPadOS 27.0+ (Open Minis 1.16+)** | `d73ed2043d349a5713cb99e8afd2068541e62c64955d57db8c92284c843a2789` |
| [`tvs-boot-aarch64`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/tvs-boot-aarch64) | Open Minis Linux `aarch64` static | `fe8bb417a86869896f69d0bc8694e099956601818cebd9f3e83b308b4be93caa` |
| [`4AppleTV-S.ipa`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/4AppleTV-S.ipa) | iOS / iPadOS 17.0+ & 27.0+ | `17895e9046724f00464023cd6c26bd3224811bde0e244744829925212b00c29d` |
| [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/4appletv-s-windows.zip) | Windows 10/11 (x64) | `245e5373a0f7d41e229cea87fa673f9607bbd00eff4e4dbee1068cef45ae66b0` |
| [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/4appletv-s-macos-universal.zip) | macOS 11+ (Apple Silicon & Intel) | `c85ee18af15f368171e985127a8b37a11689a2d1d212c43fa7f66af93458e170` |

- **Release page:** [v1.1.4](https://github.com/hongson117/4AppleTV-S/releases/tag/v1.1.4)
- **Hướng dẫn không cần PC & AI Playbook:** [`OPEN-MINIS.md`](OPEN-MINIS.md) · [`AI-INSTALL.md`](AI-INSTALL.md)
- **AltStore / Feather / SideStore Source (`source.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/source.json`
- **OTA Version Manifest (`version.json`):** `https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/version.json`

### ✨ Điểm mới trong `v1.1.4` (Build `7`)
- **Cài mới 1 lệnh không cần máy tính trên iOS / iPadOS 27+ qua Open Minis (`tvs-boot` + `install.sh`):** Tự ghép nối ngay trên iPhone (`Pair with 4AppleTV-S`), hỗ trợ ký bằng cả **Apple ID cá nhân (chỉ chiếm 1 Slot)** lẫn **Chứng chỉ mua (`.p12` + `.mobileprovision`)**, tự động bàn giao sẵn `pairing.plist`, khóa ký RSA và chứng chỉ vào `/Documents/Storage` của ứng dụng.
- **Nút tự ghép nối lại ngay trong ứng dụng (`Ghép nối ngay trên máy · iOS 27+`):** Cho phép tạo lại `pairing.plist` trong 15 giây trực tiếp tại tab **Tài khoản** của `4AppleTV-S` mà không cần cắm PC hay mở lại Open Minis.
- **Giữ trọn mọi cải tiến từ `v1.1.3`:** Tự nối lại đường hầm Apple TV TLS-PSK, đánh thức Wi-Fi đa IP, đồng bộ 7 ngày với `LiveContainerTV`, chụp màn hình 4K/1080p không dây & tự cập nhật OTA qua `LocalDevVPN` (`10.7.0.1`).

---

## 🚀 Phương Thức 1 (Mới — Không Cần Máy Tính): Cài Trực Tiếp Qua Open Minis (`iOS / iPadOS 27+`)

![Hướng dẫn cài đặt 4AppleTV-S 1 lệnh qua Open Minis](https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/docs/open-minis-install.jpg)

> 🤖 **Nhờ AI cầm tay chỉ việc từng bước:** Sao chép câu dưới đây dán vào **ChatGPT / Gemini / Claude**:  
> `Hãy đọc tài liệu tại https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/OPEN-MINIS.md và hướng dẫn tôi cài đặt 4AppleTV-S trực tiếp trên iPhone/iPad không cần máy tính từng bước một.`  
> *(Xem tài liệu đầy đủ và bảng xử lý lỗi tại [**`OPEN-MINIS.md`**](OPEN-MINIS.md)).*

1. **Chuẩn bị (`iOS / iPadOS 27.0+`):** Bật **Chế độ nhà phát triển** (*Cài đặt → Quyền riêng tư & Bảo mật → Chế độ nhà phát triển*), bật **Wi-Fi** (tạm tắt VPN), rồi tải miễn phí [**Open Minis (`1.16+`)**](https://apps.apple.com/app/id6759188481) và [**LocalDevVPN**](https://apps.apple.com/app/id6755608044) từ App Store.
2. **Chạy 1 lệnh trong Open Minis:** Mở **Open Minis** → chạm biểu tượng **`>_`** góc trên phải → chọn **Shell Terminal**, dán đầy đủ dòng lệnh dưới đây (có cả đuôi `| sh`) rồi nhấn **Enter**:
   ```sh
   wget -qO- https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/install.sh | sh
   ```
   *(Link dự phòng CDN nếu mạng chặn GitHub raw: `wget -qO- https://fastly.jsdelivr.net/gh/hongson117/4AppleTV-S@main/install.sh | sh`)*
3. **Tự ghép nối & Bật LocalDevVPN:** Trên bảng **4AppleTV-S Bootstrap** bật lên (lỡ vuốt đóng thì nhấn `Enter` trong Terminal để mở lại): bấm **Bắt đầu ghép nối** → vào **Cài đặt → Quyền riêng tư & Bảo mật → Chế độ nhà phát triển → `Pair with 4AppleTV-S`** ở cuối trang → nhập mật mã máy + **mã PIN 6 số** trên thông báo → mở **LocalDevVPN** bật **Connect** → quay lại bấm **Tiếp tục**.
4. **Ký 1-Slot & Kích hoạt:** Chọn **Apple ID cá nhân (1-Slot)** hoặc **Chứng chỉ mua (`.p12` + `.mobileprovision`)** để cài thẳng **4AppleTV-S** kèm sẵn `pairing.plist` và khóa ký ra màn hình chính! Tin cậy chứng chỉ (nếu dùng Apple ID miễn phí), mở **4AppleTV-S** đăng nhập cùng Apple ID và nhập **mã kích hoạt TVS** để sử dụng.

---

## 💻 Phương Thức 2: Cài 1 Lần Qua Cáp USB Từ Windows / macOS (`Mọi bản iOS 17.0+ & 27.0+`)

### Bước 1 — Cài từ máy tính qua cáp USB (chỉ làm 1 lần)
- **Windows 10/11:** Tải [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/4appletv-s-windows.zip), giải nén toàn bộ thư mục, cài **Apple Devices** hoặc **iTunes**, cắm iPhone qua USB (Tin cậy máy tính), rồi chạy **`Cai-4AppleTV-S.bat`**.
- **macOS 11+:** Tải [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/4appletv-s-macos-universal.zip), giải nén, cắm iPhone vào Finder & chọn **Trust**, rồi mở **`Cai-4AppleTV-S.command`**.

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

1. **PC-Free On-Device Install (`iOS / iPadOS 27.0+`):** Install **Open Minis (`1.16+`)** and **LocalDevVPN** from the App Store, open **Open Minis → Shell Terminal (`>_`)**, and run:
   ```sh
   wget -qO- https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/install.sh | sh
   ```
   Follow the guided Web UI to self-pair under *Settings › Developer Mode › Pair with 4AppleTV-S*, connect **LocalDevVPN**, and sign with your **Apple ID (1-Slot)** or **Paid Certificate (`.p12`)**.
2. **One-time USB setup (`iOS 17.0+`):** Download [`4appletv-s-windows.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/4appletv-s-windows.zip) (Windows) or [`4appletv-s-macos-universal.zip`](https://github.com/hongson117/4AppleTV-S/releases/download/v1.1.4/4appletv-s-macos-universal.zip) (macOS Universal), extract completely, connect your iPhone over USB, trust the computer, and run `Cai-4AppleTV-S.bat` or `Cai-4AppleTV-S.command`.
3. **Standalone 1-Slot Self-Refresh:** Sign in with the same Apple ID in **4AppleTV-S → Account**, activate your **TVS** license key, and enjoy ~2-second `misagent` 7-day renewals and SHA-256 verified OTA updates via **LocalDevVPN (`10.7.0.1`)** without ever needing a computer again.
