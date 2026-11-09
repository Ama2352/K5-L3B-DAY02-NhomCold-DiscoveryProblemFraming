# Team

## Thông tin nhóm

- Tên nhóm: Cold
- Candidate problem nhóm chọn (1 câu): Khi tiếp nhận yêu cầu bồi thường kèm hình ảnh xe tai nạn, nhân viên giám định muốn xác định bộ phận hư hỏng và ước lượng chi phí sửa chữa, để có cơ sở đánh giá mức bồi thường và tư vấn khách hàng.
- Quyết định cuối (Go / Not Yet / No-Go): Chưa chốt; đánh giá tại CP6 sau khi kiểm chứng bài toán.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Vũ Lương Duy | 2A202603945 | Tổng hợp hội tụ và quyết định | vuduy21 |
| 2 | Nguyễn Thảo Quyên | 2A202603895 | Phụ trách research, hỗ trợ làm rõ nghiệp vụ | |
| 3 | Hồ Nguyễn Minh Sang | 2A202603905 | Phụ trách quy trình, metric và Problem Statement v0 | |
| 4 | Mai Danh Hiếu | 2A202603948 | Phụ trách kiểm chứng, hỗ trợ quy trình | |

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Vũ Lương Duy | Cả nhóm | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Mai Danh Hiếu | Hồ Nguyễn Minh Sang | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Thảo Quyên | Vũ Lương Duy | Bảng research có link |
| CP5 — Quy trình trước/sau | Hồ Nguyễn Minh Sang | Mai Danh Hiếu | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Hồ Nguyễn Minh Sang | Nguyễn Thảo Quyên | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Vũ Lương Duy | Cả nhóm | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Vũ Lương Duy | Cả nhóm | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

### VuLuongDuy-2A202603945

**Phần việc phụ trách:**

- Tổng hợp hội tụ CP3; tổng hợp mức can thiệp, Problem Statement v1 và quyết định CP6.
- Hỗ trợ research CP4.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Báo cáo cá nhân có scan và ba card về chép đơn từ inbox, tồn kho đa kênh và đăng sản phẩm.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603945_VuLuongDuy.md).

**Điều mình học được từ phần nhóm:**

*Bản gợi ý để thành viên tự đối chiếu với trải nghiệm của mình:*

- Hội tụ cần dựa trên actor, quy trình, bằng chứng và khả năng đo tác động; tổng điểm giúp giải thích lựa chọn nhưng không thay thế thảo luận về các giả định còn thiếu.
- Candidate được chọn chỉ xác định bài toán cần đào sâu, chưa đồng nghĩa với quyết định triển khai. Kết luận Go, Not Yet hoặc No-Go phải nhất quán với bằng chứng và bốn rủi ro.
- Với bài toán dự toán sửa chữa, cần so sánh checklist và bảng giá chuẩn hóa trước khi chọn mức hỗ trợ phức tạp hơn; số liệu ước lượng không được dùng làm bằng chứng hiệu quả đã đạt.

### NguyenThaoQuyen-2A202603895

**Phần việc phụ trách:**

- Research CP4 và hỗ trợ làm rõ quy trình đánh giá hư hỏng, tra cứu phụ tùng và chi phí.
- Hỗ trợ Problem Statement v0.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Báo cáo cá nhân có ba card về đánh giá hư hỏng và chi phí, tra cứu phụ tùng, kiểm tra bài tập.
- Card #1 là candidate nhóm chọn để phân tích tiếp.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603895_NguyenThaoQuyen.md).
- [Báo cáo nhóm, mục 2.4 — Candidate được chọn](report/team/group_report.md).

**Điều mình học được từ phần nhóm:**

*Bản gợi ý để thành viên tự đối chiếu với trải nghiệm của mình:*

- Bài toán xác định hư hỏng cần tách rõ nhận diện bộ phận, đối chiếu phụ tùng và tra giá. Gộp cả ba thành một bottleneck sẽ khó xác định bước nào thực sự cần cải thiện.
- Có công cụ nhận diện ảnh không đồng nghĩa với việc lập được dự toán đáng tin cậy. Cần kiểm tra phạm vi dữ liệu, phụ tùng tương thích, nguồn giá và vai trò xác nhận của người giám định.
- Research cần chỉ ra công cụ giải được bước nào và còn thiếu gì trong quy trình. Đề xuất Agent ở card ban đầu chỉ là giả thuyết; kiến trúc phải được xem xét lại sau kiểm chứng.

### HoNguyenMinhSang-2A202603905

**Phần việc phụ trách:**

- Quy trình trước/sau, metric và Problem Statement v0 ở CP5.
- Hỗ trợ kiểm chứng CP4.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Báo cáo cá nhân có ba card về ghi chú họp, chốt sổ nhà trọ và hiểu khái niệm khi research.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603905_HoNguyenMinhSang.md).

**Điều mình học được từ phần nhóm:**

- Tôi học được cách bắt đầu từ tình huống, nhu cầu và quy trình hiện tại trước khi nghĩ đến công cụ. Với bài toán nhóm chọn, cần làm rõ nhân viên giám định vướng ở bước xác định hư hỏng, tra phụ tùng hay tra giá, rồi mới so sánh các cách hỗ trợ.
- Khi xem lại cây OST, tôi phân biệt rõ hơn giữa pain và solution: “phải tra giá từ nhiều nguồn” là khó khăn cần giải quyết, còn “nhận diện bằng Computer Vision” hay “Agent tự xử lý hồ sơ” là cách giải, không đặt ở tầng opportunity.
- Tôi nhận ra bottleneck phải khớp với cách công việc thực sự diễn ra. Ở card ghi chú họp, điểm chưa rõ được hỏi ngay trong cuộc họp; phần cần phân tích là công sức tổng hợp ghi chú, không mặc định thành viên phải hỏi lại sau họp. Tương tự, bài toán sửa chữa phải tách thời gian thao tác khỏi thời gian chờ phê duyệt để đo đúng vấn đề.

### MaiDanhHieu-2A202603948

**Phần việc phụ trách:**

- Kiểm chứng CP4.
- Hỗ trợ quy trình trước/sau ở CP5.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Báo cáo cá nhân có ba card về tổng hợp tiến độ, phân công và bàn giao công việc phụ thuộc.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603948_MAIDANHHIEU.md).

**Điều mình học được từ phần nhóm:**

*Bản gợi ý để thành viên tự đối chiếu với trải nghiệm của mình:*

- Kiểm chứng cần hỏi về một hồ sơ hoặc sự việc đã xảy ra, các bước thực hiện và thời gian cụ thể; lời khen dành cho ý tưởng không xác nhận rằng vấn đề đủ lớn để giải quyết.
- Với hồ sơ sửa chữa, thời gian giám định và tra cứu phải được ghi riêng với thời gian chờ phê duyệt. Mốc xử lý nhiều ngày chưa chứng minh thao tác tra cứu là bước nghẽn chính.
- Cần ghi cả trường hợp trái với giả định, chẳng hạn người xử lý đã có bảng giá và checklist đủ dùng. Những tín hiệu này giúp thu hẹp phạm vi hoặc chọn cách cải thiện đơn giản hơn.
