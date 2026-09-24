# Audit report quyết định chạy Ads — Hi-Den HeatTech

## 1. Kết luận

**Nên thực hiện audit report trước khi chạy hoặc scale Ads.** Bộ keyword có đủ tín hiệu để kiểm tra và tối ưu, nhưng chưa đủ sạch để đưa toàn bộ ngân sách vào ngay.

Lý do:

1. Có nhu cầu thương mại rõ ở các cụm `bộ trao đổi nhiệt`, `bộ trao đổi nhiệt dạng ống`, `ống trao đổi nhiệt cánh nhôm`, `máy thổi khí nóng công nghiệp` và `báo giá bộ trao đổi nhiệt`.
2. Cạnh tranh cao: nhiều cụm có Competition 81–100; Top of Page Bid có thể lên tới 36.097đ hoặc 61.251đ tùy keyword.
3. Volume lớn đang lẫn intent: `máy thổi khí nóng` 110 volume và `bộ trao đổi nhiệt` 260 volume chưa đồng nghĩa với 350 lượt tìm kiếm B2B.
4. Website có LP Hot Air Blower khá đầy đủ nhưng còn thiếu CTA/form qualification và đang có xung đột thông tin nhận diện giữa các trang.
5. Hai nhóm Fin Tube và Heat Exchanger chưa thể xác nhận đầy đủ bằng live fetch trong lần quét này; không nên dùng làm căn cứ triển khai rộng nếu chưa có quyền kiểm tra trực tiếp.

## 2. Phạm vi và phương pháp

| Hạng mục | Kết quả |
|---|---|
| Domain | `https://hi-den.vn/` |
| Ngày quét | 24/09/2026 |
| Thị trường | Việt Nam, tiếng Việt |
| Keyword input | Bộ dữ liệu Keyword Tool do khách hàng cung cấp |
| Website scan | Trang liên hệ, Hot Air Blower, trang giới thiệu và các URL sản phẩm được phát hiện từ navigation |
| GA4/GSC/Google Ads/Meta | Chưa được cấp quyền; không có số liệu conversion hoặc search terms thực tế |
| PageSpeed/mobile | Chưa đo trực tiếp trong lần này; không suy diễn điểm Core Web Vitals |
| SERP | Dùng để định hướng intent/đối thủ; không ghi nhận thứ hạng chính xác nếu chưa có SERP export hoặc công cụ rank checker |

## 3. Quyết định keyword → audit

| Cụm | Dữ liệu thực tế | Mức phù hợp B2B | Quyết định audit |
|---|---|---|---|
| Bộ trao đổi nhiệt | 260 volume, trend -46%, bid 4.540–16.212đ, competition 81 | Cao nhưng rộng | Audit LP, search intent, form và negative keyword |
| Bộ trao đổi nhiệt dạng tấm | 140 volume, trend +180%, bid 4.116–36.097đ, competition 100 | Chưa chắc phù hợp sản phẩm | Audit năng lực sản phẩm trước khi chạy |
| Bộ trao đổi nhiệt dạng ống | 50 volume, trend +25%, bid 3.168–7.996đ, competition 86 | Cao | Audit LP dạng ống/ống chùm |
| Báo giá bộ trao đổi nhiệt | 10 volume, bid 0đ, competition 0 | Rất cao về intent | Ưu tiên tạo CTA/form báo giá |
| Ống trao đổi nhiệt | 40 volume, trend +75%, bid 379–7.979đ, competition 68 | Cao | Audit LP Fin Tube |
| Ống trao đổi nhiệt cánh nhôm | 20 volume, trend +200%, competition 16 | Cao nếu có cấu hình đúng | Ưu tiên kiểm tra product-market fit |
| Máy thổi khí nóng công nghiệp | 40 volume, competition 100 | Cao | Audit Hot Air Blower và chạy pilot có kiểm soát |
| Máy thổi khí nóng | 110 volume, competition 100 | Rộng, dễ sai intent | Chỉ audit search terms/negative, không scale theo volume |
| Máy sưởi công nghiệp | 70 volume, competition 100 | Có thể phù hợp | Audit ngôn ngữ “heater công nghiệp” và intent dân dụng |

## 4. Kết quả quét website

### 4.1 Hot Air Blower — LP ưu tiên pilot

URL: [https://hi-den.vn/hot-air-blower/](https://hi-den.vn/hot-air-blower/)

**Observed:**

- H1 khớp trực tiếp với nhóm `Hot Air Blower | Máy Thổi Khí Nóng Công Nghiệp`.
- Có cấu tạo, ứng dụng, hướng dẫn lựa chọn, FAQ và quy trình tư vấn.
- Có các model/thông số: HDBM126 6,5 kW; HDBM3310 10 kW; HDCB 15–60 kW; điện áp, nhiệt độ, lưu lượng khí, kích thước ống và kích thước máy.
- Trang nêu các ngành ứng dụng: điện tử, thực phẩm, nhựa, bao bì, hóa chất, cơ khí.

**Gap cần audit/sửa:**

- CTA báo giá và gửi thông số chưa nổi bật xuyên suốt trang.
- Chưa thấy form qualification chuyên biệt cho nhiệt độ, lưu lượng, áp suất, điện áp, kích thước ống, số lượng và timeline.
- Nội dung có các claim như tiết kiệm năng lượng, tuổi thọ cao, hiệu suất cao; cần datasheet/test report trước khi đưa vào quảng cáo.
- Dải `6,5–60 kW` cần đối chiếu với bảng model chính thức để tránh sai lệch giữa ad copy và tư vấn kỹ thuật.
- Nội dung dài, phần thông số quan trọng nên đưa lên trước phần diễn giải khái niệm.

**Verdict:** Có thể làm LP pilot sau khi sửa P0; chưa nên dùng nguyên trạng để scale.

### 4.2 Máy Fin Tube / máy sưởi tuần hoàn

URL được navigation trỏ tới: [https://hi-den.vn/may-suoi-tuan-hoan/](https://hi-den.vn/may-suoi-tuan-hoan/)

**Observed:** Tên trang gắn với Fin Tube và sản xuất theo yêu cầu; đây là hướng phù hợp với keyword `ống trao đổi nhiệt cánh nhôm` và nhu cầu custom.

**Chưa xác minh được:** Nội dung chi tiết, bảng cấu hình, vật liệu, fin pitch, dung sai, áp suất/nhiệt độ, upload bản vẽ và CTA do live fetch không trả đủ nội dung.

**Verdict:** Cần audit riêng trước khi chạy nhóm Fin Tube; không điều hướng toàn bộ keyword về Hot Air Blower.

### 4.3 Heat Exchanger

URL được navigation trỏ tới: [https://hi-den.vn/heat-exchanger/](https://hi-den.vn/heat-exchanger/)

**Observed:** Website có thực thể “Heat Exchanger” trong navigation và nội dung liên quan đến bộ trao đổi nhiệt.

**Chưa xác minh được:** LP có khớp đầy đủ với `dạng tấm`, `dạng ống`, `ống chùm`, môi chất, tải nhiệt, nhiệt độ vào/ra, áp suất và yêu cầu bản vẽ hay không.

**Verdict:** Nên audit và xây nhóm quảng cáo riêng; keyword `bộ trao đổi nhiệt dạng tấm` chỉ chạy sau khi Hi-Den xác nhận có sản phẩm/năng lực tương ứng.

### 4.4 Contact và trust

URL: [https://hi-den.vn/lien-he/](https://hi-den.vn/lien-he/)

**Observed:** Có form tên, email, số liên lạc, tỉnh và chi tiết yêu cầu; có thông tin công ty, MST, email và số điện thoại.

**High priority issue:** Trang giới thiệu và các trang sản phẩm/liên hệ hiển thị địa chỉ, MST và hotline khác nhau. Cần chốt một bộ thông tin pháp nhân trước khi chạy quảng cáo.

## 5. Technical/CRO issue table

| URL | Issue | Evidence | Severity | Fix | Owner | Validation |
|---|---|---|---|---|---|---|
| Toàn site | Entity/contact không đồng nhất | Các trang hiển thị địa chỉ, MST, hotline khác nhau | High | Chốt thông tin pháp lý và cập nhật toàn site | Client/Dev | Crawl lại header/footer/contact |
| Hot Air Blower | CTA chưa gắn rõ với thông số kỹ thuật | Nội dung có tư vấn nhưng chưa có form chuyên biệt | High | Thêm CTA và form theo nhiệt độ/lưu lượng/model | CRO/Dev | Test form + conversion event |
| Hot Air Blower | Claim kỹ thuật cần chứng cứ | Tiết kiệm, tuổi thọ, hiệu suất, coil heater | High | Duyệt datasheet/test report trước ad copy | Client/Technical | QA claim matrix |
| Fin Tube | Thiếu dữ liệu cấu hình để qualify | Chưa xác minh vật liệu, fin pitch, dung sai, bản vẽ | High | Tạo LP/form upload bản vẽ | Product/Content/Dev | Lead có đủ trường kỹ thuật |
| Heat Exchanger | Chưa map rõ dạng sản phẩm | Keyword có dạng tấm, ống, ống chùm, nước | High | Tách ad group và LP theo loại/năng lực thật | Ads/Product | Search term + lead quality |
| Toàn site | Tracking chưa xác minh | Chưa có quyền GA4/GTM/Ads/Meta | High | Cài event form/call/email/UTM và dashboard | Analytics/Dev | DebugView + Ads test conversion |
| Mobile/Speed | Chưa đo được | Chưa có PageSpeed/real-user data | Medium | Đo sau khi xác định 2 LP pilot | Dev | Mobile CWV report |

## 6. Khuyến nghị chạy thử sau audit

Trong 30 ngày đầu, nếu ngân sách media giữ ở 60 triệu/tháng và không tính phí quản lý:

- Google media 50 triệu: 60% Heat Exchanger/Fin Tube, 25% Hot Air Blower, 10% máy sưởi công nghiệp, 5% brand/test.
- Facebook media 10 triệu: ưu tiên remarketing và retarget người xem LP, không dùng làm nguồn lead chính.
- Không mở rộng từ khóa `máy sấy công nghiệp`, `vệ sinh bộ trao đổi nhiệt`, `Samsung`, `LG`, `rửa xe` nếu không có landing page và năng lực đúng nhu cầu.
- Chỉ tăng ngân sách khi có ít nhất một chu kỳ Search Terms và CRM cho biết nhóm nào tạo MQL/SQL, không tối ưu theo lead thô.

## 7. Kết luận cuối

**Audit report là cần thiết và nên được thực hiện trước khi triển khai đầy đủ ngân sách.** Tuy nhiên, phạm vi hợp lý là audit Ads-readiness + LP/CRO + keyword-to-intent trong giai đoạn đầu; chưa nên báo cáo như một audit SEO toàn diện khi chưa có GA4, GSC, PageSpeed, crawl đầy đủ và dữ liệu CRM.

### Dữ liệu cần cấp để hoàn tất audit cấp production

- Quyền GA4, GSC, GTM, Google Ads và Meta Business.
- Danh sách model/sản phẩm thực sự bán hoặc sản xuất.
- Datasheet, bản vẽ, chứng nhận, case study và chính sách bảo hành.
- Thông tin pháp nhân/hotline/email chính thức.
- 20–50 lead gần nhất có phân loại đạt/chưa đạt và trạng thái sales.
