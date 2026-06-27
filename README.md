# 🏭 Avielora · Tính giá sản xuất & Quyết định Launching

> 🔗 **Demo chạy thật (GitHub Pages):** https://ngoclinh272005-dotcom.github.io/BTVN-Claude-B1-Linh/

Mini tool web giúp **so sánh giá sản xuất từ nhiều NSX (nhà sản xuất) ở MOQ 20 / 100**, đối chiếu với **giá sản xuất mong muốn** (suy ra từ giá brand gốc), và đưa ra **quyết định có nên launch sản phẩm hay không**.

Giao diện theo brand **Avielora**: font Lora (heading) + Inter (body), màu chủ đạo `#321646`, logo ở đầu trang.

## ✨ Tính năng

**1. Thông số sản phẩm**
- Giá brand gốc (USD), giá vải (RMB, nhập tay), tỉ giá USD→RMB (mặc định 7.2).
- Tự tính **Giá sản xuất mong muốn** làm ngưỡng mục tiêu để đối chiếu (hiển thị RMB & USD).

**2. Báo giá NSX**
- Mỗi NSX nhập: tên, giá công may @MOQ 20, giá công may @MOQ 100.
- Tự tính **Giá SX tổng** cho cả mức MOQ thấp và cao.

**3. Bảng so sánh & quyết định** (so sánh ở mức MOQ cao)
- Hiển thị giá SX tổng (RMB & USD), giá mong muốn và **chênh lệch** so với ngưỡng mục tiêu.
- Tự gắn nhãn quyết định **🟢 Nên launch / 🟡 Cân nhắc / 🔴 Chưa nên launch**.
- Banner tự highlight phương án tốt nhất, và cột **"Chọn SX"** để bạn chốt NSX sẽ sản xuất.

Có lưu dữ liệu (`localStorage`), xuất **CSV**, và nút dữ liệu mẫu.

## 🚀 Cách dùng

Không cần cài đặt hay hosting. Mở file **`index.html`** bằng trình duyệt là chạy. Bấm **"Dùng dữ liệu mẫu"** để xem ví dụ ngay.

## 🛠️ Công nghệ

HTML + CSS + JavaScript thuần (không framework, không backend).

## 📁 Cấu trúc

```
production-cost-tool/
├── index.html        # Toàn bộ tool (UI + logic)
├── assets/logo.png   # Logo Avielora
├── README.md
└── chat-history.txt  # Lịch sử trò chuyện với Claude Code (/export)
```
