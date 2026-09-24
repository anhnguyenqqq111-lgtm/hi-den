# Technical and Ads-readiness audit — hi-den.vn

## Mức độ tin cậy dữ liệu

Ngày kiểm tra: 24/09/2026. Đã kiểm tra các trang công khai và trang sản phẩm có thể truy cập. PageSpeed, robots.txt, sitemap.xml, schema chi tiết, trạng thái gửi form và dữ liệu chuyển đổi vẫn cần xác nhận bằng quyền truy cập website/GA4/GSC/GTM.

## Bảng kiểm

| Hạng mục | Điểm tạm tính | Trạng thái | Việc cần làm trước khi chạy |
|---|---:|---|---|
| HTTPS và domain | 8/10 | 🟢 | Duy trì HTTPS, kiểm tra redirect www/non-www |
| Crawl/index | 4/10 | 🟡 | Xác nhận robots.txt, XML sitemap, canonical, trang tag và bài trùng |
| Core Web Vitals | Chưa đo | 🟡 | Đo mobile/desktop trên các LP quảng cáo; nén ảnh, giảm script nếu cần |
| Mobile UX | Chưa đo | 🟡 | Kiểm tra tap target, nút gọi, form và sticky CTA trên mobile |
| Schema | Chưa xác nhận | 🟡 | Tối thiểu Organization, Product/Service, Breadcrumb, FAQ khi nội dung đủ điều kiện |
| Tracking | 2/10 | 🔴 | Cài GA4, Google Ads conversion, GTM, Meta Pixel/CAPI nếu có thể |
| Lead routing | 4/10 | 🟡 | Gắn nguồn/medium/campaign vào form, email, hotline và CRM |
| Trust/identity | 5/10 | 🟡 | Đồng nhất tên pháp nhân, địa chỉ, MST, hotline, email, nhà máy và chứng nhận |

## Phát hiện live cần xử lý trước Ads

- Trang giới thiệu ghi địa chỉ tại Tòa nhà Vietcombank, MST `0318583138` và hotline `028-7301-1677`; trang liên hệ và Hot Air Blower lại ghi địa chỉ 123 Lý Chính Thắng, MST `0319569231` và số `0938-31-31-56`.
- Trang [Hot Air Blower](https://hi-den.vn/hot-air-blower/) có dữ liệu hữu ích cho quảng cáo B2B: model HDBM126/HDBM3310, công suất 6,5–60 kW, nhiệt độ, lưu lượng khí, điện áp, kích thước ống và kích thước máy.
- Cần xác nhận sự khác nhau giữa dải công suất giới thiệu `6,5–60 kW` và các bảng model; không đưa claim vào quảng cáo trước khi kỹ thuật duyệt datasheet chính thức.
- Fanpage không được kiểm tra đầy đủ bằng trình thu thập công khai; cần cấp quyền Meta Business để kiểm tra lịch sử quảng cáo, pixel, tài khoản và chất lượng lead.

## Điều kiện kỹ thuật để mở Ads

1. Tất cả CTA gọi điện, email và form phải tạo được conversion riêng
2. Form phải có trường công ty, chức danh, loại máy/giải pháp, môi chất, nhiệt độ, công suất/kích thước, số lượng và thời điểm mua
3. Có trang cảm ơn hoặc event xác nhận gửi form thành công
4. Có UTM chuẩn và bảng đối soát lead theo tuần
5. Không dùng một LP chung cho toàn bộ nhóm máy
6. Các claim như ISO, số năm kinh nghiệm, tỷ lệ tiết kiệm và hiệu suất phải có tài liệu chứng minh nội bộ

## Ưu tiên sửa

- P0: tracking, form qualification, hotline/email, trang cảm ơn và quyền truy cập GA4/GSC/Ads
- P1: tách LP theo nhóm nhu cầu, viết lại hero/CTA/thông số/ứng dụng và bổ sung tài liệu kỹ thuật
- P1: kiểm tra index, canonical, sitemap, schema và tốc độ trang
- P2: remarketing audiences, video, case study, tài liệu tải xuống và nội dung hỗ trợ kỹ thuật
