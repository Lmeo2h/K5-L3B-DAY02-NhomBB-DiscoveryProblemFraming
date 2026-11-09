# Báo cáo cá nhân — 2A202601245_NguyenDucMinh

> Đổi tên file theo quy tắc `MSSV_HoTen.md`. Tiêu đề: `Báo cáo cá nhân — 2A202601245_NguyenDucMinh`.  
> Báo cáo hoàn chỉnh các phần cá nhân: CP1 (Scan problem), CP2 (Top 3 Problem Cards), CP3 (Nhật ký phản biện), CP7 (Reflection & Hiểu bài).

---

## 1. Thông tin học viên

- **Họ tên:** Nguyễn Đức Minh
- **MSSV:** 2A202601245
- **Tên nhóm:** NhomBB (Lớp K5 · L3B)
- **Link repo nhóm:** [https://github.com/Lmeo2h/K5-L3B-DAY02-NhomBB-DiscoveryProblemFraming](https://github.com/Lmeo2h/K5-L3B-DAY02-NhomBB-DiscoveryProblemFraming)

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tài xế giao ca trực, tôi muốn tổng hợp nhanh nhật ký các sự cố pin và kỹ thuật phát sinh trong ca, để bàn giao đầy đủ cho điều phối viên ca sau | Điều phối viên trực ca | Mất 30 phút cuối mỗi ca lọc tin nhắn Zalo; 2 lần tháng trước ca sau không biết xe đang chờ sửa |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi khách hàng gọi hỏi về chính sách cọc và đổi pin xe máy điện VinFast Feliz/Klara, tôi muốn trích xuất đúng điều khoản hợp đồng mới nhất, để giải đáp chính xác | Nhân viên CSKH VinFast | Mất 7 phút tra cứu qua 15 file PDF chính sách; trung bình 20 cuộc gọi/ngày |
| 3 | Pain từ người khác | Khi tài xế báo cáo trạm sạc bị xe xăng chiếm dụng vị trí đỗ, tôi muốn thông báo ngay cho ban quản lý bãi xe, để giải phóng trụ sạc cho xe điện vào sạc | Tài xế Xanh SM, Ban quản lý bãi đỗ | Tài xế chờ 15–20 phút tại trạm; trung bình 5–8 vụ phản ánh/ngày trên nhóm Zalo |
| 4 | Tốn thời gian | Khi xe taxi điện bị cạn pin khẩn cấp (< 10%), tôi muốn có hướng dẫn trạm sạc khả dụng ngay lập tức, để di chuyển tới sạc an toàn | Tài xế taxi Xanh SM | Chờ tổng đài 12–15 phút; 2 lần tài xế bị sập nguồn xe trên đường |
| 5 | Lặp lại | Khi sinh viên đăng ký mượn phòng lab làm đồ án AI, tôi muốn kiểm tra lịch trống và tự động duyệt theo quy định, để không phải trả lời từng email | Quản trị phòng lab VinUni, Sinh viên | 40 email/tuần; mất 10 phút/email kiểm tra lịch và gửi xác nhận |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi học môn Deep Learning, tôi muốn tóm tắt nhanh các phương pháp tối ưu hóa từ bài giảng PDF 80 trang, để ôn thi hiệu quả | Sinh viên | Mất 2–3 tiếng đọc và rút trích công thức cho mỗi chương |

**Dùng AI gợi ý thêm:** Sau khi tự scan 5 ý, tôi nhờ AI gợi ý thêm và bổ sung ý #6. Tôi bỏ ý "Chatbot giải đáp thắc mắc toàn diện cho khách hàng VinFast" vì quá rộng và không có quy trình thật.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp nhật ký bàn giao ca (#1) | Quy trình lặp lại hàng ngày, tốn thời gian cố định | Dữ liệu Zalo rời rạc có trích xuất tự động được không |
| 2 | Tra cứu chính sách thuê pin VinFast (#2) | Nỗi đau đọc tài liệu PDF dài dòng của CSKH | Chính sách thay đổi liên tục, dễ bị trích dẫn văn bản cũ |
| 3 | Báo cáo trạm sạc bị chiếm dụng (#3) | Nỗi bức xúc thường xuyên của tài xế xe điện | Phụ thuộc vào con người ngoài đời (bảo vệ bãi xe) |

---

### Problem Card #1 — Tổng hợp nhật ký bàn giao ca trực vận hành

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi tài xế giao ca trực, tôi muốn tổng hợp nhanh nhật ký các sự cố pin và kỹ thuật phát sinh trong ca, để bàn giao đầy đủ cho điều phối viên ca sau |
| **Actor** | Điều phối viên trực ca vận hành GSM |
| **Thời điểm / bối cảnh** | 30 phút trước khi hết ca trực (ca sáng 6h–14h, ca chiều 14h–22h, ca đêm 22h–6h) |
| **Quy trình hiện tại** | 1. Đọc lại tin nhắn nhóm Zalo điều phối · 2. Lọc các đầu việc chưa hoàn thành · 3. Nhập vào file Word nhật ký ca · 4. Gửi email bàn giao |
| **Bottleneck** | Bước 1 & 2 (lọc tin nhắn Zalo thủ công mất 20 phút) |
| **Impact** | Tốn 30 phút/ca trực; nguy cơ bỏ sót sự cố xe chưa được cứu hộ sang ca sau |
| **Success metric** | Giảm thời gian tổng hợp từ 30 phút xuống dưới 5 phút/ca |
| **Phương án không dùng AI** | Tạo bảng Google Form / Sheet để ghi nhận sự cố theo thời gian thực thay vì gõ tự do vào Zalo |
| **Giả thuyết về AI** | AI tự động quét thread chat và trích xuất danh sách sự cố mở (Open issues) |
| **Cảm nhận nhanh** | Workflow |

```text
HIỆN TẠI — 30 phút / ca bàn giao

[1. Đọc Zalo nhóm: 15'] → [2. Lọc sự cố tồn đọng: 10'] ← BOTTLENECK
→ [3. Gõ file Word: 5']
```

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (Bàn giao ca trực) và tham gia thảo luận. | Giúp nhóm nhận diện quy trình bàn giao thông tin trong ca trực của điều phối viên. |
| Phản biện bài của bạn khác | Đặt câu hỏi cho Hiệp: *"Nếu chỉ tìm trạm sạc, tại sao app tài xế không tự làm mà phải qua điều phối viên?"* | Buộc Hiệp phải làm rõ ranh giới: App chỉ xử lý pin > 10%; khi pin < 5% nguy cấp cần điều xe cứu hộ thì bắt buộc phải có điều phối viên can thiệp. |
| Kiểm chứng thực tế (CP4) | Trực tiếp phụ trách khâu phỏng vấn The Mom Test: phỏng vấn 3 đối tượng (Tài xế VF e34, Điều phối viên ca, Kỹ thuật viên xe sạc lưu động). | Thu được các câu nói nguyên văn đắt giá và tín hiệu phản bác: 100% phản đối AI tự động điều xe cứu hộ. |
| Cây OST & Quyết định | Cùng nhóm xây dựng cây OST rút gọn và thống nhất chọn Candidate #1 của Hiệp. | Thống nhất được outcome và các opportunity cốt lõi không bị lẫn solution. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tìm thêm góc nhìn về nghiệp vụ CSKH xe điện. | Gợi ý ý tưởng tra cứu chính sách cọc pin PDF. | Gợi ý chatbot toàn năng giải quyết mọi việc. | Bỏ gợi ý chung chung, chỉ giữ lại bài toán đọc PDF. |
| CP4 Kiểm chứng | Soạn bộ câu hỏi phỏng vấn theo phong cách The Mom Test. | Nhắc nhở không được dùng câu hỏi tương lai "Bạn có muốn...". | Gợi ý câu hỏi vẫn mang tính khảo sát ý kiến. | Sửa lại thành các câu hỏi về hành vi quá khứ: *"Lần gần nhất xảy ra khi nào, mất bao lâu?"*. |

---

## 6. Reflection (CP7)

### 6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?
Khi nghe Hiệp trình bày về sự cố pin Xanh SM và Linh trình bày về quy trình bảo hiểm va chạm, tôi thấy các vấn đề ngoài hiện trường luôn có mức độ rủi ro và áp lực thời gian lớn hơn rất nhiều so với các vấn đề văn phòng hay học tập. Bài toán của Hiệp nổi bật vì tính tức thời và an toàn tính mạng.

### 6.2. Nhóm có lúc nào bị "solution-first" không?
Có, khi bắt đầu CP3, tôi đã nghĩ ngay đến việc tạo một con Bot tự động đọc Zalo rồi xuất ra báo cáo. Cả nhóm sau đó nhận ra rằng vấn đề cốt lõi là việc thông tin bị phân mảnh, và giải pháp căn cơ có thể chỉ là đổi sang dùng Google Form (No AI) chứ chưa chắc đã cần AI.

### 6.3. Tôi có đổi ý sau khi bị phản biện không?
Tôi đã đổi ý khi nhận ra bài toán bàn giao ca của mình hoàn toàn có thể giải quyết bằng một quy trình nhập liệu kỷ luật trên Google Sheet (No AI) mà không cần dùng đến LLM để đọc Zalo. Do đó, tôi đã hoàn toàn ủng hộ việc nhóm chọn đề tài Sự cố pin của Hiệp.

### 6.4. Kết quả kiểm chứng có làm tôi bất ngờ không?
Rất bất ngờ khi phỏng vấn anh điều phối viên Hub Long Biên: anh ấy mở cùng lúc 3 tab trình duyệt và phải ghi nhớ thông số trong đầu vì các phần mềm không kết nối với nhau. Nỗi đau thao tác tay của người lao động lớn hơn nhiều so với những gì chúng tôi tưởng tượng khi ngồi trong phòng học.

### 6.5. Điều khó nhất khi viết Problem Statement là gì?
Khó nhất là xác định Boundary: vạch ra ranh giới rõ ràng những việc AI KHÔNG ĐƯỢC làm. Rất dễ bị cám dỗ cho AI làm thêm việc này việc kia, nhưng trong môi trường vận hành an toàn, càng hạn chế quyền của AI thì hệ thống càng tin cậy.

### 6.6. Nếu làm lại, tôi sẽ đổi gì?
Tôi sẽ đi phỏng vấn thêm cả đại diện phía trạm sạc V-GREEN để hiểu rõ hơn về tình trạng trụ sạc báo ảo trên hệ thống.

---

### 6.7. Hiểu bài

1. **Problem:** Điều phối viên Xanh SM mất 15 phút xử lý thủ công mỗi ca xe báo pin thấp, gây nguy cơ xe chết máy giữa đường.
2. **Quy trình:** Hiện tại gồm 5 bước tra cứu phân mảnh giữa telemetry xe và bản đồ trạm sạc.
3. **Metric:** Giảm thời gian xử lý xuống dưới 5 phút, tỷ lệ duyệt nháp $\ge 85\%$, vi phạm an toàn pin $0\%$.
4. **Boundary:** AI không tự phát lệnh điều xe cứu hộ, cấm chỉ dẫn xe chạy tiếp khi pin $< 5\%$.
5. **Mức can thiệp AI:** Workflow bán tự động (Rule an toàn + AI soạn nháp + Người duyệt 1-click).
6. **Quyết định:** Go, phạm vi nhỏ thông qua pilot 2 tuần tại Hub Long Biên có ngưỡng dừng nghiêm ngặt.

---

## 7. Tài liệu tham khảo

1. Fitzpatrick, R. (2013). *The Mom Test*. Founder Centric.
2. Torres, T. (2021). *Continuous Discovery Habits*. Product Talk LLC.
