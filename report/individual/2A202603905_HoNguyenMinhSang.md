# Báo cáo cá nhân — 2A202603905_HoNguyenMinhSang

**Học viên:** Hồ Nguyễn Minh Sang · MSSV: 2A202603905 · Nhóm Cold.

**Repo nhóm:** https://github.com/Ama2352/K5-L3B-DAY02-NhomCold-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi tham gia cuộc họp nhóm có nhiều nội dung, tôi muốn ghi lại đầy đủ các quyết định và công việc đã thống nhất, để sau họp có ghi chú rõ ràng làm căn cứ thực hiện. | Các thành viên nhóm | Nội dung được phổ biến và điểm chưa rõ được hỏi ngay trong cuộc họp. Khó khăn cần xem xét là ghi chép và sắp xếp lại nội dung đã hiểu. Thời gian xử lý ghi chú tạm ước lượng 10–15 phút/buổi, chưa đo thực tế. |
| 2 | Tốn thời gian | Khi chuẩn bị trình bày tiến độ dự án trong buổi họp, tôi muốn xác định nhanh các file liên quan và phiên bản đang dùng, để trình bày đúng kết quả đã hoàn thành. | Dev phụ trách trình bày tiến độ | Nhiều file được sinh ra khiến thư mục lộn xộn, khó trình bày tiến độ khi họp. Thời gian tìm đúng file tạm ước lượng 10–15 phút trước mỗi buổi họp, chưa đo thực tế. Chưa bổ sung bằng chứng thực tế. |
| 3 | Lặp lại | Khi đến hạn cập nhật tiến độ hằng tuần, tôi muốn xác định những việc đã hoàn thành, đang làm và bị vướng, để báo cáo chính xác và biết việc nào cần hỗ trợ. | Thành viên phụ trách báo cáo, nhóm trưởng | Tạm ước lượng 20–30 phút/lần xem lại commit, task và tin nhắn, 1 lần/tuần. Tình huống, tần suất và thời gian chưa được xác nhận bằng trải nghiệm thực tế. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi yêu cầu dự án thay đổi qua nhiều cuộc trao đổi, tôi muốn xác định yêu cầu mới nhất và lý do thay đổi, để triển khai đúng phạm vi đã thống nhất. | Dev và người kiểm thử | Tạm ước lượng 15–20 phút đối chiếu 3–4 đoạn trao đổi mỗi lần thay đổi yêu cầu. Chưa xác nhận tình huống và số liệu thực tế. |
| 5 | Pain từ người khác | Khi nhận phần code được bàn giao để tích hợp, tôi muốn biết cách chạy, cấu hình cần thiết và lỗi còn tồn tại, để tiếp tục công việc mà không phải chờ người viết hướng dẫn lại. | Thành viên nhận bàn giao, người phụ trách tích hợp | Tạm ước lượng 30–60 phút thiết lập và hỏi lại 2–3 lần mỗi lượt bàn giao. Chưa xác nhận từ người nhận bàn giao thực tế. |

**AI gợi ý thêm:** sau hai vấn đề ban đầu (#1–#2), AI gợi ý #3–#5 và hỗ trợ diễn đạt. Các số liệu tham khảo trong CP1–CP2 do AI đề xuất, chưa đo hoặc xác nhận; chưa phải bằng chứng thực tế. Ý #3–#5 chưa được xác nhận bằng trải nghiệm cá nhân.

---

## 3. Top 3 Problem Cards (CP2)

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp ghi chú cuộc họp (#1) | Nhiều nội dung cần ghi lại; quy trình rõ; đo được thời gian tổng hợp và mức độ đầy đủ của ghi chú | Bước tốn công nhất là ghi chép hay sắp xếp lại? Có thường bỏ sót quyết định không? |
| 2 | Tìm đúng file báo cáo tiến độ (#2) | Tốn thời gian tìm và đối chiếu phiên bản; phạm vi gọn trong một dự án; đo được thời gian tìm đúng file | Vướng ở cách đặt tên, vị trí lưu hay thiếu quy ước phiên bản? |
| 3 | Xác định yêu cầu đã chốt (#4) | Phải đối chiếu nhiều nguồn; bước nghẽn cụ thể; có nguy cơ làm lại khi dùng yêu cầu cũ | Tần suất thay đổi và chi phí làm lại chưa được xác nhận; ai có quyền chốt yêu cầu? |

### Problem Card #1 — Tổng hợp ghi chú cuộc họp

| Trường | Nội dung |
|---|---|
| Job Story | Khi tham gia cuộc họp nhóm có nhiều nội dung, tôi muốn ghi lại đầy đủ các quyết định và công việc đã thống nhất, để sau họp có ghi chú rõ ràng làm căn cứ thực hiện. |
| Actor | Thành viên nhóm Cold tổng hợp ghi chú từ cuộc họp dự án |
| Thời điểm / bối cảnh | Nội dung và phân công được hiểu, làm rõ ngay trong cuộc họp; ghi chú được sắp xếp lại ngay sau khi kết thúc |
| Quy trình hiện tại | 1. Đọc lại ghi chú đã ghi trong họp · 2. Gom nội dung theo chủ đề · 3. Tách quyết định và công việc · 4. Đối chiếu người phụ trách, hạn đã thống nhất · 5. Lưu bản ghi chú hoàn chỉnh |
| Bottleneck | Bước 2, gom ghi chú rời rạc theo chủ đề: giả định 5 phút vì nội dung trao đổi có thể đan xen nhiều việc |
| Impact | Giả định 15 phút sắp xếp ghi chú sau mỗi cuộc họp; có nguy cơ bỏ sót quyết định trong bản lưu dù thành viên đã hiểu nội dung khi họp |
| Success metric | Thời gian hoàn thiện ghi chú từ baseline giả định 15 phút xuống ≤5 phút/buổi; không bỏ sót hoặc ghi sai quyết định và công việc đã thống nhất. Bấm giờ từ lúc đọc lại ghi chú đến khi lưu bản hoàn chỉnh trong 3 buổi họp, đối chiếu với ghi chép chung |
| Phương án không dùng AI | Ghi trực tiếp vào mẫu chung có chủ đề, quyết định, công việc, người phụ trách và hạn; kiểm tra nội dung và hỏi điểm chưa rõ ngay trong cuộc họp |
| Giả thuyết về AI | Chưa xác định; cần kiểm chứng bước nghẽn và đánh giá phương án không dùng AI trước |
| Cảm nhận nhanh | Chưa biết |

```text
HIỆN TẠI GIẢ ĐỊNH — 15 phút hoàn thiện ghi chú sau họp

[1 Đọc lại ghi chú: 3'] → [2 Gom nội dung theo chủ đề: 5'] ← BOTTLENECK
→ [3 Tách quyết định và công việc: 3']
→ [4 Đối chiếu phân công và hạn đã thống nhất: 2'] → [5 Lưu ghi chú: 2']
```

### Problem Card #2 — Tìm đúng file báo cáo tiến độ

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị báo cáo tiến độ dự án, tôi muốn tìm đúng file kết quả và phiên bản đang dùng, để trình bày đầy đủ những việc đã hoàn thành mà không đưa nhầm bản cũ. |
| Actor | Dev phụ trách chuẩn bị và trình bày kết quả dự án |
| Thời điểm / bối cảnh | Trước buổi họp tiến độ, khi thư mục dự án có nhiều file kết quả và bản nháp |
| Quy trình hiện tại | 1. Xác định nội dung cần báo cáo · 2. Tìm file trong thư mục dự án · 3. Mở và đối chiếu các phiên bản · 4. Xác nhận bản đang dùng · 5. Chuẩn bị liên kết trình bày |
| Bottleneck | Bước 3, mở nhiều file để đối chiếu phiên bản: giả định 5 phút vì tên và vị trí file chưa thể hiện rõ bản đang dùng |
| Impact | Tham khảo 10–15 phút tìm và xác nhận file mỗi lần chuẩn bị họp; có nguy cơ trình bày bản cũ hoặc bỏ sót kết quả đã hoàn thành |
| Success metric | Thời gian tìm và xác nhận file từ baseline giả định 15 phút xuống ≤5 phút/lần; không trình bày nhầm phiên bản. Bấm giờ 3 lần chuẩn bị họp và đối chiếu với bản được người phụ trách phần việc xác nhận |
| Phương án không dùng AI | Thống nhất cách đặt tên, tách thư mục bản nháp và bản báo cáo; duy trì mục lục liên kết đến file được xác nhận, ghi rõ người phụ trách cập nhật |
| Giả thuyết về AI | Chưa xác định; cần kiểm chứng bước nghẽn và đánh giá phương án không dùng AI trước |
| Cảm nhận nhanh | Chưa biết |

```text
HIỆN TẠI GIẢ ĐỊNH — 15 phút thao tác, chưa tính thời gian chờ xác nhận

[1 Xác định nội dung báo cáo: 2'] → [2 Tìm file: 4']
→ [3 Mở và đối chiếu phiên bản: 5'] ← BOTTLENECK
→ [4 Xác nhận bản đang dùng: 2'] → [5 Chuẩn bị liên kết: 2']
```

### Problem Card #3 — Xác định yêu cầu đã chốt

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận task có yêu cầu thay đổi qua nhiều cuộc trao đổi, tôi muốn biết nội dung nào đã được duyệt và vì sao thay đổi, để triển khai đúng phạm vi mà không làm theo bản cũ. |
| Actor | Dev nhận task thay đổi yêu cầu trong nhóm dự án |
| Thời điểm / bối cảnh | Trước khi triển khai task, khi thông tin trong tài liệu và các đoạn trao đổi chưa thống nhất |
| Quy trình hiện tại | 1. Tìm yêu cầu ban đầu · 2. Đọc các trao đổi thay đổi · 3. So sánh nội dung khác nhau · 4. Hỏi người có quyền duyệt · 5. Cập nhật task theo yêu cầu đã chốt |
| Bottleneck | Bước 3, đối chiếu nội dung giữa tài liệu và trao đổi: giả định 7 phút; chưa tính thời gian chờ người duyệt xác nhận |
| Impact | Tham khảo 15–20 phút xác định yêu cầu mỗi lần thay đổi; có nguy cơ triển khai sai phạm vi, làm lại hoặc kiểm thử theo tiêu chí cũ. Chưa xác nhận bằng tình huống thực tế |
| Success metric | Thời gian xác định yêu cầu từ baseline giả định 20 phút xuống ≤7 phút thao tác/lần; nội dung dùng triển khai được người duyệt xác nhận có hiệu lực. Đo 3 yêu cầu thay đổi từ lúc bắt đầu đối chiếu đến khi cập nhật task, ghi riêng thời gian chờ |
| Phương án không dùng AI | Một change log chung ghi ngày, nội dung trước/sau, lý do, người duyệt và task liên quan; chỉ dùng bản đã duyệt để triển khai |
| Giả thuyết về AI | Chưa xác định; cần kiểm chứng bước nghẽn và đánh giá phương án không dùng AI trước |
| Cảm nhận nhanh | Chưa biết |

```text
HIỆN TẠI GIẢ ĐỊNH — 20 phút thao tác, chưa tính thời gian chờ phản hồi

[1 Tìm yêu cầu ban đầu: 3'] → [2 Đọc trao đổi thay đổi: 5']
→ [3 So sánh nội dung khác nhau: 7'] ← BOTTLENECK
→ [4 Hỏi người có quyền duyệt: 3'] → [5 Cập nhật task: 2']
```

**AI phản biện card #1:**

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Bottleneck là hỏi lại người chủ trì sau họp | Không đồng ý | Xác định lại bottleneck là gom ghi chú rời rạc theo chủ đề; điểm chưa rõ được hỏi ngay trong cuộc họp |
| Chỉ đo thời gian có thể dẫn đến bản ghi chú nhanh nhưng thiếu quyết định hoặc công việc | Đồng ý | Bổ sung điều kiện không bỏ sót hoặc ghi sai quyết định và công việc đã thống nhất |
| Baseline 15 phút và bottleneck 5 phút chưa có dữ liệu đo thực tế | Đồng ý | Ghi rõ số liệu giả định; xác định cách đo từ lúc đọc lại ghi chú đến khi lưu bản hoàn chỉnh trong 3 buổi họp |
| Chưa kiểm chứng bước nghẽn và hiệu quả của mẫu ghi chú chung nên chưa đủ căn cứ chọn mức can thiệp | Đồng ý | Giữ cảm nhận ở mức Chưa biết; nêu phương án không dùng AI để so sánh sau khi đo quy trình hiện tại |

---

## 4. Tôi đã tham gia phần nào

| Hoạt động | Tôi đã làm gì? | Kết quả |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |

---

## 5. Dùng AI

| Checkpoint | Dùng AI để làm gì? | Hữu ích ở đâu? | Sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI góp ý hai vấn đề tự nêu, gợi ý thêm ba vấn đề, đề xuất số liệu tham khảo và trình bày bảng CP1. | Làm rõ tình huống, mục đích trong Job Story và mở rộng sang các lăng kính khác. | Các ý gợi ý và số liệu tham khảo chưa có bằng chứng thực tế; chưa thể dùng làm dữ liệu xác nhận. | Cần tự xác nhận ý 3–5, thay số tham khảo bằng số liệu thật và ghi rõ ý giữ/bỏ cùng lý do. |
| CP2 Problem Card | Soạn nháp 3 card, vẽ quy trình và phản biện bằng vai PM hoài nghi | Chỉ ra metric thiếu chất lượng, baseline chưa đo và cần thử phương án đơn giản hơn | Xác định sai bottleneck là hỏi lại người chủ trì sau họp | Chuyển bottleneck sang tổng hợp ghi chú; thêm metric về độ đầy đủ, giữ nhãn số liệu giả định và chưa chọn mức can thiệp |

---

## 6. Reflection
