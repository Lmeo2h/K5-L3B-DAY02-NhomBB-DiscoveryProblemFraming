# Phụ lục CP4 — Biên bản phỏng vấn kiểm chứng (Interview Snapshots)

Tài liệu này ghi lại chi tiết 5 buổi phỏng vấn kiểm chứng thực tế theo nguyên tắc **The Mom Test** (Rob Fitzpatrick), phục vụ đề tài: **Trợ lý hỗ trợ điều phối viên xử lý sự cố pin thấp và điều phối cứu hộ đội xe Xanh SM**.

---

## Buổi phỏng vấn #1: Tài xế taxi điện Xanh SM (VF e34)

- **Người được hỏi:** Tài xế taxi Xanh SM (chạy VF e34, hơn 1.5 năm kinh nghiệm, khu vực nội thành Hà Nội).
- **Hình thức & Thời gian:** Phỏng vấn trực tiếp tại trạm sạc V-GREEN Ocean Park, 10:30 sáng Chủ nhật, thời lượng 20 phút.
- **Mục tiêu kiểm chứng:** Hành vi thực tế khi xe báo pin yếu, cách xử lý và liên hệ tổng đài điều phối.

| Trường | Chi tiết |
|---|---|
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Lúc pin xuống dưới 10% ở giữa cầu Vĩnh Tuy giờ tan tầm, điều hòa tự ngắt, xe lì ga, gọi tổng đài mà mất gần 15 phút mới có hướng dẫn đi đâu sạc, lúc đó toát mồ hôi hột chỉ sợ chết máy nằm giữa cầu."* |
| **Lần gần nhất gặp sự cố** | Thứ Ba tuần trước (khoảng 17h45), xe còn 8% pin, khách đang ngồi trên xe đi từ Time City sang Long Biên. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Bấm nút khẩn cấp trên app tài xế và gọi thẳng số hotline điều phối ca trực. Vừa lái xe vừa phải đọc số VIN, địa chỉ hiện tại và mức pin hiển thị trên taplo xe cho điều phối viên ghi lại. |
| **Mất bao lâu, bao lần?** | Mất 14 phút tính từ lúc bắt đầu gọi đến khi nhận được tin nhắn Zalo thông báo trạm sạc còn slot ở chân cầu. Trung bình 1 tháng bị cảnh báo pin đỏ 2–3 lần. |
| **Insight / Tín hiệu xác nhận** | Quy trình trao đổi qua điện thoại rất thủ công; tài xế đang lái xe rất nguy hiểm nếu phải đọc thông số; điều phối viên mất thời gian tra cứu trạm sạc còn chỗ. |
| **Tín hiệu phản bác / Lưu ý** | Tài xế nói nếu pin trên 10% thì app tài xế đã tự hiển thị gợi ý trạm sạc trên bản đồ rồi, không cần điều phối can thiệp; chỉ khi **pin < 8% hoặc có nguy cơ chết máy khẩn cấp** thì mới cần điều phối cứu hộ khẩn cấp. |

---

## Buổi phỏng vấn #2: Điều phối viên ca trực vận hành GSM

- **Người được hỏi:** Nhân viên trực ban điều phối đội xe (kinh nghiệm 10 tháng tại Hub vận hành GSM).
- **Hình thức & Thời gian:** Phỏng vấn qua Google Meet, tối thứ Bảy, thời lượng 25 phút.
- **Mục tiêu kiểm chứng:** Thao tác thực tế của điều phối viên khi tiếp nhận hồ sơ pin yếu, bottleneck thời gian.

| Trường | Chi tiết |
|---|---|
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Cái mệt nhất không phải là nghe máy, mà là tay vừa giữ tai nghe, mắt vừa phải đảo giữa 3 màn hình: 1 tab Telemetry GPS xe, 1 tab bản đồ trạm sạc V-GREEN xem còn súng sạc trống không, rồi lại mở Zalo gõ thông tin cho đội xe sạc lưu động."* |
| **Lần gần nhất xử lý hồ sơ** | Ca trực chiều hôm qua: tiếp nhận 18 ca báo pin thấp từ tài xế trong vòng 4 tiếng cao điểm mưa ngập. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Dùng một file Excel cá nhân lưu sẵn các mẫu tin nhắn (template SMS/Zalo), copy-paste tọa độ GPS và tên tài xế vào rồi gửi. |
| **Mất bao lâu, bao lần?** | Mỗi ca xử lý trung bình từ 12 đến 16 phút. Nếu gặp trạm sạc báo ảo (trên app báo còn chỗ nhưng thực tế tài xế đến nơi thì kín trụ sạc), tài xế gọi lại mắng thì mất thêm 10 phút điều phối lại. |
| **Insight / Tín hiệu xác nhận** | Bottleneck nằm ở khâu **tổng hợp dữ liệu đa nguồn** (Telemetry xe + Tình trạng trạm sạc + Vị trí xe sạc lưu động) và **soạn nội dung chỉ dẫn chuẩn xác**. |
| **Tín hiệu phản bác / Lưu ý** | Người được hỏi nhấn mạnh: *"Không được để máy tự động điều xe cứu hộ đi đâu nhé, vì xe cứu hộ sạc lưu động chi phí xuất bến rất đắt, phải có người trực ban bấm nút xác nhận."* |

---

## Buổi phỏng vấn #3: Tài xế Xanh SM Luxury (VF 8)

- **Người được hỏi:** Tài xế Xanh SM Luxury chạy xe VF 8 (chuyên tuyến sân bay Nội Bài).
- **Hình thức & Thời gian:** Phỏng vấn trực tiếp tại khu vực chờ sân bay Nội Bài, thời lượng 15 phút.
- **Mục tiêu kiểm chứng:** Hành vi khi xe điện phân khúc cao gặp sự cố pin khẩn cấp trên tuyến đường tốc độ cao.

| Trường | Chi tiết |
|---|---|
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Xe VF 8 mà pin tụt xuống dưới 5% là hệ thống tự khóa tốc độ tối đa dưới 30 km/h để bảo vệ cell pin. Lúc đó dù trạm sạc cách có 1 km cũng không bao giờ dám liều bò tới vì sợ sập nguồn giữa đường cao tốc, chỉ có đứng yên bật đèn khẩn cấp chờ xe sạc lưu động tới thôi."* |
| **Lần gần nhất gặp sự cố** | Tháng trước, chạy cao tốc Nhật Tân - Nội Bài lúc rạng sáng, pin báo ảo do thời tiết lạnh tụt từ 11% xuống 4%. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Tấp xe vào làn khẩn cấp, bật xi-nhan hazard, chụp màn hình taplo gửi vào nhóm Zalo khẩn cấp của đội xe Luxury và chờ điều phối viên gọi lại. |
| **Mất bao lâu, bao lần?** | Chờ 18 phút mới có phương án điều xe sạc lưu động xuất phát từ bãi xe Đông Anh. |
| **Insight / Tín hiệu xác nhận** | Ngưỡng pin **< 5% là ranh giới sinh tử**: không được điều xe chạy tiếp dù khoảng cách ngắn. Bắt buộc phải kích hoạt quy trình cứu hộ tại chỗ. |
| **Tín hiệu phản bác / Lưu ý** | Tài xế không quan tâm AI hay công nghệ gì, chỉ cần tin nhắn xác nhận rõ ràng: Xe cứu hộ biển số mấy, số điện thoại tài xế cứu hộ, và dự kiến bao nhiêu phút tới nơi. |

---

## Buổi phỏng vấn #4: Kỹ thuật viên xe sạc pin lưu động (Mobile Charging Van)

- **Người được hỏi:** Kỹ thuật viên vận hành xe cứu hộ sạc lưu động GSM (khu vực Cầu Giấy - Nam Từ Liêm).
- **Hình thức & Thời gian:** Phỏng vấn trực tiếp tại trạm bảo dưỡng GSM, thời lượng 20 phút.
- **Mục tiêu kiểm chứng:** Điểm nghẽn từ phía đầu tiếp nhận lệnh cứu hộ và thông tin cần thiết.

| Trường | Chi tiết |
|---|---|
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Nhiều lần điều phối viên gửi tin báo sang Zalo ghi mỗi địa chỉ chung chung kiểu 'đầu đường Tố Hữu', bọn tôi đến nơi tìm đỏ mắt không thấy xe, gọi cho tài xế thì máy tài xế hết pin sập nguồn luôn rồi. Cần nhất là tọa độ GPS chuẩn và số VIN xe."* |
| **Lần gần nhất đi cứu hộ** | 2 ngày trước, cứu hộ một xe VF 5 hết pin chết máy tại đường gom Đại lộ Thăng Long. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Nhận tin nhắn từ Zalo nhóm, tự gõ tọa độ vào Google Maps trên điện thoại để lái xe đến. |
| **Mất bao lâu, bao lần?** | Nhận lệnh sau khoảng 10–15 phút kể từ khi tài xế gặp sự cố; di chuyển tới nơi mất thêm 15–25 phút. |
| **Insight / Tín hiệu xác nhận** | Bản nháp tin nhắn điều phối bắt buộc phải chứa các trường dữ liệu cứng chuẩn hóa: Tọa độ Google Maps, Mức pin cuối ghi nhận, Số điện thoại tài xế, Model xe (e34, VF 5, VF 8) để mang đúng đầu sạc và công suất. |
| **Tín hiệu phản bác / Lưu ý** | Không phải lúc nào xe sạc lưu động cũng sẵn sàng; cần kiểm tra trạng thái xe cứu hộ (đang rảnh hay đang sạc dở cho xe khác). |

---

## Buổi phỏng vấn #5: Trưởng ca vận hành đội xe (Fleet Operations Supervisor)

- **Người được hỏi:** Giám sát vận hành ca trực GSM (quản lý 12 điều phối viên ca).
- **Hình thức & Thời gian:** Phỏng vấn trực tuyến qua Teams, chiều thứ Sáu, thời lượng 30 phút.
- **Mục tiêu kiểm chứng:** Khía cạnh kinh doanh (Viability), an toàn (Safety) và rào cản ứng dụng AI.

| Trường | Chi tiết |
|---|---|
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Mục tiêu của chúng tôi là giảm thời gian chết máy của xe để tối ưu tỷ lệ xe hoạt động (Fleet Availability). Nhưng an toàn là số 1: AI chỉ được đóng vai trò 'thư ký chuẩn bị dữ liệu và soạn nháp', tuyệt đối không trao quyền tự động ra quyết định điều động tài sản."* |
| **Số liệu vận hành thực tế** | Toàn đội xe nội thành có khoảng 2.500–3.000 xe hoạt động đồng thời; mỗi ngày ghi nhận 40–60 sự cố liên quan đến pin (trong đó 60% chỉ cần hướng dẫn trạm sạc gần nhất, 40% cần can thiệp cứu hộ lưu động). |
| **Quan điểm về tự động hóa / AI** | Rất ủng hộ việc tự động gom dữ liệu Telemetry + lọc trạm sạc + soạn nháp tin nhắn điều phối để giảm áp lực cho điều phối viên. |
| **Insight / Tín hiệu xác nhận** | Ý tưởng Workflow kết hợp Rule (kiểm tra an toàn) + AI (soạn nháp tin nhắn) + Con người (duyệt lệnh) hoàn toàn phù hợp với chính sách an toàn của GSM. |
| **Tín hiệu phản bác / Lưu ý** | Bắt buộc phải có **Ngưỡng dừng an toàn**: Nếu mô hình AI đưa ra thông tin trạm sạc không có thật hoặc sai lệch mức pin thì phải đình chỉ ngay lập tức và quay về quy trình thủ công. |

---

## Tổng kết các thay đổi quan trọng của nhóm sau 5 buổi phỏng vấn

1. **Thu hẹp phạm vi bài toán:** Nhóm không cố giải quyết mọi câu hỏi thông thường của tài xế, mà tập trung chính xác vào **tình huống khẩn cấp pin thấp (SOC < 10% và SOC < 5%)**.
2. **Quy tắc an toàn cứng (Rule-based Constraint):** Khi pin < 5%, hệ thống **cấm tuyệt đối** việc AI gợi ý tài xế tiếp tục lái xe tìm trạm, mà bắt buộc chuyển sang kịch bản: Dừng xe khẩn cấp tại vị trí an toàn + Chuẩn bị lệnh điều xe sạc lưu động.
3. **Mô hình tương tác Human-in-the-Loop:** 100% người được phỏng vấn (từ tài xế, điều phối viên đến quản lý) đều bác bỏ ý tưởng Autonomous Agent tự bắn lệnh cứu hộ; khẳng định giải pháp phải là **Workflow bán tự động** với con người là chốt chặn cuối cùng.
