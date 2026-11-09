# Báo cáo cá nhân — 2A202602734_PhamQuocHuy

> Đổi tên file theo quy tắc `MSSV_HoTen.md`. Tiêu đề: `Báo cáo cá nhân — 2A202602734_PhamQuocHuy`.  
> Báo cáo hoàn chỉnh các phần cá nhân: CP1 (Scan problem), CP2 (Top 3 Problem Cards), CP3 (Nhật ký phản biện), CP7 (Reflection & Hiểu bài).

---

## 1. Thông tin học viên

- **Họ tên:** Phạm Quốc Huy
- **MSSV:** 2A202602734
- **Tên nhóm:** NhomBB (Lớp K5 · L3B)
- **Link repo nhóm:** [https://github.com/Lmeo2h/K5-L3B-DAY02-NhomBB-DiscoveryProblemFraming](https://github.com/Lmeo2h/K5-L3B-DAY02-NhomBB-DiscoveryProblemFraming)

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi bắt đầu khung giờ cao điểm mưa gió, tôi muốn dự báo khu vực nào sẽ thiếu xe nghiêm trọng trong 30 phút tới, để điều phối xe từ khu vực thừa sang đón khách | Quản lý điều vận khu vực, Hành khách | Mất 15–20 phút quan sát biểu đồ nhiệt (heatmap) và kinh nghiệm cá nhân; tỷ lệ hủy chuyến giờ mưa tăng lên 25% |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi tài xế báo trụ sạc bị lỗi ngắt sạc giữa chừng, tôi muốn đọc nhanh mã lỗi kỹ thuật từ xa, để quyết định reset trụ sạc hay cử thợ đến sửa | Kỹ thuật viên vận hành trạm sạc V-GREEN | Mất 10 phút tra mã lỗi hexadecimal trong tài liệu kỹ thuật; trung bình 12 sự cố/ngày tại cụm trạm nội đô |
| 3 | Lặp lại | Khi nhận hàng trăm hồ sơ ứng tuyển tài xế taxi mỗi đợt, tôi muốn kiểm tra nhanh tính hợp lệ của bằng lái B2 và lý lịch tư pháp, để mời ứng viên đạt chuẩn vào phỏng vấn | Chuyên viên tuyển dụng nhân sự GSM | Mất 5 phút/hồ sơ đối soát thủ công trên cổng thông tin GPLX; đợt cao điểm nhận 500 hồ sơ/tuần |
| 4 | Tốn thời gian | Khi xe taxi điện báo pin < 10% giữa đường, tôi muốn nhanh chóng tra cứu vị trí trạm sạc còn chỗ hoặc xe sạc lưu động gần nhất, để gửi chỉ dẫn cứu hộ cho tài xế trước khi xe sập nguồn | Điều phối viên GSM, Tài xế | Xử lý thủ công mất 15 phút/ca; 1 ca trực tiếp nhận 15–20 ca pin đỏ; nguy cơ chết máy giữa đường |
| 5 | Pain từ người khác | Khi sinh viên trong nhóm không chịu nộp phần việc đúng hạn, tôi muốn có công cụ tự động nhắc việc kèm cảnh báo tiến độ, để đồ án nhóm không bị trễ hạn | Trưởng nhóm đồ án, Thành viên | Mỗi tuần mất 45 phút nhắn tin riêng đôn đốc từng bạn; nhóm từng bị nộp muộn bài lab trước 15 phút |
| 6 | Lặp lại | Khi giải bài tập môn Machine Learning, tôi muốn tự động so khớp kết quả ma trận nhầm lẫn (confusion matrix) với barem đáp án, để biết code mình sai ở đâu | Sinh viên | Mất 20 phút bấm máy tính kiểm tra lại từng công thức precision/recall |

**Dùng AI gợi ý thêm:** Tôi giữ lại ý #6 cho việc học tập. Tôi bỏ ý "Hệ thống AI tự động lái xe taxi tránh điểm kẹt đường" do AI gợi ý vì quá viển vông và không nằm trong phạm vi buổi lab.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Dự báo khu vực thiếu xe taxi giờ cao điểm (#1) | Tác động kinh tế rất lớn, giúp tăng doanh thu cuốc xe | Dữ liệu chuỗi thời gian quá lớn, không khả thi trong lab 4 tiếng |
| 2 | Chẩn đoán mã lỗi trụ sạc xe điện (#2) | Giúp giải phóng trụ sạc nhanh, tăng tỷ lệ sạc thành công | Cần quyền truy cập vào firmware phần cứng trụ sạc V-GREEN |
| 3 | Tự động xác thực bằng lái tài xế mới (#3) | Tiết kiệm công sức tuyển dụng quy mô lớn | Đã có các giải pháp eKYC/OCR sẵn có trên thị trường |

---

### Problem Card #1 — Dự báo khu vực thiếu xe taxi giờ cao điểm

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi bắt đầu khung giờ cao điểm mưa gió, tôi muốn dự báo khu vực nào sẽ thiếu xe nghiêm trọng trong 30 phút tới, để điều phối xe từ khu vực thừa sang đón khách |
| **Actor** | Quản lý điều vận đội xe GSM khu vực Hà Nội |
| **Thời điểm / bối cảnh** | Đầu các khung giờ cao điểm (7h–8h30 sáng và 17h–19h chiều) khi thời tiết xấu |
| **Quy trình hiện tại** | 1. Mở bản đồ heatmap mật độ cuốc xe · 2. Quan sát lịch sử và kinh nghiệm cá nhân · 3. Dự đoán các quận thiếu xe · 4. Phát thông báo Zalo khuyến khích tài xế di chuyển sang khu vực đó |
| **Bottleneck** | Bước 2 & 3 (phân tích thủ công thiếu chính xác, mất 15–20 phút, lúc dự đoán xong thì đường đã tắc cứng không di chuyển xe được) |
| **Impact** | Tỷ lệ hủy chuyến do không tìm thấy xe tăng vọt lên 25%; mất doanh thu ước tính hàng trăm triệu đồng mỗi ngày mưa |
| **Success metric** | Dự báo chính xác nhu cầu thiếu xe trước 30 phút với độ chính xác $\ge 80\%$; giảm tỷ lệ hủy chuyến xuống dưới 10% |
| **Phương án không dùng AI** | Thiết lập biểu đồ thống kê cố định theo các ngày mưa trong quá khứ để phân bổ sẵn xe từ trước |
| **Giả thuyết về AI** | Mô hình học máy dự báo chuỗi thời gian (Time-series) kết hợp dữ liệu thời tiết và lịch sử đặt xe |
| **Cảm nhận nhanh** | Machine Learning chuyên sâu (vượt quá phạm vi lab LLM) |

```text
HIỆN TẠI — 20 phút / lần phân tích

[1. Mở heatmap: 2'] → [2. Đọc & suy luận kinh nghiệm: 10'] ← BOTTLENECK
→ [3. Chọn quận thiếu xe: 5'] → [4. Bắn tin Zalo: 3']
```

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch Card #1 (Dự báo nhu cầu xe) với lập luận về doanh thu lớn. | Nhóm thảo luận sôi nổi nhưng chỉ ra tính bất khả thi về dữ liệu trong thời gian lab. |
| Người phản biện chính (Devil's Advocate) | Đặt câu hỏi phản biện gắt gao cho các thành viên: *"Đề tài này có thật sự cần AI không hay chỉ cần script Excel? Lỡ AI ảo giác thì hậu quả là gì?"*. | Giúp nhóm loại bỏ các đề tài viển vông và tập trung vào bài toán pin với boundary chặt chẽ. |
| Thiết kế Mức can thiệp AI (CP6) | Điền AI Canvas rút gọn, trả lời 2 câu hỏi Google PAIR (chọn Augment và ưu tiên tránh False Negative). | Định hình rõ ràng cấu trúc Workflow bán tự động với vai trò con người phê duyệt 1-click. |
| Xây dựng Bộ tiêu chí Eval & 10 Test cases (CP6) | Thiết lập 5 tiêu chí đánh giá nghiêm ngặt và trực tiếp xây dựng bộ dữ liệu 10 test case mẫu tại [report/assets/cp6-eval-dataset.md](../assets/cp6-eval-dataset.md) (Bonus B3). | Cung cấp công cụ đo lường định lượng chính xác để đánh giá đầu ra của mô hình AI. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tìm thêm góc nhìn về nghiệp vụ chẩn đoán kỹ thuật xe điện. | Gợi ý bài toán đọc mã lỗi trạm sạc (#2). | Gợi ý ý tưởng AI tự lái xe taxi tránh kẹt đường. | Tôi gạt bỏ ngay ý tưởng tự lái vì hoàn toàn phi thực tế đối với sinh viên. |
| CP6 Mức can thiệp | Hỗ trợ phân tích câu hỏi False Positive vs False Negative của Google PAIR. | Giúp phân biệt rõ hậu quả của việc "báo nhầm" và "bỏ sót" trong an toàn pin. | Cho rằng việc báo nhầm pin yếu sẽ gây thiệt hại nặng nề hơn. | Tôi phản biện lại: Bỏ sót nguy cơ xe sập nguồn trên cao tốc nguy hiểm hơn gấp trăm lần việc báo động sớm một chút. |
| CP6 Eval | Soạn thảo 10 kịch bản test case đánh giá mô hình. | Giúp sinh nhanh các tọa độ GPS và thông số telemetry giả lập. | Các kịch bản ban đầu quá dễ, không có các trường hợp ngoại lệ (corner cases). | Tôi tự thêm vào các ca hóc búa: xe mất GPS trong hầm, pin đúng 4.8% sát biên, trụ sạc bảo trì, v.v. |

---

## 6. Reflection (CP7)

### 6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?
Giữ vai trò là người phản biện chính trong nhóm, khi nghe bài của Hiệp, Minh và Linh, tôi học được rằng **một bài toán hay không phải là bài toán dùng công nghệ phức tạp nhất, mà là bài toán có quy trình định lượng rõ nhất**. Bài dự báo của tôi nghe rất "ngầu" nhưng mù mờ về dữ liệu, trong khi bài sự cố pin của Hiệp có từng bước với số phút đo lường chính xác, giúp việc thiết kế giải pháp và tiêu chí eval trở nên vô cùng mạch lạc.

### 6.2. Nhóm có lúc nào bị "solution-first" không?
Chính bản thân tôi là người suýt làm nhóm rơi vào bẫy này khi liên tục đề xuất: *"Hãy làm một hệ thống Multi-Agent tự động hoàn toàn đi!"*. Rất may là các bạn trong nhóm đã dùng framework của Anthropic để "bẻ" lại tôi: Agent chỉ dùng khi bước tiếp theo không đoán trước được; ở đây quy trình điều phối đã có 5 bước định sẵn, dùng Workflow là chuẩn nhất. Tôi hoàn toàn bị thuyết phục.

### 6.3. Tôi có đổi ý sau khi bị phản biện không?
Tôi đã đổi ý 180 độ về đề tài của mình. Ban đầu tôi rất bảo thủ muốn làm bài toán Dự báo nhu cầu xe. Nhưng khi Hiệp chất vấn: *"Bạn lấy đâu ra dữ liệu thời gian thực của 3.000 xe taxi chạy ngoài đường để train mô hình trong chiều nay?"*, tôi cứng họng và nhận ra mình đang mộng tưởng trên mây. Tôi đã vui vẻ đồng ý chuyển sang hỗ trợ Hiệp làm đề tài pin Xanh SM.

### 6.4. Kết quả kiểm chứng có làm tôi bất ngờ không?
Tôi rất bất ngờ khi thấy kết quả khảo sát 22 tài xế: có tới gần 90% từng trải qua cảm giác hoảng loạn khi pin báo đỏ dưới 10%. Điều đó chứng minh đây là một nỗi đau có thật 100%, không phải sản phẩm tưởng tượng của sinh viên trong phòng lab.

### 6.5. Điều khó nhất khi viết Problem Statement là gì?
Khó nhất là xây dựng bộ tiêu chí đánh giá (Eval Criteria). Khi làm việc với LLM, rất khó để định nghĩa thế nào là một câu trả lời "đạt". Việc lượng hóa thành 5 tiêu chí: Đúng số liệu, Tuân thủ an toàn < 5%, Khả thi trạm sạc, Không ảo giác, và Chuẩn format là một thử thách trí tuệ thực sự nhưng mang lại giá trị rất cao.

### 6.6. Nếu làm lại, tôi sẽ đổi gì?
Nếu làm lại, tôi sẽ xây dựng bộ test case eval gồm 30–50 trường hợp thay vì 10 trường hợp để kiểm thử khả năng chống chịu của mô hình trước các tình huống tấn công prompt injection từ phía tài xế.

---

### 6.7. Hiểu bài

1. **Problem:** Điều phối viên Xanh SM mất 15 phút xử lý thủ công mỗi ca xe báo pin thấp, gây nguy cơ xe chết máy dừng giữa đường.
2. **Quy trình:** Hiện tại gồm 5 bước tra cứu phân mảnh giữa telemetry xe và bản đồ trạm sạc.
3. **Metric:** Giảm thời gian xử lý xuống dưới 5 phút, tỷ lệ duyệt nháp $\ge 85\%$, vi phạm an toàn pin $0\%$.
4. **Boundary:** AI không tự phát lệnh điều xe cứu hộ, cấm chỉ dẫn xe chạy tiếp khi pin $< 5\%$.
5. **Mức can thiệp AI:** Workflow bán tự động (Rule an toàn + AI soạn nháp + Người duyệt 1-click).
6. **Quyết định:** Go, phạm vi nhỏ thông qua pilot 2 tuần tại Hub Long Biên có ngưỡng dừng nghiêm ngặt.

---

## 7. Tài liệu tham khảo

1. Google PAIR. (2019). *People + AI Guidebook*. [https://pair.withgoogle.com/guidebook/](https://pair.withgoogle.com/guidebook/)
2. Anthropic. (2024). *Building Effective Agents*. [https://www.anthropic.com/research/building-effective-agents](https://www.anthropic.com/research/building-effective-agents)
