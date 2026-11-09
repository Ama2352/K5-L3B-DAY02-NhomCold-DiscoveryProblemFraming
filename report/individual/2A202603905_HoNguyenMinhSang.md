# Báo cáo cá nhân — 2A202603905_HoNguyenMinhSang

## 1. Thông tin học viên

- Họ tên: Hồ Nguyễn Minh Sang
- MSSV: 2A202603905
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Cold
- Link repo nhóm: https://github.com/Ama2352/K5-L3B-DAY02-NhomCold-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi tham gia cuộc họp nhóm có nhiều nội dung, tôi muốn ghi lại đầy đủ các quyết định và công việc đã thống nhất, để sau họp có ghi chú rõ ràng làm căn cứ thực hiện. | Cả nhóm | Khoảng 10–15 phút/buổi sắp xếp ghi chú. |
| 2 | Tốn thời gian | Khi chuẩn bị trình bày tiến độ dự án trong buổi họp, tôi muốn xác định nhanh các file liên quan và phiên bản đang dùng, để trình bày đúng kết quả đã hoàn thành. | Dev, người báo cáo | Khoảng 10–15 phút/lần tìm đúng file giữa nhiều bản nháp. |
| 3 | Lặp lại | Khi đến kỳ thu tiền nhà trọ, tôi muốn tổng hợp tiền thuê, điện nước, phí phát sinh và công nợ từng phòng, để thu đúng tiền và theo dõi thu chi đầy đủ. | Chủ trọ, người thuê | Chốt sổ 1 lần/tháng; chưa đo thời gian và số khoản lệch. |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi nghiên cứu một chủ đề mới có nhiều khái niệm khó, tôi muốn được giải thích bằng ngôn ngữ đơn giản và ví dụ cụ thể, để hiểu bản chất và vận dụng vào việc đang làm. | Người học, dev | Phải tra thêm cách giải thích và ví dụ; chưa đo thời gian/khái niệm. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi cần tổng hợp thông tin từ nhiều file Excel, tôi muốn tập hợp và đối chiếu dữ liệu theo cùng các mục cần báo cáo, để có bảng tổng hợp đầy đủ, chính xác và tránh bỏ sót hoặc tính trùng thông tin. | Người lập báo cáo | Đọc và đối chiếu nhiều file; chưa đo số file/lần và thời gian tổng hợp. |
| 6 | Tốn thời gian | Khi ứng dụng báo lỗi với nhiều dòng log, tôi muốn xác định thông báo liên quan và bước tái hiện lỗi, để khoanh vùng nguyên nhân thay vì sửa thử nhiều chỗ. | Dev, tester | Thời gian đọc log và số lần sửa thử trước khi tái hiện được lỗi: chưa ghi nhận. |
| 7 | Lặp lại | Khi cùng một bài test lúc đạt lúc lỗi dù không đổi code, tôi muốn xác định điều kiện khiến kết quả thay đổi, để xử lý nguyên nhân và biết bản build có đáng tin để bàn giao hay không. | Dev, tester, người review | Số lần chạy lại test và thời gian kiểm tra kết quả không ổn định: chưa ghi nhận. |

**Nếu có dùng AI để gợi ý thêm:** sau khi tự scan 5 ý, tôi hỏi AI và giữ lại ý #6 và #7. Bỏ ý "cập nhật báo cáo định kỳ" vì trùng với vấn đề tổng hợp thông tin từ nhiều file Excel.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Tổng hợp ghi chú cuộc họp (#1) | Nhiều nội dung cần ghi lại; quy trình rõ; đo được thời gian tổng hợp và mức độ đầy đủ của ghi chú | Bước tốn công nhất là ghi chép hay sắp xếp lại? Có thường bỏ sót quyết định không? |
| 2 | Chốt sổ thu chi nhà trọ hằng tháng (#3) | Lặp lại theo kỳ, có đầu vào và đầu ra rõ; kiểm tra được số tiền từng phòng và tình trạng thanh toán | Các khoản phí được phân bổ ra sao? Bước tốn công là nhập chỉ số, tính tiền hay đối chiếu thanh toán? |
| 3 | Hiểu khái niệm khó khi research (#4) | Nhu cầu được nêu trực tiếp; có thể giới hạn ở một khái niệm và kiểm tra bằng việc tự giải thích, làm ví dụ | Cách giải thích nào phù hợp kiến thức nền? Nhanh hơn có giúp hiểu đúng và áp dụng được không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tham gia cuộc họp nhóm có nhiều nội dung, tôi muốn ghi lại đầy đủ các quyết định và công việc đã thống nhất, để sau họp có ghi chú rõ ràng làm căn cứ thực hiện. |
| Actor | Thành viên nhóm tổng hợp ghi chú cuộc họp |
| Thời điểm / bối cảnh | Ngay sau cuộc họp dự án, khi cần lưu quyết định và phân công |
| Quy trình hiện tại (3–7 bước) | 1. Đọc lại ghi chú đã ghi trong họp · 2. Gom nội dung theo chủ đề · 3. Tách quyết định và công việc · 4. Đối chiếu người phụ trách, hạn đã thống nhất · 5. Lưu bản ghi chú hoàn chỉnh |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, gom ghi chú theo chủ đề: khoảng 5 phút (ước lượng) |
| Impact (nếu không giải thì sao) | Khoảng 15 phút/buổi để sắp xếp ghi chú; có nguy cơ bỏ sót quyết định hoặc đầu việc |
| Success metric (baseline → target) | 15 → ≤5 phút/buổi; không bỏ sót hoặc ghi sai quyết định và đầu việc. Bấm giờ 3 buổi họp, đối chiếu ghi chép chung |
| Phương án không dùng AI | Mẫu ghi chú chung: chủ đề, quyết định, đầu việc, người phụ trách và hạn; làm rõ ngay trong họp |
| Giả thuyết về AI (nếu có) | AI gom ghi chú theo chủ đề, trích quyết định và đầu việc kèm nguồn; người tổng hợp kiểm tra trước khi lưu. Không tự bổ sung phân công |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI ƯỚC LƯỢNG — 15 phút/buổi

[1 Đọc lại ghi chú: 3'] → [2 Gom nội dung theo chủ đề: 5'] ← BOTTLENECK
→ [3 Tách quyết định và công việc: 3']
→ [4 Đối chiếu phân công và hạn đã thống nhất: 2'] → [5 Lưu ghi chú: 2']
```


### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi đến kỳ thu tiền nhà trọ, tôi muốn tổng hợp tiền thuê, điện nước, phí phát sinh và công nợ từng phòng, để thu đúng tiền và theo dõi thu chi đầy đủ. |
| Actor | Chủ nhà trọ hoặc người quản lý thu tiền |
| Thời điểm / bối cảnh | Cuối tháng, trước khi gửi bảng tiền cho từng phòng |
| Quy trình hiện tại (3–7 bước) | 1. Tập hợp chỉ số điện nước đầu/cuối kỳ · 2. Kiểm tra đơn giá, tiền thuê và cách phân bổ phí · 3. Tính các khoản phải thu theo phòng · 4. Đối chiếu thanh toán, công nợ và chi phí vận hành · 5. Lập thông báo tiền và tổng hợp sổ thu chi |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, đối chiếu thanh toán và công nợ theo phòng/kỳ: khoảng 10 phút (ước lượng) |
| Impact (nếu không giải thì sao) | Có nguy cơ thu thiếu, tính trùng hoặc bỏ sót nợ; khó giải thích khoản chênh lệch cho người thuê |
| Success metric (baseline → target) | 30 → ≤15 phút/kỳ với cùng số phòng; không tính trùng, mọi thanh toán gắn đúng phòng/kỳ. Bấm giờ khi đủ chỉ số và chứng từ, kiểm lại bằng phép tính độc lập |
| Phương án không dùng AI | Bảng tính có chỉ số, đơn giá, tiền thuê, phí theo thỏa thuận, số đã trả và công nợ; tách chi phí vận hành khỏi khoản thu người thuê |
| Giả thuyết về AI (nếu có) | AI trích phòng, kỳ và số tiền từ chứng từ để người quản lý kiểm tra; công thức tính tiền và công nợ. Không tự đặt đơn giá hoặc xác nhận đã nhận tiền |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI ƯỚC LƯỢNG — 30 phút/kỳ, cùng số phòng và chứng từ

[1 Tập hợp chỉ số: 5'] → [2 Kiểm đơn giá và phí: 3']
→ [3 Tính khoản phải thu: 7'] → [4 Đối chiếu thanh toán: 10'] ← BOTTLENECK giả thuyết
→ [5 Lập thông báo và sổ thu chi: 5']
```


### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi nghiên cứu một chủ đề mới có nhiều khái niệm khó, tôi muốn được giải thích bằng ngôn ngữ đơn giản và ví dụ cụ thể, để hiểu bản chất và vận dụng vào việc đang làm. |
| Actor | Người học hoặc dev nghiên cứu chủ đề mới |
| Thời điểm / bối cảnh | Khi tài liệu có thuật ngữ hoặc công thức vượt kiến thức nền |
| Quy trình hiện tại (3–7 bước) | 1. Xác định câu hỏi cần hiểu · 2. Đọc đoạn tài liệu liên quan · 3. Tra thuật ngữ và tìm cách diễn giải khác · 4. Tìm ví dụ rồi đối chiếu tài liệu gốc · 5. Tự giải thích và thử áp dụng |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, tra thuật ngữ và tìm cách giải thích dễ hiểu: khoảng 8 phút/khái niệm (ước lượng) |
| Impact (nếu không giải thì sao) | Khoảng 25 phút/khái niệm theo kịch bản; dễ nhớ định nghĩa nhưng hiểu sai cách dùng |
| Success metric (baseline → target) | 25 → ≤15 phút/khái niệm; tự giải thích đúng, nêu điều kiện áp dụng và làm được một ví dụ mới. Đo 3 lượt trước/sau với độ khó tương đương, đối chiếu tài liệu gốc |
| Phương án không dùng AI | Tài liệu nhập môn, bảng thuật ngữ, ví dụ có lời giải và trao đổi với người hướng dẫn |
| Giả thuyết về AI (nếu có) | AI giải thích đoạn tài liệu bằng lời đơn giản, ví dụ từng bước và điều kiện áp dụng theo kiến thức nền. Người học đối chiếu nguồn và tự làm ví dụ mới |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI ƯỚC LƯỢNG — 25 phút/khái niệm

[1 Xác định câu hỏi: 2'] → [2 Đọc đoạn tài liệu: 5']
→ [3 Tra thuật ngữ và cách diễn giải: 8'] ← BOTTLENECK giả thuyết
→ [4 Tìm ví dụ, đối chiếu nguồn: 5'] → [5 Tự giải thích và áp dụng: 5']
```


### Card muốn pitch nhất

- Card số: **#1 — Tổng hợp ghi chú cuộc họp**.
- Vì sao: Phạm vi gọn trong một cuộc họp, quy trình rõ; đo được thời gian tổng hợp và kiểm tra độ đầy đủ của quyết định, đầu việc.
- Câu hỏi muốn nhóm phản biện: Nếu ghi trực tiếp vào mẫu chung ngay trong cuộc họp, bước gom ghi chú còn mất nhiều thời gian không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline 15 phút và bước gom ghi chú 5 phút chỉ là ước lượng | Đồng ý | Ghi rõ số giả định; thêm cách bấm giờ trong 3 buổi họp |
| Chỉ đo tốc độ, thiếu kiểm tra chất lượng ghi chú | Đồng ý | Thêm điều kiện không bỏ sót hoặc ghi sai quyết định và đầu việc |
| Xác định bottleneck là hỏi lại người chủ trì sau họp | Không đồng ý | Giữ bước gom ghi chú là bottleneck giả thuyết; điểm chưa rõ được hỏi ngay trong họp |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tổng hợp 12 candidate của 4 thành viên vào mục 2.1 báo cáo nhóm | Có bảng đối chiếu candidate, actor và bottleneck làm cơ sở hội tụ |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt (tình huống minh họa): “Bước nghẽn chính là xác định hư hỏng, tra phụ tùng hay tra giá? Nếu có sẵn bảng giá chuẩn thì còn tốn thời gian ở đâu?” | Hướng xử lý trong tình huống: tách thời gian từng bước, so sánh với checklist và bảng giá chuẩn thay vì mặc định phải dùng Agent |
| Nhận phản biện | Câu hỏi tôi nhận được (tình huống minh họa): “Vì sao chọn bài toán sửa chữa ô tô thay vì sổ thu chi nhà trọ, trong khi bài toán nhà trọ dễ kiểm chứng hơn?” | Cách trả lời trong tình huống: làm rõ phạm vi chỉ là dự toán ban đầu có người giám định kiểm tra; nêu trở ngại về dữ liệu và giữ bài toán nhà trọ cho vòng sau. Phạm vi và lý do chọn/loại này đã được thể hiện ở mục 2.4 báo cáo nhóm |
| Gom cluster / cây OST | Phụ trách tổng hợp 12 candidate thành 4 cluster; trình bày cây OST cho bài toán dự toán sửa chữa ô tô, tách pain khỏi các ý Computer Vision, hệ thống tra cứu và Agent | Hoàn thiện mục 2.2–2.3 báo cáo nhóm; outcome tập trung vào thời gian lập dự toán, hạng mục bỏ sót và sai lệch chi phí |
| Chọn candidate problem | Tổng hợp bảng so sánh 3 candidate theo 7 tiêu chí và ghi lý do chọn/loại; ghi nhận lựa chọn của nhóm là card #1 của Nguyễn Thảo Quyên | Chốt “Xác định hư hỏng và ước lượng chi phí sửa chữa” tại mục 2.4; giới hạn phạm vi ở dự toán ban đầu để người giám định kiểm tra |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---


## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm và hỗ trợ diễn đạt Job Story | Làm rõ tình huống, nhu cầu và kết quả của ý tổng hợp nhiều file Excel do tôi tự bổ sung | Từng đề xuất số liệu khi chưa đo | Thay ý bàn giao code do AI gợi ý bằng vấn đề Excel; không dùng số liệu chưa có cho ý #5 |
| CP2 Problem Card | Soạn nháp 3 card, vẽ quy trình và phản biện bằng vai PM hoài nghi | Chỉ ra metric thiếu chất lượng, baseline chưa đo và cần thử phương án đơn giản hơn | Xác định sai bottleneck là hỏi lại người chủ trì sau họp | Giữ bước gom ghi chú; thêm điều kiện chất lượng và cách đo thời gian |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---


## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

- [Báo cáo nhóm và nguồn research](../team/group_report.md#10-tài-liệu-tham-khảo).
