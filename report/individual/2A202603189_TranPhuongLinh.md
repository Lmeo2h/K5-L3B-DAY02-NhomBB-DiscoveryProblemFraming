# Báo cáo cá nhân — 2A202603189_TranPhuongLinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`. Tiêu đề: `Báo cáo cá nhân — 2A202603189_TranPhuongLinh`.  
> Báo cáo hoàn chỉnh các phần cá nhân: CP1 (Scan problem), CP2 (Top 3 Problem Cards), CP3 (Nhật ký phản biện), CP7 (Reflection & Hiểu bài).

---

## 1. Thông tin học viên

- **Họ tên:** Trần Phương Linh
- **MSSV:** 2A202603189
- **Tên nhóm:** NhomBB (Lớp K5 · L3B)
- **Link repo nhóm:** [https://github.com/Lmeo2h/K5-L3B-DAY02-NhomBB-DiscoveryProblemFraming](https://github.com/Lmeo2h/K5-L3B-DAY02-NhomBB-DiscoveryProblemFraming)

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi xảy ra va chạm giao thông nhẹ, tôi muốn biết các bước chụp ảnh hiện trường và liên hệ bảo hiểm đúng chuẩn, để không bị hãng từ chối bồi thường | Tài xế taxi, Nhân viên giám định bảo hiểm | Hướng dẫn qua điện thoại mất 20–25 phút; 10% hồ sơ bồi thường bị từ chối do thiếu ảnh góc rộng |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận hàng trăm đánh giá 1 sao từ khách hàng mỗi ngày, tôi muốn phân loại nguyên nhân cốt lõi (thái độ, xe bẩn, đi ẩu, giá cước), để xử lý kỷ luật hoặc đào tạo lại | Quản lý chất lượng dịch vụ GSM | Đọc và gắn nhãn thủ công mất 2 tiếng/ngày trên portal phản hồi; trung bình 150 đánh giá tiêu cực/ngày |
| 3 | Lặp lại | Khi xe trong đội sắp đến hạn đăng kiểm định kỳ, tôi muốn hệ thống tự động thông báo và xếp lịch bảo dưỡng, để tránh xe bị phạt quá hạn | Quản lý phương tiện đội xe | Mất 3 tiếng mỗi tuần tra cứu file Excel ngày đăng ký của 200 xe; tháng trước 1 xe bị phạt 4 triệu do quá hạn 3 ngày |
| 4 | Tốn thời gian | Khi xe taxi điện báo pin < 10% giữa giờ cao điểm, tôi muốn nhanh chóng tìm ra trạm sạc còn chỗ hoặc xe cứu hộ, để xe không bị chết máy giữa đường | Tài xế Xanh SM, Điều phối viên | Mất 15 phút xử lý thủ công; tài xế toát mồ hôi lo sợ chết máy trên cầu |
| 5 | Pain từ người khác | Khi sinh viên năm nhất làm thủ tục đăng ký ký túc xá, họ muốn biết giấy tờ ưu tiên nào còn thiếu, để nộp bổ sung trước hạn | Tân sinh viên, Cán bộ quản lý KTX | Cán bộ KTX mất 5 phút/hồ sơ đối soát giấy tờ; 30% sinh viên phải đi lại 2 lần |
| 6 | Lặp lại | Khi tổ chức sự kiện workshop câu lạc bộ, tôi muốn tự động gửi email xác nhận kèm mã QR check-in cho người tham gia, để không phải gửi tay từng thư | Ban tổ chức sự kiện, Người tham dự | Mất 2 tiếng ngồi copy email gửi thư cho 120 người đăng ký |

**Dùng AI gợi ý thêm:** Tôi giữ lại ý #6 và bổ sung số liệu thời gian thật của câu lạc bộ. Bỏ ý "Trợ lý AI tự động giải quyết tranh chấp pháp lý bảo hiểm" vì vượt quá năng lực mô hình và có rủi ro pháp lý cao.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Hướng dẫn thủ tục bảo hiểm khi va chạm (#1) | Pain thật, tài xế hoang mang khi gặp tai nạn | Tần suất sự cố của 1 tài xế không cao bằng sự cố pin |
| 2 | Phân loại đánh giá 1 sao khách hàng (#2) | Lượng dữ liệu lớn, NLP phân tích cảm xúc tốt | Chưa giải quyết được ngay hành vi tức thời của tài xế |
| 3 | Tự động nhắc hạn đăng kiểm đội xe (#3) | Tránh phạt tài chính trực tiếp cho công ty | Dùng Rule/Cron-job thông thường là đủ, không cần AI |

---

### Problem Card #1 — Hướng dẫn thủ tục hiện trường bảo hiểm khi xảy ra va chạm

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi xảy ra va chạm giao thông nhẹ, tôi muốn biết các bước chụp ảnh hiện trường và liên hệ bảo hiểm đúng chuẩn, để không bị hãng từ chối bồi thường |
| **Actor** | Tài xế taxi Xanh SM; Nhân viên giám định bảo hiểm GSM |
| **Thời điểm / bối cảnh** | Ngay khi xảy ra va quệt nhẹ trên đường, tài xế đang hoảng sợ, cần giải phóng hiện trường tránh kẹt xe |
| **Quy trình hiện tại** | 1. Tài xế gọi hotline thông báo va chạm · 2. Tổng đài viên hướng dẫn các góc chụp ảnh cần thiết · 3. Tài xế chụp ảnh gửi Zalo · 4. Tổng đài viên kiểm tra ảnh đủ góc chưa · 5. Gửi thông tin sang công ty bảo hiểm |
| **Bottleneck** | Bước 2 & 4 (hướng dẫn qua điện thoại thiếu trực quan, tài xế chụp thiếu ảnh toàn cảnh hoặc mờ biển số mất 15–20 phút) |
| **Impact** | Tốn 25 phút/vụ va chạm; 10% hồ sơ bị bảo hiểm từ chối bồi thường, tài xế phải tự đền tiền |
| **Success metric** | Giảm thời gian xác nhận ảnh hiện trường từ 20 phút xuống dưới 5 phút |
| **Phương án không dùng AI** | Soạn một infographic hướng dẫn 4 góc chụp chuẩn dán sẵn trên kính chắn gió của xe |
| **Giả thuyết về AI** | Computer Vision kiểm tra độ nét và góc chụp của ảnh hiện trường ngay trên app tài xế |
| **Cảm nhận nhanh** | Workflow |

```text
HIỆN TẠI — 25 phút / vụ va chạm

[1. Gọi hotline: 3'] → [2. Nghe hướng dẫn miệng: 7'] 
→ [3. Chụp & gửi Zalo: 5'] → [4. Kiểm tra ảnh thiếu/sai: 8'] ← BOTTLENECK
→ [5. Bàn giao bảo hiểm: 2']
```

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (Bảo hiểm va chạm) và Card #2 (Phân loại đánh giá 1 sao). | Giúp nhóm mở rộng góc nhìn về các nghiệp vụ sau bán hàng của GSM. |
| Phản biện bài của bạn khác | Đặt câu hỏi cho Hiệp: *"Bài toán phân loại cư dân Vinhomes có cần AI không hay chỉ cần sửa form dropdown?"* | Giúp nhóm nhận diện ranh giới giữa No AI (sửa form) và AI thật sự cần thiết. |
| Research giải pháp có sẵn (CP4) | Trực tiếp tra cứu, mở và kiểm chứng 4 giải pháp: Tesla Fleet API, Geotab EV, Jira Service Management, n8n. | Tìm ra bài học cốt lõi: Thế giới đã có API telemetry, nhóm chỉ cần tập trung vào lớp logic cứu hộ và an toàn đặc thù của xe điện. |
| Đánh giá 4 Rủi ro (CP6) | Soạn thảo bảng đánh giá 4 rủi ro Marty Cagan (Value, Usability, Feasibility, Viability) và đề xuất kịch bản Kill Switch. | Đảm bảo sản phẩm tuân thủ chặt chẽ các quy định an toàn và khả thi về mặt kỹ thuật. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tìm thêm góc nhìn về nghiệp vụ quản lý tài sản phương tiện. | Gợi ý bài toán đăng kiểm xe định kỳ. | Ý tưởng rất rời rạc, không gắn với ngữ cảnh xe điện. | Viết lại thành Job Story gắn với rủi ro tài chính của công ty vận tải. |
| CP4 Research | Tìm kiếm các bài báo và tài liệu kỹ thuật về quản lý sạc xe điện. | Giới thiệu case study của Geotab trong quản lý sạc thông minh. | Đưa một đường link tài liệu cũ bị lỗi 404. | Tôi tự Google tìm lại trang tài liệu chính thức năm 2024 của Geotab và kiểm chứng nội dung. |
| CP6 Quyết định | Gợi ý các tiêu chuẩn an toàn cho hệ thống điều phối cứu hộ. | Giúp làm rõ khái niệm "Kill Switch" và ngưỡng dừng rủi ro. | Cho rằng rủi ro Viability là Cao vì chi phí server đắt. | Tôi sửa thành rủi ro Thấp vì mô hình dùng Gemini Flash rất rẻ, chi phí dưới 100đ/ca. |

---

## 6. Reflection (CP7)

### 6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?
Tôi học được rằng một vấn đề có hay đến đâu trên lý thuyết cũng sẽ vô nghĩa nếu không thể kiểm chứng được trong thực tế. Đề tài dự báo nhu cầu xe của Huy nghe rất hấp dẫn, nhưng khi nhóm chất vấn về nguồn dữ liệu và cách đo lường thì hoàn toàn bế tắc. Ngược lại, đề tài pin của Hiệp rất cụ thể và chạm đúng nỗi sợ có thật của tài xế.

### 6.2. Nhóm có lúc nào bị "solution-first" không?
Có, khi nghiên cứu về Tesla Fleet API, tôi từng đề xuất: *"Hay nhóm mình làm một hệ thống IoT cắm thẳng vào cổng OBD-II của xe luôn"*. Minh đã kéo tôi về thực tế: *"Chúng ta đang làm Problem Framing để giải quyết nỗi đau của điều phối viên, không phải đi chế tạo phần cứng!"*. Nhờ vậy nhóm không bị lạc lối sang đề tài kỹ thuật vi mạch.

### 6.3. Tôi có đổi ý sau khi bị phản biện không?
Tôi đã đổi ý về bài toán bảo hiểm của mình. Ban đầu tôi nghĩ bài đó rất hay, nhưng khi Hiệp chỉ ra rằng tần suất va chạm của một tài xế chỉ là 1–2 lần/năm (quá thấp so với 2–3 lần/tháng bị pin yếu), tôi nhận ra giá trị kinh tế và tần suất sử dụng của bài toán sự cố pin vượt trội hơn hẳn.

### 6.4. Kết quả kiểm chứng có làm tôi bất ngờ không?
Tôi rất bất ngờ trước sự nghiêm ngặt của chính sách an toàn tại GSM qua lời kể của bác Trưởng ca: an toàn là ưu tiên tuyệt đối, không có chỗ cho sự "thử nghiệm liều lĩnh". Nếu AI đưa ra chỉ dẫn sai dù chỉ một lần làm xe chết máy giữa đường, toàn bộ dự án sẽ bị đình chỉ ngay. Điều này củng cố tầm quan trọng của Ngưỡng dừng (Stopping Threshold) mà tôi phụ trách thiết kế.

### 6.5. Điều khó nhất khi viết Problem Statement là gì?
Khó nhất là giữ cho Problem Statement thuần khiết, không chứa đựng bất kỳ giải pháp nào. Rất dễ vô thức viết *"vấn đề là thiếu một phần mềm AI..."* thay vì mô tả đúng bản chất: *"vấn đề là điều phối viên mất 15 phút tra cứu thủ công qua 3 màn hình"*.

### 6.6. Nếu làm lại, tôi sẽ đổi gì?
Tôi sẽ chuẩn bị sẵn một kịch bản giả lập số liệu chi tiết hơn về chi phí vận hành của xe cứu hộ sạc lưu động để tính toán ROI (Return on Investment) thuyết phục hơn cho ban lãnh đạo.

---

### 6.7. Hiểu bài

1. **Problem:** Điều phối viên Xanh SM mất 15 phút xử lý thủ công mỗi ca xe báo pin thấp, gây nguy cơ xe chết máy dừng giữa đường.
2. **Quy trình:** Hiện tại gồm 5 bước tra cứu phân mảnh giữa telemetry xe và bản đồ trạm sạc.
3. **Metric:** Giảm thời gian xử lý xuống dưới 5 phút, tỷ lệ duyệt nháp $\ge 85\%$, vi phạm an toàn pin $0\%$.
4. **Boundary:** AI không tự phát lệnh điều xe cứu hộ, cấm chỉ dẫn xe chạy tiếp khi pin $< 5\%$.
5. **Mức can thiệp AI:** Workflow bán tự động (Rule an toàn + AI soạn nháp + Người duyệt 1-click).
6. **Quyết định:** Go, phạm vi nhỏ thông qua pilot 2 tuần tại Hub Long Biên có ngưỡng dừng an toàn rõ ràng.

---

## 7. Tài liệu tham khảo

1. Cagan, M. (2017). *Inspired: How to Create Tech Products Customers Love*. Wiley.
2. Tesla Inc. (2024). *Fleet API*. [https://developer.tesla.com/docs/fleet-api](https://developer.tesla.com/docs/fleet-api)
3. Geotab Inc. (2024). *EV Management*. [https://www.geotab.com/fleet-management-solutions/electric-vehicles/](https://www.geotab.com/fleet-management-solutions/electric-vehicles/)
