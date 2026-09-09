# Phân Tích Thiết Kế Quảng Cáo CPAS Shopee — MOCHA Skincare

## 1. CPAS Shopee là gì?

**CPAS (Collaborative Performance Advertising Solution)** là hình thức quảng cáo hợp tác giữa thương hiệu và Shopee, chạy trên nền tảng **Meta Ads (Facebook/Instagram)** nhưng liên kết trực tiếp đến sản phẩm trên Shopee.

### Ưu điểm CPAS:
- Retarget người dùng đã xem/thêm giỏ hàng trên Shopee
- Đồng bộ catalog sản phẩm từ Shopee store
- Tối ưu conversion (mua hàng) trực tiếp
- Tracking end-to-end từ impression → click → purchase

---

## 2. Thuật Toán Đề Xuất — 2 Tầng

### Tầng 1: Meta Algorithm (Facebook/Instagram)
| Yếu tố | Ảnh hưởng | Cách tối ưu |
|---------|-----------|-------------|
| **Relevance Score** | Cao | Hình ảnh phù hợp đối tượng mục tiêu |
| **CTR Prediction** | Cao | Giá khuyến mãi nổi bật, product hero |
| **Image Quality** | Trung bình | Ảnh rõ nét, không mờ, ≥1080px |
| **Text Overlay** | Cao | **< 20% diện tích ảnh** (quy tắc Meta) |
| **Engagement** | Trung bình | Hình ảnh hấp dẫn, có gift/promotion |

### Tầng 2: Shopee Algorithm
| Yếu tố | Ảnh hưởng | Cách tối ưu |
|---------|-----------|-------------|
| **Product Catalog Sync** | Bắt buộc | Đồng bộ đúng SKU từ Shopee store |
| **Dynamic Retargeting** | Cao | Hiển thị đúng sản phẩm người dùng đã xem |
| **Price Signal** | Cao | Giá cạnh tranh + giảm giá rõ ràng |
| **Conversion Rate** | Cao | Landing page tối ưu trên Shopee |

---

## 3. Nguyên Tắc Thiết Kế Tối Ưu CPAS

### Kích thước & Tỷ lệ
- **1:1 (1080×1080px)** — hiển thị tốt nhất trên Facebook/Instagram feed
- Cũng hỗ trợ 4:5 (1080×1350px) cho Instagram Stories

### Bố cục (Layout)
- **Sản phẩm chiếm 60-70%** diện tích ảnh
- **Text < 20%** diện tích (Meta penalizes quảng cáo có nhiều text)
- Bố cục đường chéo (diagonal) tạo chuyển động mắt
- 2 deal sections cho cross-sell/upsell

### Giá & Khuyến mãi
- **Price anchoring**: Hiển thị giá gốc gạch bỏ → giá sale nổi bật
- **Gift value badges**: Hiển thị tổng giá trị quà tặng (tạo urgency)
- **Contrast pricing**: Giá sale bằng màu brand (xanh dương MOCHA)

### Thương hiệu
- Header bar thương hiệu ở top (nhận diện nhanh)
- Màu sắc nhất quán: xanh dương MOCHA (#1A5A9E, #0F3B6B)
- Font: Montserrat (headings), Noto Sans (body Vietnamese)

---

## 4. Chi Tiết Thiết Kế — File: `cpas-ad-design.html`

### Deals Structure

**MUA 01: Sữa Rửa Mặt Bio-Active Cleanser 300g**
- Giá gốc: 399.000 VND → Giá sale: 279.000 VND
- Tặng: Kem Chống Nắng UV-Block Plus 15g (trị giá 145.000 VND)

**MUA 02: Combo Gel Trị Mụn Smart Target + Sữa Rửa Mặt Bio-Active**
- Giá gốc: 699.000 VND → Giá sale: 449.000 VND
- Tặng: Kem Chống Nắng UV-Block Plus 15g (trị giá 145.000 VND)

### Color Palette
```
Deep Blue:    #0F3B6B (brand header, headings)
Brand Blue:   #1A5A9E (products, badges, CTA)
Mid Blue:     #3B7DD8 (badge gradients)
Light Blue:   #8BB8E8 (decorative)
Background:   #E2E8F2 → #EEF1F7 (gradient)
Teal:         #1D8B72 (Smart Target accent)
```

### Lưu Ý Khi Sản Xuất Ảnh Thật
1. **Thay thế SVG illustrations** bằng ảnh sản phẩm thật (chụp studio, nền trắng/trong suốt)
2. **Giữ nguyên layout** — vị trí sản phẩm, text, badges
3. **Kiểm tra text ratio** bằng Facebook Text Overlay Tool
4. **Export** ở 1080×1080px, chất lượng cao (PNG hoặc JPG quality 95%)
5. **A/B test**: Thử 2-3 biến thể (thay đổi giá, gift, sắp xếp sản phẩm)

---

## 5. Khuyến Nghị Chạy CPAS

### Targeting
- **Retargeting**: Người đã xem sản phẩm trên Shopee 7-14 ngày
- **Lookalike**: Người tương tự khách hàng đã mua
- **Interest**: Skincare, chăm sóc da, mỹ phẩm, acne treatment

### Budget
- Bắt đầu: 200K-500K VND/ngày
- Scale lên khi ROAS > 3x
- Thời gian chạy tối thiểu: 7 ngày để tối ưu

### KPIs theo dõi
- **CTR**: > 1.5% (tốt), > 2.5% (xuất sắc)
- **CPC**: < 3.000 VND
- **ROAS**: > 3x
- **Conversion Rate**: > 2%
