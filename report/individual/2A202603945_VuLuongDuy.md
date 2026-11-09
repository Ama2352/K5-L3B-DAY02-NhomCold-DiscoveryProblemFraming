# Báo cáo cá nhân — 2A202603945_VuLuongDuy

> ⚠️ **Trước khi nộp:** mọi chỗ `[ĐO THẬT]` / `___` là số ước tính hoặc ô trống — thay bằng số bạn tự quan sát, hỏi hoặc đếm được (ảnh chụp inbox đã che tên, lịch sử đơn). Mục 4–6 phải tự viết bằng trải nghiệm thật (RULES §2, RUBRIC C4). Xóa khối ghi chú này khi xong.

## 1. Thông tin học viên

- Họ tên: Vũ Lương Duy
- MSSV: 2A202603945
- Email trường (không bắt buộc):
- Tên nhóm: NhomCold
- Link repo nhóm: https://github.com/Ama2352/K5-L3B-DAY02-NhomCold-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Chủ đề scan: **Kinh doanh / bán hàng online** (shop nhỏ bán qua Facebook, Zalo, Shopee, TikTok Shop).

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi khách inbox đồng ý mua, chủ shop muốn có ngay thông tin đơn (tên, SĐT, địa chỉ, sản phẩm, size) trong file quản lý, để tạo vận đơn mà không phải đọc lại cả cuộc chat | Chủ shop, khách | ~1 phút chép tay/đơn × 200 đơn/ngày |
| 2 | Lặp lại | Khi nhiều khách hỏi cùng câu "giá bao nhiêu, còn size M không, ship bao lâu", chủ shop muốn trả lời nhanh mà vẫn đúng, để khách không bỏ đi | Chủ shop, khách | 40% tin nhắn là câu hỏi lặp lại  |
| 3 | Pain từ người khác | Khi tôi nhắn hỏi mua hàng qua Facebook, tôi muốn được trả lời trong vài phút, để quyết định mua luôn thay vì sang shop khác | Người mua (chính tôi) | Lần gần nhất tôi chờ 3 giờ mới được trả lời và đã mua chỗ khác |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi bán cùng lúc trên Facebook, Zalo và Shopee, chủ shop muốn biết tổng số đơn và tồn kho thật, để không bán quá số hàng đang có | Chủ shop | 20 lần/tháng phải xin lỗi khách vì hết hàng sau khi đã chốt |
| 5 | Pain từ người khác | Khi giao hàng thất bại vì sai SĐT/địa chỉ, chủ shop muốn biết sớm trước khi gửi, để không mất phí ship 2 chiều | Chủ shop, đơn vị vận chuyển | 8 đơn hoàn/tháng do sai thông tin ; mỗi đơn hoàn mất phí ship chiều về |
| 6 | Lặp lại | Khi có sản phẩm mới, chủ shop muốn đăng lên nhiều kênh với mô tả phù hợp từng nơi, để không mất cả buổi tối đăng bài | Chủ shop | ~18 phút/sản phẩm × 5 kênh |
| 7 | Tốn thời gian | Khi cuối ngày đối soát, chủ shop muốn khớp tiền COD về với danh sách đơn, để biết đơn nào chưa thu tiền | Chủ shop | ~30 phút/ngày |
| 8 | Pain từ người khác | Khi nhận đánh giá 1–2 sao trên sàn, chủ shop muốn phản hồi sớm, để không ảnh hưởng điểm shop | Chủ shop, khách | 10 đánh giá xấu/tháng |

**Nếu có dùng AI để gợi ý thêm:** sau khi tự scan 6 ý, tôi hỏi AI thêm góc nhìn. Giữ lại ý #7 và #8. Bỏ ý "chatbot AI bán hàng 24/7" vì là solution trá hình, không mô tả pain cụ thể.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Chốt đơn từ inbox: chép thông tin đơn thủ công (#1, gộp #2 và #5) | Lặp lại mỗi ngày, đo được (phút/đơn, số đơn sai thông tin), có đủ 4 mức can thiệp để so sánh | Bottleneck nằm ở trả lời câu hỏi lặp lại hay ở chép đơn? |
| 2 | Tồn kho lệch giữa nhiều kênh (#4) | Gây hậu quả thật (hủy đơn, mất uy tín) | Có thể chỉ cần phần mềm quản lý kho |
| 3 | Đăng sản phẩm lên nhiều kênh (#6) | Tốn thời gian rõ | Tần suất thấp hơn (chỉ khi có hàng mới) |

### Problem Card #1 — Chốt đơn từ inbox

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách inbox đồng ý mua, chủ shop muốn có ngay thông tin đơn đầy đủ và đúng trong file quản lý, để tạo vận đơn mà không phải đọc lại cả cuộc chat |
| Actor | Chủ shop nhỏ (1–3 người), bán thời trang/mỹ phẩm qua Facebook Page và Zalo, ~200 đơn/ngày |
| Thời điểm / bối cảnh | Buổi tối (giờ khách nhắn nhiều nhất) và sau mỗi buổi livestream |
| Quy trình hiện tại (3–7 bước) | 1. Mở inbox, lọc tin chưa đọc · 2. Trả lời câu hỏi giá/size/ship · 3. Kiểm tồn kho trong Sheet · 4. Xin tên, SĐT, địa chỉ · 5. Chép thông tin đơn sang Sheet/phần mềm vận chuyển · 6. Tạo vận đơn, gửi mã cho khách |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5: đọc lại đoạn chat, chép từng trường sang Sheet, ~1 phút/đơn, dễ chép sai SĐT/địa chỉ |
| Impact (nếu không giải thì sao) | ~200 phút/ngày; 8 đơn hoàn/tháng do sai thông tin (mất phí ship 2 chiều) |
| Success metric (baseline → target) | Thời gian từ "khách đồng ý mua" đến "đơn có trong Sheet": ~1 phút → ≤ 20 giây/đơn; đơn hoàn do sai thông tin: 8 → 0 |
| Phương án không dùng AI | Mẫu tin "xác nhận đơn" khách tự điền theo khuôn (Tên / SĐT / Địa chỉ / Sản phẩm / Size), hoặc gửi link Google Form |
| Giả thuyết về AI (nếu có) | AI đọc đoạn chat tự do, trích các trường đơn hàng thành 1 dòng; chủ shop duyệt rồi mới lưu |
| Cảm nhận nhanh | Rule hoặc Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 1 đơn, ~6 phút

[1 Mở inbox: 0.5'] → [2 Trả lời giá/size/ship: 2'] → [3 Kiểm kho: 0.5']
→ [4 Xin thông tin giao hàng: 1.5'] → [5 Chép đơn sang Sheet: 1'] ← BOTTLENECK (dễ sai)
→ [6 Tạo vận đơn + gửi mã: 0.5']
```

### Problem Card #2 — Tồn kho lệch giữa nhiều kênh

| Trường | Nội dung |
|---|---|
| Job Story | Khi bán cùng lúc trên Facebook, Zalo và Shopee, chủ shop muốn biết tồn kho thật, để không chốt đơn món đã hết |
| Actor | Chủ shop bán trên ≥ 2 kênh |
| Thời điểm / bối cảnh | Khi có món bán chạy hoặc sau livestream |
| Quy trình hiện tại (3–7 bước) | 1. Chốt đơn trên kênh A · 2. Nhớ trừ kho trong Sheet · 3. Cập nhật số lượng trên Shopee · 4. Khi khách kênh B hỏi, kiểm lại Sheet |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3: cập nhật tay sau mỗi đơn (~2 phút), hay quên khi đông khách |
| Impact (nếu không giải thì sao) | 20 lần/tháng hủy đơn vì hết hàng |
| Success metric (baseline → target) | Số đơn hủy vì hết hàng: 20 → 0/tháng |
| Phương án không dùng AI | Phần mềm quản lý bán hàng đa kênh đồng bộ kho |
| Giả thuyết về AI (nếu có) | Không cần — bài toán đúng/sai rõ |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
[1 Chốt đơn kênh A: 3'] → [2 Trừ kho trong Sheet: 1'] ← BOTTLENECK (hay quên)
→ [3 Cập nhật Shopee: 1'] → [4 Kiểm lại khi kênh B hỏi: 1']
```

### Problem Card #3 — Đăng sản phẩm lên nhiều kênh

| Trường | Nội dung |
|---|---|
| Job Story | Khi có sản phẩm mới, chủ shop muốn đăng lên nhiều kênh với mô tả phù hợp, để không mất cả buổi tối |
| Actor | Chủ shop |
| Thời điểm / bối cảnh | Mỗi lần nhập hàng mới (~1–2 lần/tuần) |
| Quy trình hiện tại (3–7 bước) | 1. Chụp ảnh · 2. Sửa ảnh · 3. Viết mô tả · 4. Đăng Facebook · 5. Đăng Shopee (điền thuộc tính) · 6. Đăng Zalo |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: viết mô tả, ~5 phút/sản phẩm |
| Impact (nếu không giải thì sao) | 270 phút/tuần |
| Success metric (baseline → target) | ~18 → 8 phút/sản phẩm |
| Phương án không dùng AI | Mẫu mô tả theo loại sản phẩm |
| Giả thuyết về AI (nếu có) | AI soạn nháp mô tả từ ảnh + thông số, chủ shop sửa |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[1 Chụp: 3'] → [2 Sửa ảnh: 3'] → [3 Viết mô tả: 5'] ← BOTTLENECK
→ [4 Đăng FB: 1'] → [5 Đăng Shopee: 5'] → [6 Đăng Zalo: 1']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: xảy ra với mọi đơn, mỗi ngày; sai sót có cái giá đo được bằng tiền (đơn hoàn); so sánh được đủ No AI / Rule / Workflow / Agent.
- Câu hỏi muốn nhóm phản biện: "Bottleneck thật là bước chép đơn, hay là bước trả lời câu hỏi lặp lại (bước 2 tốn nhiều phút hơn)?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Bước 2 (trả lời câu hỏi) tốn nhiều phút hơn bước 5, sao lại chọn bước 5 là bottleneck? | Đồng ý một phần | Ghi rõ: bước 5 không dài nhất nhưng là bước **gây lỗi tốn tiền** (đơn hoàn); bước 2 đưa vào giả định cần kiểm chứng |
| Chưa có người bán thật nào xác nhận số liệu | Đồng ý | Hỏi lại người bán để thay số ước tính bằng số thật (200 đơn/ngày, 8 đơn hoàn/tháng…) |
| Gợi ý chatbot tự chốt đơn và tự tạo vận đơn | Không đồng ý | Tạo vận đơn sai = mất tiền thật; giữ bước chủ shop duyệt trước khi lưu |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)


| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Lựa chọn pitch Problem Card #1 – Chốt đơn từ inbox trong lĩnh vực kinh doanh online. Tôi trình bày vấn đề chủ shop phải đọc lại hội thoại và nhập thủ công thông tin khách hàng vào Sheet. Đồng thời, tôi đặt câu hỏi: "Bottleneck thật sự nằm ở bước chép đơn hay bước trả lời các câu hỏi lặp lại?" | Card của tôi không được nhóm lựa chọn. Sau khi thảo luận, nhóm thống nhất tập trung vào bài toán giám định tổn thất xe ô tô vì đây là vấn đề có quy trình nghiệp vụ cụ thể, có thể phân tích bottleneck và đánh giá khả năng ứng dụng AI. |
| Phản biện bài của bạn khác | Tôi quan tâm đến tính xác thực của số liệu và khả năng giải quyết vấn đề thực tế. Đối với bài toán giám định tổn thất xe, những vấn đề cần làm rõ gồm: thời gian 20–40 phút/vụ là số liệu đo thực tế hay ước tính; ảnh ban đầu có thể nhận diện được những hư hỏng nào; AI có thể đánh giá được hư hỏng bên trong xe hay không. | Những câu hỏi này giúp làm rõ giới hạn của việc đánh giá hư hỏng thông qua hình ảnh. Đặc biệt, cần phân biệt hư hỏng bên ngoài có thể quan sát được với hư hỏng ẩn chỉ phát hiện khi tháo dỡ tại garage. |
| Nhận phản biện | Trong quá trình trình bày Problem Card #1, vấn đề được đặt ra là bước trả lời các câu hỏi về giá, size và vận chuyển có thời gian xử lý dài hơn bước nhập thông tin đơn hàng. Do đó, việc lựa chọn bước nhập liệu làm bottleneck cần có thêm căn cứ. | Tôi nhận ra rằng bottleneck không nhất thiết phải là bước tốn nhiều thời gian nhất. Bước nhập thông tin tuy chỉ mất khoảng 1 phút nhưng có nguy cơ sai SĐT, địa chỉ và gây ra chi phí hoàn hàng. Tôi giữ lại vấn đề này nhưng xác định cần kiểm chứng thêm vai trò của bước trả lời câu hỏi lặp lại. |
| Gom cluster  |  |  |
| Chọn candidate problem |  |  |
| Kiểm chứng / research |  |  |
| Quy trình nhóm | Phụ trách CP5, xây dựng sơ đồ quy trình hiện tại và tương lai. Quy trình hiện tại gồm 7 bước, xác định bottleneck nằm ở bước 3–5. Với quy trình tương lai, tôi phân chia rõ các công đoạn do Rule, AI và con người thực hiện. | Thời gian thao tác kỳ vọng 40–60' → ~17–20'/vụ; có điều kiện bắt buộc chuyển giám định trực tiếp và phương án quay về |
| Problem Statement | Viết Problem Statement v0 với 3 metric (thời gian bước 3–5, độ khớp danh sách hư hỏng, sai lệch chi phí); đưa AI phản biện và ghi 6 lỗ hổng | Lỗ hổng "chưa chắc có dữ liệu hồ sơ đã đóng để đo metric" trở thành giả định phải kiểm chứng |
| Mức can thiệp AI | | |
| Quyết định |  |  |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm problem sau khi tự scan | Gợi ý đối soát COD, đánh giá xấu | Đưa ý "chatbot bán hàng 24/7" — solution trá hình | Bỏ ý đó |
| CP2 Problem Card | Đóng vai "PM hoài nghi" phản biện card #1 | Chỉ ra bước 2 tốn nhiều phút hơn bước 5 | Đề xuất chatbot tự tạo vận đơn | Giữ bước chủ shop duyệt |
| CP4 Research |  |  |  |  |
| CP5 Quy trình | Chuyển mô tả quy trình giám định xe sang sơ đồ Mermaid, tách bước Rule / AI / con người | Dựng nhanh sơ đồ và bảng before/after; gợi ý checklist ảnh bắt buộc là bước Rule không cần AI | Màu sơ đồ (nền hồng nhạt) gần như không đọc được ở chế độ tối của GitHub; số phút từng bước chỉ là ước tính, không có nguồn | Yêu cầu đổi màu nền đậm + chữ trắng; đánh dấu các số chưa đo để thay bằng số phỏng vấn |
| CP5–6 Problem Statement |  |  |
| CP6 Mức can thiệp / quyết định |  |  |  |  |


---

## 6. Reflection (CP7)


**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Mỗi bạn có cách nhìn nhận pain point khác nhau tùy lĩnh vực và trải nghiệm.

Một vấn đề nghe có vẻ đơn giản nhưng có thể gây ảnh hưởng lớn nếu xảy ra thường xuyên.

Học cách đánh giá problem dựa trên Actor, tần suất, mức độ ảnh hưởng, bottleneck và khả năng đo lường.

**6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Liên hệ với việc ban đầu bạn từng nghĩ đến chatbot AI bán hàng 24/7.

Nhận ra chatbot là một giải pháp, chưa mô tả rõ vấn đề thực tế mà chủ shop gặp phải.

Cách nhóm phân biệt problem và solution thông qua Job Story, quy trình hiện tại và bottleneck.

Bài học: cần hiểu vấn đề trước khi lựa chọn công nghệ.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Lấy ví dụ về Problem Card #1.

Ban đầu chọn bước chép đơn là bottleneck vì dễ gây sai thông tin và hoàn hàng.

Sau phản biện, nhận ra bước trả lời câu hỏi lặp lại có thời gian xử lý dài hơn.

Điều chỉnh nhận định: phân biệt bước tốn nhiều thời gian nhất với bước gây hậu quả nghiêm trọng nhất.

Bài học về việc tiếp nhận phản biện và không bảo vệ ý tưởng chỉ vì đó là ý tưởng của mình.

**6.4. Kết quả kiểm chứng có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó xác định chính xác bottleneck và impact.

Phân biệt số liệu ước tính với số liệu đã được kiểm chứng.

Xây dựng Success Metrics có baseline, target và cách đo cụ thể.

Xác định Boundary: AI được làm gì, không được làm gì và khi nào cần HITL.

Liên hệ với 6 lỗ hổng mà AI đã chỉ ra trong Problem Statement v0.

Đặt câu hỏi về hiệu quả của phương án No AI trước khi đề xuất AI.
**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Không thay đổi hướng nghiên cứu nhiều lần nếu chưa đánh giá kỹ problem ban đầu.

Tiến hành kiểm chứng với người dùng sớm hơn thay vì dựa nhiều vào giả định.

Yêu cầu nguồn dữ liệu cụ thể cho từng con số trong Problem Statement.

Phản biện kỹ hơn về tính khả thi của việc thu thập dữ liệu ảnh, hồ sơ đã đóng và bảng giá phụ tùng.

Đặt câu hỏi về hiệu quả của phương án No AI trước khi đề xuất AI.
**6.7. Hiểu bài:** *(tự viết 5–8 câu, không nhìn tài liệu: problem → quy trình → metric → boundary → mức can thiệp → quyết định)*

---

## 7. Tài liệu tham khảo

- Pancake: https://pancake.vn/
- Meta Business Suite — About Automated Responses: https://www.facebook.com/business/help/395965998733706
- Shopee Seller Education Hub — Auto-Reply in Chat Assistant: https://seller.shopee.com.my/edu/article/3719/auto-reply-in-chat-assistant
