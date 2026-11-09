# Team

## Thông tin nhóm

- Tên nhóm: Cold
- Candidate problem nhóm chọn (1 câu): Khi tiếp nhận yêu cầu bồi thường kèm hình ảnh xe tai nạn, nhân viên giám định muốn xác định bộ phận hư hỏng và ước lượng chi phí sửa chữa, để có cơ sở đánh giá mức bồi thường và tư vấn khách hàng.
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet — theo mục 8 báo cáo nhóm.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Vũ Lương Duy | 2A202603945 | Quy trình trước/sau và Problem Statement v0 | vuduy21 |
| 2 | Nguyễn Thảo Quyên | 2A202603895 | Mức can thiệp, Problem Statement v1 và quyết định | 100678carwyn |
| 3 | Hồ Nguyễn Minh Sang | 2A202603905 | Hội tụ nhóm CP3 | Ama2352 |
| 4 | Mai Danh Hiếu | 2A202603948 | Phỏng vấn, tổng hợp kiểm chứng và research CP4 | danhhieu204ns |

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Hồ Nguyễn Minh Sang | Cả nhóm | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Mai Danh Hiếu | Hồ Nguyễn Minh Sang | Assumption map, snapshot hoặc survey |
| CP4 — Research | Mai Danh Hiếu | Nguyễn Thảo Quyên | Bảng research có link |
| CP5 — Quy trình trước/sau | Vũ Lương Duy | Mai Danh Hiếu | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Vũ Lương Duy | Nguyễn Thảo Quyên | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Thảo Quyên | Cả nhóm | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Nguyễn Thảo Quyên | Cả nhóm | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

### VuLuongDuy-2A202603945

**Phần việc phụ trách:**

- Quy trình trước/sau và Problem Statement v0 ở CP5.
- Hỗ trợ làm rõ dữ liệu đầu vào của quy trình.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- **CP5 — Quy trình trước/sau (phụ trách chính):**
  - Vẽ quy trình hiện tại 7 bước bằng Mermaid, kèm bảng actor / input / output / thời gian từng bước. Xác định bottleneck ở bước 3–5 (xác định hư hỏng, tra mã phụ tùng, tìm giá), chiếm 20–40 trong tổng 40–60 phút/vụ.
  - Thiết kế quy trình tương lai, tách rõ bước nào Rule (checklist ảnh, lấy thông tin xe, tra bảng giá), bước nào AI (đề xuất bộ phận hư hỏng), bước nào con người (giám định viên kiểm tra, chốt giá, cấp thẩm quyền duyệt).
  - Xác định boundary: AI không quyết định mức bồi thường, không từ chối hồ sơ, không kết luận gian lận, không tự gửi kết quả, không tự đặt giá. Liệt kê các trường hợp bắt buộc chuyển giám định trực tiếp và 3 tầng phương án quay về khi AI sai.
  - Lập bảng before/after: thời gian thao tác 40–60' → ~17–20'/vụ, số bước thủ công 7/7 → 3/7, kèm rủi ro mới phát sinh.
- **CP5 — Problem Statement v0:**
  - Viết đủ 6 trường. 3 success metric có baseline, target và cách đo: thời gian bước 3–5, độ khớp danh sách hư hỏng so với giám định cuối, sai lệch chi phí sơ bộ.
  - Đưa AI phản biện và ghi lại 6 lỗ hổng để nhóm xử lý ở v1.


**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603945_VuLuongDuy.md).
- [Báo cáo nhóm, mục 4 — Quy trình trước/sau(CP5)](report/team/group_report.md).
- [Báo cáo nhóm, mục 5 — Problem Statement v0(CP5)](report/team/group_report.md).

**Điều mình học được từ phần nhóm:**

- Hội tụ cần dựa trên actor, quy trình, bằng chứng và khả năng đo tác động; tổng điểm giúp giải thích lựa chọn nhưng không thay thế thảo luận về các giả định còn thiếu.
- Candidate được chọn chỉ xác định bài toán cần đào sâu, chưa đồng nghĩa với quyết định triển khai. Kết luận Go, Not Yet hoặc No-Go phải nhất quán với bằng chứng và bốn rủi ro.
- Với bài toán dự toán sửa chữa, cần so sánh checklist và bảng giá chuẩn hóa trước khi chọn mức hỗ trợ phức tạp hơn; số liệu ước lượng không được dùng làm bằng chứng hiệu quả đã đạt.

### NguyenThaoQuyen-2A202603895

**Phần việc phụ trách:**

- Mức can thiệp, Problem Statement v1, tiêu chí đánh giá và quyết định CP6.
- Hỗ trợ làm rõ nghiệp vụ giám định xe.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Báo cáo cá nhân có ba card về đánh giá hư hỏng và chi phí, tra cứu phụ tùng, kiểm tra bài tập.
- Card #1 là candidate nhóm chọn để phân tích tiếp.
- Viết mục 6–8 báo cáo nhóm: ma trận độ mơ hồ × độ phức tạp; so sánh 4 mức và chọn Workflow (AI chỉ ở bước 3, không chọn Agent); AI Canvas và 2 câu Google PAIR.
- Viết Problem Statement v1 (khác v0 ở 4 trường: mức chọn, bottleneck, success metric, boundary) và 5 tiêu chí đánh giá (bỏ sót ≤ 15%, báo thừa ≤ 2 bộ phận/hồ sơ).
- Chấm 4 rủi ro, đề xuất Not Yet kèm 4 ngưỡng dừng; viết mục 9–10 (hạn chế, tài liệu tham khảo).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603895_NguyenThaoQuyen.md).
- [Báo cáo nhóm, mục 2.4 — Candidate được chọn](report/team/group_report.md).
- [Báo cáo nhóm, mục 6–8 — Mức can thiệp, Problem Statement v1, quyết định (CP6)](report/team/group_report.md); commit `cb85c7e` ("CP6: muc 6-10 cho card #1").

**Điều mình học được từ phần nhóm:**

- Bài toán xác định hư hỏng cần tách rõ nhận diện bộ phận, đối chiếu phụ tùng và tra giá. Gộp cả ba thành một bottleneck sẽ khó xác định bước nào thực sự cần cải thiện.
- Có công cụ nhận diện ảnh không đồng nghĩa với việc lập được dự toán đáng tin cậy. Cần kiểm tra phạm vi dữ liệu, phụ tùng tương thích, nguồn giá và vai trò xác nhận của người giám định.
- Research cần chỉ ra công cụ giải được bước nào và còn thiếu gì trong quy trình. Đề xuất Agent ở card ban đầu chỉ là giả thuyết; kiến trúc phải được xem xét lại sau kiểm chứng.

### HoNguyenMinhSang-2A202603905

**Phần việc phụ trách:**

- Tổng hợp candidate, cluster, cây OST và bảng so sánh ở CP3.
- Ghi nhận candidate nhóm chọn và lý do chọn/loại.
- Hỗ trợ Mai Danh Hiếu rà soát assumption map và interview snapshot ở CP4 — Kiểm chứng.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Báo cáo cá nhân có ba card về ghi chú họp, chốt sổ nhà trọ và hiểu khái niệm khi research.
- Tổng hợp 12 candidate của 4 thành viên, trình bày actor, bottleneck và câu hỏi chuẩn bị pitch tại mục 2.1 báo cáo nhóm.
- Gom candidate thành 4 cluster và xây cây OST cho bài toán giám định xe; tách các nhu cầu, pain khỏi đề xuất công cụ và kiến trúc.
- Tổng hợp bảng so sánh 3 candidate theo 7 tiêu chí, ghi nhận lựa chọn card #1 của Quyên và lý do giữ các candidate còn lại cho vòng sau.
- Hỗ trợ rà soát assumption map và đối chiếu interview snapshot với problem nhóm chọn; góp ý tách thời gian thao tác khỏi thời gian chờ, phân biệt bằng chứng về pain với kỳ vọng về giải pháp, làm rõ tín hiệu xác nhận và phản bác ở CP4.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [Báo cáo cá nhân](report/individual/2A202603905_HoNguyenMinhSang.md).
- [Báo cáo nhóm — mục 2. Hội tụ nhóm (CP3)](report/team/group_report.md#2-hội-tụ-nhóm-cp3), gồm bảng candidate, cluster, cây OST và bảng shortlist.
- [Báo cáo nhóm — mục 3. Kiểm chứng và research (CP4)](report/team/group_report.md#3-kiểm-chứng--research-giải-pháp-đã-có-cp4), phần assumption map và tổng hợp interview snapshot.

**Điều mình học được từ phần nhóm:**

- Tôi học được cách bắt đầu từ tình huống, nhu cầu và quy trình hiện tại trước khi nghĩ đến công cụ. Với bài toán nhóm chọn, cần làm rõ nhân viên giám định vướng ở bước xác định hư hỏng, tra phụ tùng hay tra giá, rồi mới so sánh các cách hỗ trợ.
- Khi xem lại cây OST, tôi phân biệt rõ hơn giữa pain và solution: “phải tra giá từ nhiều nguồn” là khó khăn cần giải quyết, còn “nhận diện bằng Computer Vision” hay “Agent tự xử lý hồ sơ” là cách giải, không đặt ở tầng opportunity.
- Tôi nhận ra bottleneck phải khớp với cách công việc thực sự diễn ra. Ở card ghi chú họp, điểm chưa rõ được hỏi ngay trong cuộc họp; phần cần phân tích là công sức tổng hợp ghi chú, không mặc định thành viên phải hỏi lại sau họp. Tương tự, bài toán sửa chữa phải tách thời gian thao tác khỏi thời gian chờ phê duyệt để đo đúng vấn đề.

### MaiDanhHieu-2A202603948

**Phần việc phụ trách:**

- trực tiếp thực hiện ba cuộc phỏng vấn với giám định viên, nhân viên bồi thường và nhân viên garage; tổng hợp assumption map và research giải pháp theo Problem Card #1 của Nguyễn Thảo Quyên. AI hỗ trợ tổng hợp tài liệu và research.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- hoàn thiện mục 3 báo cáo nhóm; đổi bộ câu hỏi từ đề tài deadline sang giám định xe; phân biệt số liệu ước tính với baseline, nguồn sản phẩm với kiểm chứng người dùng; sửa kết luận chưa đủ nguồn về độ phủ Việt Nam. Đã thực hiện ba cuộc phỏng vấn và cung cấp tài liệu gốc để tổng hợp; chưa có bộ hồ sơ và log thời gian kèm theo.
- sử dụng ba cuộc phỏng vấn do Mai Danh Hiếu trực tiếp thực hiện, kết hợp nghiên cứu thứ cấp và research ba nhà cung cấp. Thời gian phỏng vấn: 16h00 ngày 09/11/2026; hình thức: trực tiếp.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- [CP4 báo cáo nhóm](report/team/group_report.md), [báo cáo cá nhân](report/individual/2A202603948_MAIDANHHIEU.md).

**Điều mình học được từ phần nhóm:**

- có sản phẩm AI tương tự không chứng minh đơn vị mục tiêu cần Agent; cần kiểm tra bottleneck, nguồn giá, quyền dữ liệu và phương án No AI/Rule trước.
