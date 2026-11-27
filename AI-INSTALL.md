# 🤖 AI-Executable Installation Guide — `4AppleTV-S`

Tài liệu chuẩn dành cho **AI Assistant / AI Agent** (ChatGPT, Gemini, Claude, Grok, Codex, Antigravity, Cursor) khi người dùng yêu cầu hướng dẫn hoặc tự động cài đặt **4AppleTV-S** (Standalone 1-Slot Self-Signing Apple TV Companion for iPhone/iPad).

- **Kho phân phối công khai:** <https://github.com/hongson117/4AppleTV-S>
- **Hướng dẫn cài không cần PC (iOS 27+ · Open Minis):** [`OPEN-MINIS.md`](https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/OPEN-MINIS.md)
- **Tệp thông tin bản mới nhất:** [`version.json`](https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/version.json)

---

## 1. Phân Nhánh Theo Thiết Bị Của Người Dùng

1. **Hỏi phiên bản iOS / iPadOS của người dùng trước tiên:**
   - **Nếu `iOS / iPadOS 27.0+` (và không muốn dùng máy tính):** Đọc [`OPEN-MINIS.md`](OPEN-MINIS.md) và hướng dẫn từng bước chạy 1 lệnh trong **Open Minis (`1.16+`)**:
     ```sh
     wget -qO- https://raw.githubusercontent.com/hongson117/4AppleTV-S/main/install.sh | sh
     ```
   - **Nếu `iOS / iPadOS 17.0 – 26.x` (ví dụ `18.6.2`) hoặc có sẵn laptop Windows / macOS:** Hướng dẫn hoặc thực thi bộ cài cáp USB 1 lần (`4appletv-s-windows.zip` hoặc `4appletv-s-macos-universal.zip`) theo [`README.md`](README.md).

## 2. Nguyên Tắc Bảo Mật Bắt Buộc Cho AI
- **Tuyệt đối không hỏi mật khẩu Apple ID, mã 2FA, mật khẩu `.p12` hay mã bản quyền `TVS`** trong khung trò chuyện AI. Người dùng chỉ tự gõ vào giao diện cục bộ (`127.0.0.1` của `tvs-boot`, cửa sổ CLI trên máy tính, hoặc trực tiếp trong ứng dụng `4AppleTV-S`).
- **`4AppleTV-S` chỉ chiếm đúng 1 slot Apple ID miễn phí** trên iPhone (không có app phụ Runner1/Runner2). Sau khi cài xong lần đầu, ứng dụng tự gia hạn nhanh ~2 giây qua `LocalDevVPN` (`10.7.0.1`) mà không cần máy tính nữa.
