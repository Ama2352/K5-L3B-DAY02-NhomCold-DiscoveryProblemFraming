# Báo cáo cá nhân — 2A202603895_NguyenThaoQuyen

## 1. Thông tin học viên

- Họ tên: Nguyễn Thảo Quyên
- MSSV:2A202603895
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: NhomCold
- Link repo nhóm: https://github.com/Ama2352/K5-L3B-DAY02-NhomCold-DiscoveryProblemFraming/tree/main

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 |Tốn thời gian |Khi khách hàng yêu cầu báo giá phụ tùng ô tô nhưng chỉ cung cấp hình ảnh hoặc tên gọi thông thường, nhân viên muốn xác định đúng phụ tùng theo dòng xe và mã sản phẩm, để tránh báo giá nhầm và mất thời gian tra cứu. | Nhân viên tư vấn phụ tùng, garage, khách hàng| Phát sinh theo từng yêu cầu báo giá; có thể phải tra cứu nhiều danh mục và đối chiếu thủ công; cần đo thời gian tìm kiếm và tỷ lệ xác định sai.|
| 2 |Pain từ người khác |Khi làm việc tại một nhà máy có nhiều SOP và quy trình vận hành, nhân viên mới muốn nhanh chóng tìm được đúng tài liệu và hiểu quy trình cần tuân thủ cho từng công việc, để tránh làm sai quy trình, mất thời gian tra cứu hoặc áp dụng nhầm hướng dẫn. |Nhân viên mới, công nhân vận hành, nhân viên QC, kỹ sư sản xuất, quản lý nhà máy |Nhân viên mới phải đọc và tra cứu nhiều SOP từ các nguồn khác nhau; có thể gặp khó khăn khi xác định tài liệu nào áp dụng cho công việc hoặc phiên bản nào còn hiệu lực |
| 3 |Pain từ người khác | Khi sinh viên liên tục gặp khó khăn với cùng một nội dung, giảng viên muốn xác định những phần kiến thức mà nhiều người chưa hiểu, để điều chỉnh cách giảng dạy.|Giảng viên, sinh viên | Số câu hỏi lặp lại, số sinh viên gặp khó khăn, kết quả kiểm tra.|
| 4 |Lặp lại | 	Khi giảng viên nhận nhiều bài tập, tôi muốn kiểm tra và phân loại bài theo cùng một tiêu chí, để giảm công việc đánh giá lặp lại.|Giảng viên, trợ giảng |Số bài mỗi lớp, thời gian chấm, số lớp phụ trách. |
| 5 | Tốn thời gian|	Khi khách hàng hỏi về tình trạng một bất động sản, môi giới muốn nhanh chóng kiểm tra thông tin còn trống, giá và lịch xem nhà, để phản hồi chính xác. | Môi giới, khách hàng| Số lượt hỏi mỗi ngày, thời gian xác nhận, số hệ thống quản lý.|
| 6 | Tốn thời gian | Khi xe xảy ra tai nạn, tôi muốn nhanh chóng xác định các phụ tùng bị hư hỏng và ước lượng chi phí sửa chữa, thay thế, để xác định mức bồi thường dự kiến và chuyển hồ sơ đến cấp phê duyệt phù hợp. | Giám định viên, nhân viên bồi thường, trưởng phòng, giám đốc | Thời gian kiểm tra hư hỏng, tra cứu giá phụ tùng, lập bảng báo giá và chờ phê duyệt hồ sơ 5 đến 7 ngày. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Các ý AI gợi ý mà tôi giữ lại là ý số 3,4. Vì các Job story đọc khá hợp lí, painpoint rõ ràng. Và có các ý tôi trải qua tương tự. 


---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Xác định hư hỏng và ước lượng chi phí sửa chữa (#6) | Quy trình nhiều bước, kết hợp nhận diện hình ảnh, tra cứu phụ tùng và ước lượng chi phí; có tiềm năng phát triển bài toán AI đa phương thức và hỗ trợ ra quyết định. | Độ chính xác nhận diện hư hỏng; độ tin cậy của dữ liệu giá và chi phí ước lượng. |
| 2 | Tra cứu và xác định phụ tùng ô tô (#1) | Pain cụ thể, phát sinh thường xuyên; có chiều sâu kỹ thuật ở tìm kiếm đa phương thức, hybrid search và xác định phụ tùng tương thích. | Khả năng tiếp cận dữ liệu; độ chính xác khi xác định phụ tùng theo dòng xe và mã sản phẩm. |
| 3 | Kiểm tra và phân loại bài tập (#4) | Công việc lặp lại, có thể chuẩn hóa rubric và đánh giá mức độ nhất quán giữa AI với người chấm. | Khó đánh giá chất lượng với bài tự luận, câu trả lời sáng tạo và các trường hợp cần nhận định chuyên môn. |

### Problem Card #1 — Xác định hư hỏng và ước lượng chi phí sửa chữa (#6)

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận yêu cầu bồi thường kèm hình ảnh xe bị tai nạn, tôi muốn xác định các bộ phận bị hư hỏng và ước lượng chi phí sửa chữa, để có cơ sở đánh giá mức bồi thường và tư vấn cho khách hàng. |
| Actor | Nhân viên giám định tổn thất, nhân viên xử lý bồi thường bảo hiểm ô tô. |
| Thời điểm / bối cảnh | Khi khách hàng gửi hình ảnh xe sau tai nạn và yêu cầu đánh giá mức độ hư hỏng, chi phí sửa chữa. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận hình ảnh và thông tin xe. 2. Kiểm tra hình ảnh tổng thể. 3. Xác định các vị trí và bộ phận bị hư hỏng. 4. Tra cứu phụ tùng cần thay thế hoặc sửa chữa. 5. Tìm kiếm giá phụ tùng và công sửa chữa. 6. Tổng hợp chi phí dự kiến. 7. Chuyển kết quả cho bộ phận có thẩm quyền xác nhận. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: xác định hư hỏng, tra cứu phụ tùng và giá sửa chữa. Ước tính 20–40 phút/vụ, tùy mức độ hư hỏng và độ phức tạp của xe. |
| Impact (nếu không giải thì sao) | Thời gian xử lý hồ sơ kéo dài; kết quả ước lượng có thể thiếu nhất quán giữa các nhân viên; ảnh hưởng đến thời gian phản hồi khách hàng và tiến độ giải quyết bồi thường. |
| Success metric (baseline → target) | Thời gian đánh giá ban đầu: 20–40 phút/vụ → giảm ít nhất 30–50%; độ chính xác xác định bộ phận hư hỏng và sai số ước lượng chi phí được đánh giá trên tập hồ sơ đã có kết quả giám định thực tế. |
| Phương án không dùng AI | Xây dựng danh mục hư hỏng, bảng giá phụ tùng chuẩn hóa, checklist đánh giá theo dòng xe và biểu mẫu tính chi phí. |
| Giả thuyết về AI (nếu có) | Kết hợp Computer Vision để nhận diện vị trí và mức độ hư hỏng, hệ thống tra cứu phụ tùng và dữ liệu giá để đề xuất danh sách sửa chữa cùng chi phí dự kiến. |
| Cảm nhận nhanh | Agent |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — Ước tính 20–40 phút/vụ

[1 Tiếp nhận hình ảnh + thông tin xe]
              ↓
[2 Kiểm tra hình ảnh tổng thể]
              ↓
[3 Xác định bộ phận hư hỏng] ← BOTTLENECK
              ↓
[4 Tra cứu phụ tùng cần sửa/thay]
              ↓
[5 Tìm kiếm giá phụ tùng + công sửa chữa]
              ↓
[6 Tổng hợp chi phí dự kiến]
              ↓
[7 Chuyển kết quả xác nhận]
```

### Problem Card #2 - Tra cứu và xác định phụ tùng ô tô (#1)
 
| Trường | Nội dung |
|---|---|
| Job Story | Khi cần tìm phụ tùng thay thế cho một dòng xe cụ thể, tôi muốn xác định đúng tên, mã và loại phụ tùng tương thích, để tránh chọn nhầm sản phẩm và đảm bảo quá trình sửa chữa diễn ra chính xác. |
| Actor | Nhân viên kỹ thuật, nhân viên phụ tùng, nhân viên giám định và xử lý bồi thường bảo hiểm. |
| Thời điểm / bối cảnh | Khi tiếp nhận yêu cầu tra cứu phụ tùng từ thông tin xe, hình ảnh bộ phận hoặc mô tả hư hỏng. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận thông tin xe (hãng, dòng xe, năm sản xuất). 2. Tiếp nhận tên hoặc hình ảnh phụ tùng cần tìm. 3. Tìm kiếm trong danh mục phụ tùng hoặc file dữ liệu. 4. Đối chiếu tên gọi, mã sản phẩm và thông số kỹ thuật. 5. Kiểm tra khả năng tương thích với dòng xe. 6. Xác nhận phụ tùng phù hợp và tra cứu giá. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–5: tìm kiếm và đối chiếu phụ tùng tương thích. Ước tính 10–20 phút/lần tra cứu, có thể lâu hơn khi tên gọi không thống nhất hoặc thiếu mã sản phẩm. |
| Impact (nếu không giải thì sao) | Chọn sai phụ tùng, phát sinh chi phí đổi trả hoặc sửa chữa; kéo dài thời gian xử lý hồ sơ và phụ thuộc nhiều vào kinh nghiệm của nhân viên. |
| Success metric (baseline → target) | Thời gian tra cứu: 10–20 phút/lần → giảm ít nhất 50%; tỷ lệ xác định đúng phụ tùng và tỷ lệ tương thích được kiểm chứng trên tập dữ liệu có nhãn chuẩn. |
| Phương án không dùng AI | Chuẩn hóa danh mục phụ tùng, xây dựng từ điển tên gọi đồng nghĩa, mã hóa theo hãng và dòng xe, bổ sung bộ lọc theo thông số kỹ thuật. |
| Giả thuyết về AI (nếu có) | Kết hợp tìm kiếm từ khóa, tìm kiếm ngữ nghĩa và bộ lọc metadata để truy xuất phụ tùng từ tên gọi, mô tả hoặc hình ảnh; sau đó đối chiếu thông tin xe để xếp hạng các sản phẩm tương thích. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — Ước tính 10–20 phút/lần

[1 Tiếp nhận thông tin xe]
              ↓
[2 Nhận tên / mã / hình ảnh phụ tùng]
              ↓
[3 Tìm kiếm trong danh mục dữ liệu] ← BOTTLENECK
              ↓
[4 Đối chiếu tên gọi và mã sản phẩm]
              ↓
[5 Kiểm tra tương thích theo dòng xe]
              ↓
[6 Xác nhận phụ tùng + tra cứu giá]
```


### Problem Card #3 — Kiểm tra và phân loại bài tập (#4)

| Trường | Nội dung |
|---|---|
| Job Story | Khi học viên nộp bài tập, tôi muốn kiểm tra kết quả, phân loại lỗi và đánh giá mức độ hoàn thành theo tiêu chí có sẵn, để phản hồi kịp thời và theo dõi tiến độ học tập của từng học viên. |
| Actor | Giáo viên, trợ giảng, người phụ trách quản lý chất lượng học tập. |
| Thời điểm / bối cảnh | Sau mỗi buổi học, bài kiểm tra hoặc khi học viên hoàn thành và nộp bài tập. |
| Quy trình hiện tại (3–7 bước) | 1. Tiếp nhận bài tập của học viên. 2. Đọc và kiểm tra câu trả lời. 3. Đối chiếu với đáp án hoặc rubric. 4. Xác định câu trả lời đúng, sai hoặc chưa đầy đủ. 5. Chấm điểm và phân loại lỗi. 6. Viết nhận xét và đề xuất nội dung cần cải thiện. 7. Tổng hợp kết quả học tập. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–5: đọc, đối chiếu và phân loại lỗi. Ước tính 5–10 phút/bài đối với bài tập có cấu trúc; bài tự luận có thể mất nhiều thời gian hơn. |
| Impact (nếu không giải thì sao) | Giáo viên và trợ giảng mất nhiều thời gian cho công việc lặp lại; thời gian phản hồi học viên chậm; tiêu chí đánh giá có thể thiếu nhất quán giữa những người chấm. |
| Success metric (baseline → target) | Thời gian kiểm tra: 5–10 phút/bài → giảm ít nhất 40%; mức độ nhất quán giữa kết quả đánh giá và người chấm đạt ít nhất 90% trên tập bài đã được chấm chuẩn. |
| Phương án không dùng AI | Xây dựng ngân hàng đáp án, rubric chấm điểm, bộ quy tắc kiểm tra tự động cho câu hỏi trắc nghiệm và câu trả lời có cấu trúc. |
| Giả thuyết về AI (nếu có) | Sử dụng mô hình ngôn ngữ để đối chiếu câu trả lời với rubric, phân loại lỗi, đề xuất điểm số và tạo nhận xét. Giáo viên kiểm tra lại các trường hợp không chắc chắn trước khi công bố kết quả. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — Ước tính 5–10 phút/bài

[1 Tiếp nhận bài tập]
              ↓
[2 Đọc và kiểm tra câu trả lời] ← BOTTLENECK
              ↓
[3 Đối chiếu đáp án / rubric]
              ↓
[4 Xác định câu đúng, sai, thiếu]
              ↓
[5 Chấm điểm + phân loại lỗi]
              ↓
[6 Viết nhận xét và phản hồi]
              ↓
[7 Tổng hợp kết quả học tập]

```

### Card muốn pitch nhất

- Card số: Card số 1 
- Vì sao: Bài toán thực tế, đánh vào nổi đau của thân chủ của xe, và giám định viên. Khi làm được flow này có thể sẽ giảm thời gian của 1 bộ hồ sơ pending từ 5-7 ngày xuống chỉ còn vài giờ.
- Câu hỏi muốn nhóm phản biện: Bước nghẽn chính là xác định hư hỏng, tra phụ tùng hay tra giá? Ảnh có đủ căn cứ để lập dự toán không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card |Trình bày vấn đề xác định các phụ tùng bị hư hỏng và ước lượng chi phí sửa chữa sau tai nạn xe. |Đưa ra một vấn đề cụ thể trong quy trình xử lý hồ sơ bồi thường để nhóm xem xét. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt:  (card tổng hợp ghi chú họp): "Nếu ghi trực tiếp theo mẫu ngay trong họp, bước gom ghi chú còn tốn thời gian không?" | Góp phần kiểm tra tính rõ ràng và mức độ có thể kiểm chứng của vấn đề. Sang sửa bottleneck từ "hỏi lại sau họp" thành "công sức tổng hợp ghi chú". |
| Nhận phản biện | Câu hỏi tôi nhận được: "Nếu làm vậy thì làm sao đảm bảo AI nhận diện đúng 100%?" | Tôi đã sửa gì: Không đặt mục tiêu AI đúng 100%; thêm bước giám định viên xác nhận từng bộ phận AI đề xuất, đo riêng tỉ lệ bỏ sót (≤ 15%), và chuyển giám định trực tiếp khi AI có độ tin cậy dưới 60%. |
| Gom cluster / cây OST |Sang phụ trách gom cluster và cây OST. Tôi cung cấp 3 card (#4 hư hỏng xe, #5 phụ tùng, #6 chấm bài) để gom nhóm. | Cả 3 card của tôi vào cluster C "Đánh giá và đối chiếu chuyên môn". 4 opportunity của cây OST (xác định hư hỏng, đối chiếu phụ tùng, tra giá nhiều nguồn, đối chiếu căn cứ dự toán) đều lấy từ quy trình trong card #1 của tôi. "Computer Vision" và "Agent tự xử lý hồ sơ" trong card bị gạch khỏi tầng opportunity vì là solution.|
| Chọn candidate problem |Đề xuất card #1 "Xác định hư hỏng và ước lượng chi phí sửa chữa" vào shortlist. |Nhóm chọn card #1 với 28 điểm, cao nhất shortlist (mục 2.4). Loại "tra cứu phụ tùng" (27 điểm) vì hẹp hơn và đã là một bước của card #1. Loại "sổ nhà trọ" (26 điểm) vì chỉ cần bảng tính hoặc Rule, ít cơ sở so sánh 4 mức. |
| Kiểm chứng / research |Hiếu phụ trách CP4. Tôi cung cấp card #1 làm nguồn cho các giả định. |CP4 lập 6 giả định A1–A6 từ card #1 và research 3 công cụ (Tractable, Solera Qapter, CCC). Phát hiện: đã có sản phẩm làm sẵn nên không cần tự xây mô hình; chưa phỏng vấn được ai (0 người, 0 hồ sơ). |
| Quy trình nhóm |Duy phụ trách quy trình trước/sau. Tôi đối chiếu quy trình đó khi viết CP6. ||
| Problem Statement |Tôi viết Problem Statement v1 (mục 7) dựa trên v0 của Duy và 6 lỗ hổng AI chỉ ra. Bài toán: giám định viên tổn thất xe ô tô mất 10–15 phút/vụ để tự nhìn ảnh xác định bộ phận hư hỏng và chọn thay/sửa, kết quả khác nhau giữa các giám định viên với cùng bộ ảnh. AI chỉ đề xuất bộ phận ở bước 3, giám định viên xác nhận từng bộ phận. Việc tra mã và giá do Rule cùng bảng giá chuẩn xử lý. | v1 khác v0 ở 4 trường, có ghi lý do: mức chọn từ Agent thành Workflow; bottleneck thu hẹp từ bước 3–5 còn bước 3; metric tách bỏ sót / báo thừa và đo theo mức độ vụ; boundary thêm "chỉ hư hỏng nhìn thấy, chi phí sửa chữa ≠ tiền bồi thường, không gửi ảnh ra ngoài khi chưa được phép".|
| Mức can thiệp AI | Viết mục 6: ma trận độ mơ hồ × độ phức tạp, so sánh 4 mức, AI Canvas, 2 câu Google PAIR. Bước 3 (nhìn ảnh xác định hư hỏng) mơ hồ cao; các bước tra mã, tra giá, cộng tổng có đúng/sai rõ. | Chọn **Workflow**, AI chỉ ở bước 3, giám định viên xác nhận từng bộ phận (augment; bỏ sót tệ hơn báo nhầm). Không chọn Rule vì Rule không đọc được ảnh; không chọn Agent vì các bước đã cố định. Ưu tiên công cụ có sẵn, không tự xây. |
| Quyết định | Viết mục 8: chấm 4 rủi ro (Value Cao, Usability TB, Feasibility Cao, Viability Cao) và ngưỡng dừng. | Đề xuất **Not Yet**: chưa phỏng vấn ai, chưa có quyền dùng dữ liệu. Trước tiên thử checklist + bảng giá trên 5 hồ sơ, không dùng AI. Dừng AI nếu tỉ lệ bỏ sót > 15% trên 30 hồ sơ cũ. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Sau khi tự scan, nhờ AI gợi ý thêm problem. | Gợi ý ý #3, #4 (giảng viên) có pain rõ, tôi từng gặp tương tự. | Ý AI gợi ý chưa có số đo thật, chỉ ghi chung chung. | Chỉ giữ #3, #4 vì có trải nghiệm thật; bỏ các ý tôi không gặp. |
| CP2 Problem Card | Phản biện, đàm phán, và brainstorm | đóng vai rất tốt | bắt bẻ tiểu tiết đến mức nó không phải là lỗi cũng cho là lỗi. | Sửa lại flow theo đúng ý của mình. |
| CP4 Research | Không phụ trách (Hiếu làm). | | | |
| CP5 Quy trình | Không phụ trách (Duy làm). | | | |
| CP5–6 Problem Statement | Nhờ AI soạn nháp Problem Statement v1 và bảng v0 → v1. | Đối chiếu nhanh v1 với 6 lỗ hổng; phát hiện CP5 lệch số (20 vs 15 hồ sơ/ngày). | Thêm dòng thay đổi "Boundary" dù v0 đã có ý đó; gắn quá nhiều nhãn đối chiếu. | Bỏ dòng trùng, chỉ giữ thay đổi thật; cắt số hồ sơ/ngày khỏi Actor. |
| CP6 Mức can thiệp / quyết định | Nhờ AI soạn nháp mục 6–8 theo template. | Lập luận vì sao không chọn Agent; chỉ ra bước 3 chỉ chiếm ~17–37% thời gian nên cần đo thật. | Tự đặt 3 ngưỡng 30/50/20% không có căn cứ; có lúc báo sai về nhánh khác. | Bác 3 ngưỡng, tự chốt bỏ sót ≤ 15%, báo thừa ≤ 2 bộ phận; tự quyết Not Yet. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
- Ba đề tài có thể giúp bạn nhận ra ba cách tiếp cận khác nhau khi xác định vấn đề:
    - Tổng hợp ghi chú cuộc họp: Không chỉ là ghi chép mà còn phải phân biệt thông tin, quyết định và sắp xếp nội dung.
    - Chốt đơn từ inbox: Cần xác định chính xác bottleneck là trả lời câu hỏi lặp lại hay nhập lại thông tin đơn hàng.
    - Tổng hợp tiến độ: Phải phân biệt thông tin chưa được cung cấp với thông tin đã có nhưng khó tổng hợp.

Một problem tốt không chỉ cần có pain point mà còn phải xác định được nguyên nhân, phạm vi và metric để kiểm chứng.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
- Có. Ban đầu, nhóm tôi khá solution-first khi nghĩ ngay đến việc sử dụng Computer Vision để nhận diện hư hỏng xe sau tai nạn. Tuy nhiên, sau khi phân tích quy trình nghiệp vụ, nhóm nhận ra nhận diện hình ảnh chỉ là một bước, khó khăn còn nằm ở việc xác định phụ tùng, tra cứu giá và tổng hợp chi phí sửa chữa. Vì vậy, nhóm đã quay lại xác định bottleneck thực tế và mở rộng phạm vi bài toán thành hỗ trợ đánh giá hư hỏng và ước lượng chi phí, thay vì chỉ tập trung vào mô hình nhận diện hình ảnh.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
- Trong bài lab lần này, tôi chưa đổi ý sau khi bị phản biện. Vì paintpoint tôi đưa ra là dựa vào trải nghiệm thực tế, hoàn toàn hợp lý về mặt thực tế, có thành viên bảo là nếu làm vậy thì làm sao đảm bảo được AI có thể detect đúng được 100% - vấn đề phản biện này thì khi đã làm AI thì tỷ lệ khi đúng 100% là khá khó để đạt được. Do vậy tôi không đổi ý sau khi bị phản biện.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
- Research cho thấy Tractable, Solera và CCC đã làm sẵn phần đánh giá hư hỏng từ ảnh.
- Nhóm chưa thực hiện phỏng vấn thực tế (0 người, 0 hồ sơ)

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
- Phân biệt khó khăn trong nhận diện hư hỏng với khó khăn trong tra cứu giá
- Phải tách hai kiểu lỗi: bỏ sót và báo thừa

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
- Phản biện mạnh hơn về tính khả thi của dữ liệu đầu vào và độ tin cậy của kết quả AI.
- Tìm hiểu quy trình thực tế thay vì chỉ dựa vào suy luận.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

- Nhóm chọn bài toán hỗ trợ giám định viên xác định bộ phận hư hỏng từ ảnh xe tai nạn, vì đánh giá thủ công mất thời gian và thiếu nhất quán.
AI chỉ tham gia đề xuất các bộ phận hư hỏng, còn tra cứu thông tin xe và giá sử dụng Rule.
Nhóm đánh giá hiệu quả qua thời gian xử lý, tỷ lệ bỏ sót và số bộ phận báo thừa.
AI không được tự quyết định tiền bồi thường; giám định viên phải xác nhận mọi kết quả.
Nhóm chọn Workflow vì quy trình đã có các bước cố định, không cần Agent tự quyết định hành động.
Do chưa có phỏng vấn và dữ liệu thực tế, nhóm quyết định Not Yet.
Bước tiếp theo là thử checklist và bảng giá trên 5 hồ sơ trước khi quyết định có cần AI hay không.
---

## 7. Tài liệu tham khảo


