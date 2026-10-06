# Chuẩn form Phiếu đề xuất – Công ty TNHH TM Ứng dụng Dược Mỹ phẩm Công nghệ cao Mocha

Chuẩn này lấy theo 2 phiếu đã được anh/chị chỉnh tay trên Google Docs ngày 06/10/2026:

- [Phiếu đề xuất - Thêm máy live Shopee (iPhone 14 Pro cũ) - bản sửa](https://docs.google.com/document/d/179gOgx903yA1lUjADCJvSb73eVk5MQFn6LwOXY7O32Y/edit)
- [Phiếu đề xuất - Thêm máy live Shopee (Camera Hollyland)](https://docs.google.com/document/d/1ZeYW4PM4Tm5r-8lDc5IRdgxHRC5n0Um8tBEoTIBZCSA/edit)

Mọi phiếu đề xuất soạn sau này **phải theo đúng chuẩn dưới đây**. File HTML mẫu dựng sẵn: `vi_du_chuan_form.html`.

## 1. Thứ tự các phần

1. **Bảng đầu trang** gồm 2 cột, không có viền:
   - Cột trái: **CÔNG TY TNHH** / **TM ỨNG DỤNG DƯỢC MỸ PHẨM CÔNG NGHỆ CAO MOCHA** (in đậm, căn giữa).
   - Cột phải: **CỘNG HÒA XÃ HỘI CHỦ NGHĨA VIỆT NAM** (in đậm) / Độc lập - Tự do - Hạnh Phúc.
   - Dòng 2, cột phải: ***Tp. HCM, ngày … tháng … năm …*** (in đậm và nghiêng).
2. **PHIẾU ĐỀ XUẤT**: in đậm, căn giữa, cỡ 16.
3. **Kính gửi: Giám Đốc Công Ty** / **Phòng HCNS Công ty** (in đậm).
4. Bốn mục lớn **đánh số La Mã tự động** (danh sách đánh số của Docs/Word, không gõ tay "I." "II."), in đậm, thụt lề 36pt:
   - **I. Thông tin CBNV:**
     - Họ và tên CBNV: Nguyễn Văn Việt
     - Chức vụ: Lead Sàn
     - Bộ Phận/Phòng/Ban: Kinh doanh
   - **II. Nội dung đề xuất:** gồm 1 đoạn tóm tắt (tổng chi phí in đậm), bảng chi phí, dòng ghi chú nguồn giá (in nghiêng) và thời gian triển khai.
   - **III. Lý do đề xuất:** gồm các tiểu mục **1. 2. 3. 4.** in đậm (Thực trạng hiện tại · Kết quả đạt được · Mong muốn triển khai · Hiệu quả dự kiến/hoàn vốn). Gạch đầu dòng viết dạng `- **Nhãn:** nội dung`. Cuối mục có câu "Kính đề nghị Ban Giám đốc xem xét, phê duyệt…".
   - **IV. Ý kiến của Trưởng Bộ phận/Phòng/Ban:** để **5 dòng chấm** `……………………………………………………………………………………………………..` cho trưởng bộ phận viết tay.
5. **Bảng ký tên** gồm 4 cột, không có viền, in đậm, căn giữa, **theo đúng thứ tự**:

   | Người lập phiếu | Trưởng Phòng/Bộ phận | Phòng HCNS | Giám Đốc duyệt |
   |---|---|---|---|
   | Lê Văn Trường | Nguyễn Văn Đức | (để trống) | (để trống) |

## 2. Định dạng

- Toàn bộ văn bản dùng font Times New Roman, cỡ 12.
- Bảng số liệu có viền đen 1px. Hàng tiêu đề in đậm, căn giữa, nền `#D9E2F3`. Dòng **TỔNG CỘNG** in đậm.
- Số tiền viết dạng `20.579.400 đ` (dấu chấm phân cách hàng nghìn, dấu phẩy cho số thập phân, ví dụ `3,75%`).

## 3. Cách đưa lên Google Docs

- Tạo file bằng Google Drive `create_file` với `contentMimeType: text/html`. Lấy `vi_du_chuan_form.html` làm khung rồi thay nội dung.
- Bốn mục lớn viết bằng `<ol type="I" start="N"><li><b>…</b></li></ol>` để Docs tạo danh sách đánh số La Mã thật. Sau khi tạo file phải đọc lại để kiểm tra số La Mã đã hiện đúng.
