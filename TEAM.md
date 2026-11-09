# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- **Tên nhóm:** NhomBB (Lớp K5 · L3B)
- **Candidate problem nhóm chọn (1 câu):** Xây dựng quy trình hỗ trợ điều phối viên vận hành đội xe taxi điện Xanh SM tự động tổng hợp telemetry, kiểm tra quy tắc an toàn và soạn nháp phương án xử lý sự cố pin thấp dưới 10%, giúp giảm thời gian điều phối từ 15 phút xuống dưới 5 phút mà vẫn đảm bảo 100% quyết định do con người kiểm duyệt.
- **Quyết định cuối (Go / Not Yet / No-Go):** **Go, phạm vi nhỏ** (Pilot 2 tuần tại Hub điều phối Long Biên).

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Đào Văn Hiệp | 2A202603813 | Nhóm trưởng, Điều phối chung, Phụ trách Problem Scoping & Problem Statement | [Lmeo2h](https://github.com/Lmeo2h) |
| 2 | Nguyễn Đức Minh | 2A202601245 | Phụ trách Kiểm chứng (Phỏng vấn Mom Test & Khảo sát thực tế) | [ducminh-vinuni](https://github.com/ducminh-vinuni) |
| 3 | Trần Phương Linh | 2A202603189 | Phụ trách Research đối chuẩn công nghệ & Đánh giá 4 Rủi ro | [linhtran-vinuni](https://github.com/linhtran-vinuni) |
| 4 | Phạm Quốc Huy | 2A202602734 | Người phản biện chính, Phụ trách Mức can thiệp AI & Bộ tiêu chí Eval | [huyquoc-pham](https://github.com/huyquoc-pham) |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Đào Văn Hiệp | Phạm Quốc Huy | Bảng pitch 12 candidate, phân cụm Cluster, cây OST rút gọn, Bảng chấm điểm 7 tiêu chí |
| CP4 — Kiểm chứng | Nguyễn Đức Minh | Đào Văn Hiệp | Assumption Map 5 giả định, 5 Interview Snapshots thực tế, tổng hợp xác nhận/phản bác |
| CP4 — Research | Trần Phương Linh | Nguyễn Đức Minh | Bảng research 4 giải pháp quốc tế (Tesla, Geotab, Jira, n8n) có link chính thức |
| CP5 — Quy trình trước/sau | Đào Văn Hiệp | Trần Phương Linh | Sơ đồ quy trình hiện tại & tương lai (Mermaid + hình ảnh), Bảng so sánh Before/After |
| CP5 — Problem Statement v0 | Đào Văn Hiệp | Phạm Quốc Huy | Problem Statement v0 6 trường, nhật ký nhận phản biện từ AI |
| CP6 — Mức can thiệp + Problem Statement v1 | Phạm Quốc Huy | Đào Văn Hiệp | Ma trận độ mơ hồ/phức tạp, So sánh 4 mức, AI Canvas, Câu hỏi PAIR, 5 Eval Criteria, Problem Statement v1 |
| CP6 — Quyết định | Trần Phương Linh | Nguyễn Đức Minh | Đánh giá 4 rủi ro Marty Cagan, Kết luận Go kèm Pilot nhỏ nhất & Ngưỡng dừng (Stopping Threshold) |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

---

### DaoVanHiep-2A202603813

**Phần việc phụ trách:**
- Điều phối chung tiến độ làm việc của nhóm, quản lý GitHub repo.
- Đề xuất Candidate #1 (Sự cố pin thấp Xanh SM), pitch và bảo vệ trước phản biện của nhóm.
- Chịu trách nhiệm chính xây dựng Sơ đồ quy trình Hiện tại & Tương lai (CP5), viết Problem Statement v0 và phối hợp hoàn thiện v1.

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Xây dựng 10 problem scan cá nhân (CP1) và 3 Problem Card chi tiết (CP2).
- Trực tiếp vẽ sơ đồ quy trình hiện tại 5 bước (15 phút) và sơ đồ tương lai dạng Mermaid kết hợp Rule + AI + Human Review (~ 3 phút).
- Viết bản dự thảo Problem Statement v0 với đầy đủ 6 trường dữ liệu chuẩn, tiếp thu phản biện AI để bổ sung chỉ số an toàn vào v1.
- Biên soạn tài liệu chi tiết quy trình tương lai tại [report/assets/cp5-workflow-diagram.png](report/assets/cp5-workflow-diagram.png).

**Bằng chứng (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):**
- Báo cáo nhóm: Mục 1, Mục 2 (Candidate #1, Cây OST), Mục 4 (Quy trình trước/sau), Mục 5 (Problem Statement v0).
- File phụ lục: `report/assets/cp5-workflow-diagram.png`.
- Commit lịch sử khởi tạo và cập nhật quy trình trên GitHub repo.

**Điều mình học được từ phần nhóm:**
- Trước đây tôi hay có thói quen nghĩ ngay đến việc "xây một AI Agent tự động hóa tất cả". Qua bài lab này và sự phản biện gay gắt của các bạn trong nhóm, tôi nhận ra bài toán an toàn vận hành xe điện là tối thượng: nếu để AI tự quyết, rủi ro tai nạn và chi phí cứu hộ sẽ giết chết sản phẩm. Mức can thiệp Workflow bán tự động có con người duyệt (HITL) mới là lời giải đúng đắn và khả thi nhất.

---

### NguyenDucMinh-2A202601245

**Phần việc phụ trách:**
- Phụ trách khâu Kiểm chứng thực tế (CP4): Thiết lập Assumption Map, thiết kế câu hỏi phỏng vấn theo chuẩn The Mom Test.
- Trực tiếp tiến hành phỏng vấn sâu 3/5 đối tượng (Tài xế VF e34, Điều phối viên Hub Long Biên, Kỹ thuật viên xe sạc lưu động).
- Thực hiện khảo sát nhanh qua Google Form với 22 tài xế Xanh SM trong nhóm Zalo.

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Soạn thảo Assumption Map 5 giả định và xác định các giả định rủi ro cao nhất cần kiểm chứng ngay.
- Hoàn thành tài liệu 5 Interview Snapshots chi tiết tại [report/assets/cp4-interview-snapshots.md](report/assets/cp4-interview-snapshots.md).
- Trích xuất được "tín hiệu phản bác" cực kỳ đắt giá: 100% người được hỏi kiên quyết phản đối việc AI tự động bắn lệnh điều xe cứu hộ, buộc nhóm phải từ bỏ mức Agent để quay về Workflow.

**Bằng chứng (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):**
- Báo cáo nhóm: Mục 3.1 (Assumption Map), Mục 3.2 (Kiểm chứng thực tế).
- File phụ lục: `report/assets/cp4-interview-snapshots.md`.

**Điều mình học được từ phần nhóm:**
- Kỹ năng phỏng vấn theo The Mom Test thật sự thay đổi tư duy của tôi: không bao giờ được hỏi "Bạn có thích một công cụ AI như thế này không?" (vì họ luôn khen xã giao), mà phải hỏi về những gì họ đã trải qua trong quá khứ ("Lần gần nhất bạn xử lý việc đó mất bao lâu, chuyện gì tồi tệ đã xảy ra?"). Dữ liệu thật đã cứu nhóm một bàn thua trông thấy khi suýt chút nữa chọn giải pháp Agent tự trị quá phi thực tế.

---

### TranPhuongLinh-2A202603189

**Phần việc phụ trách:**
- Phụ trách Research đối chuẩn thị trường (CP4): Khảo sát 4 giải pháp công nghệ tương tự trên thế giới (Tesla, Geotab, Jira, n8n).
- Chịu trách nhiệm phân tích 4 Rủi ro (Value, Usability, Feasibility, Viability) theo Marty Cagan (CP6).
- Soạn thảo đề xuất kế hoạch Pilot nhỏ nhất trong 2 tuần và xác lập Ngưỡng dừng an toàn (Stopping Threshold).

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Tự tay tra cứu, mở và kiểm chứng 4 đường link chính thức của các nền tảng công nghệ, phân tích rõ bước nào họ đã giải quyết và bước nào còn bỏ trống.
- Viết bảng phân tích 4 rủi ro với các bằng chứng thực tế thu thập từ khâu kiểm chứng.
- Đề xuất kịch bản "Kill Switch" (Ngưỡng dừng an toàn): Nếu AI có 1 lần duy nhất gợi ý sai khiến xe dưới 5% pin tiếp tục chạy và chết máy, pilot lập tức bị hủy bỏ.

**Bằng chứng (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):**
- Báo cáo nhóm: Mục 3.3 (Research giải pháp đã có), Mục 8 (Đánh giá 4 rủi ro và Quyết định).

**Điều mình học được từ phần nhóm:**
- Bài học lớn nhất của tôi là: "Đừng phát minh lại bánh xe". Khi research Tesla Fleet API và n8n, tôi nhận thấy các khối công nghệ nền tảng (thu thập telemetry, webhook, luồng tự động) thế giới đã làm rất hoàn hảo rồi. Điểm khác biệt mang lại giá trị của nhóm chúng tôi không phải là viết code mô hình từ đầu, mà là đóng gói đúng quy trình nghiệp vụ đặc thù của xe điện Xanh SM kèm lớp bảo vệ an toàn nghiêm ngặt.

---

### PhamQuocHuy-2A202602734

**Phần việc phụ trách:**
- Giữ vai trò Người phản biện chính (Devil's Advocate) trong toàn bộ các buổi thảo luận của nhóm.
- Chịu trách nhiệm phân tích mức can thiệp AI: Điền AI Canvas rút gọn, trả lời 2 câu hỏi thiết kế của Google PAIR (CP6).
- Thiết lập 5 tiêu chí đánh giá chất lượng (Eval Criteria) và xây dựng bộ dữ liệu 10 test cases kiểm thử (CP6 - Bonus B3).

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Đặt ra các câu hỏi phản biện sắc bén ở CP3, giúp nhóm loại bỏ các đề tài solution trá hình (như chatbot tự động điều xe hay dự báo nhu cầu quá rộng).
- Hoàn thành AI Canvas 6 thành phần và phân tích lựa chọn giữa Augment vs Automate, False Positive vs False Negative.
- Xây dựng trọn vẹn bộ dữ liệu kiểm thử 10 test case mẫu tại [report/assets/cp6-eval-dataset.md](report/assets/cp6-eval-dataset.md) với tỷ lệ đạt 10/10.

**Bằng chứng (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):**
- Báo cáo nhóm: Mục 6 (Mức can thiệp AI, AI Canvas, PAIR), Mục 7.3 (Tiêu chí đánh giá).
- File phụ lục: `report/assets/cp6-eval-dataset.md`.

**Điều mình học được từ phần nhóm:**
- Vai trò phản biện giúp tôi hiểu rằng một ý tưởng AI hay không nằm ở việc dùng mô hình LLM to bao nhiêu, mà nằm ở chỗ nó có một bộ Eval đo lường được ranh giới đúng/sai hay không. Nhờ thiết lập 5 tiêu chí eval chặt chẽ, nhóm đã kiểm soát được hoàn toàn hiện tượng ảo giác thông tin và biến bản nháp AI thành một công cụ hỗ trợ trực quan, đáng tin cậy cho điều phối viên.
