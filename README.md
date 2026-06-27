# 🏭 Tính giá sản xuất & Quyết định Launching

Mini tool web giúp người làm thương mại điện tử **so sánh báo giá sản xuất từ nhiều NSX (nhà sản xuất) ở các mức MOQ khác nhau (mặc định MOQ 20 và MOQ 100)**, đối chiếu với giá brand gốc, và đưa ra **khuyến nghị có nên launch sản phẩm hay không**.

## ✨ Tính năng

- Nhập giá brand gốc + giá bán dự kiến + margin tối thiểu mong muốn.
- Thêm/xóa nhiều NSX, mỗi NSX có: đơn giá @MOQ thấp, đơn giá @MOQ cao, phí khuôn/setup (1 lần), phí ship + thuế / đơn vị.
- Tự động tính cho từng NSX × từng MOQ:
  - Giá vốn thực/SP (đã **phân bổ phí khuôn** theo số lượng)
  - Tổng vốn đầu tư, lợi nhuận/SP, **margin %**
  - **Chênh lệch so với brand gốc** (rẻ hơn bao nhiêu %)
  - Tổng lợi nhuận nếu bán hết + điểm hòa vốn
  - **Nhãn quyết định:** 🟢 NÊN LAUNCH / 🟡 CÂN NHẮC / 🔴 KHÔNG
- Banner tự highlight **phương án tốt nhất**.
- Lưu dữ liệu bằng `localStorage`, xuất **CSV**, có dữ liệu mẫu.

## 🚀 Cách dùng

Không cần cài đặt hay hosting. Chỉ cần **mở file `index.html` bằng trình duyệt** (Chrome/Safari/Edge...).

Hoặc bấm nút **"Dùng dữ liệu mẫu"** để xem ngay một ví dụ.

## 🛠️ Công nghệ

HTML + CSS + JavaScript thuần (không framework, không backend).

## 📁 Cấu trúc

```
production-cost-tool/
├── index.html        # Toàn bộ tool (UI + logic)
├── README.md
└── chat-history.txt  # Lịch sử trò chuyện với Claude Code (/export)
```
