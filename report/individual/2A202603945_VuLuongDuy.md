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
| 2 | Lặp lại | Khi nhiều khách hỏi cùng câu "giá bao nhiêu, còn size M không, ship bao lâu", chủ shop muốn trả lời nhanh mà vẫn đúng, để khách không bỏ đi | Chủ shop, khách | 40% tin nhắn là câu hỏi lặp lại ` |
| 3 | Pain từ người khác | Khi tôi nhắn hỏi mua hàng qua Facebook, tôi muốn được trả lời trong vài phút, để quyết định mua luôn thay vì sang shop khác | Người mua (chính tôi) | Lần gần nhất tôi chờ 3 giờ mới được trả lời và đã mua chỗ khác |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi bán cùng lúc trên Facebook, Zalo và Shopee, chủ shop muốn biết tổng số đơn và tồn kho thật, để không bán quá số hàng đang có | Chủ shop | 20 lần/tháng phải xin lỗi khách vì hết hàng sau khi đã chốt |
| 5 | Pain từ người khác | Khi giao hàng thất bại vì sai SĐT/địa chỉ, chủ shop muốn biết sớm trước khi gửi, để không mất phí ship 2 chiều | Chủ shop, đơn vị vận chuyển | 14 đơn hoàn/tháng do sai thông tin ; mỗi đơn hoàn mất phí ship chiều về |
| 6 | Lặp lại | Khi có sản phẩm mới, chủ shop muốn đăng lên nhiều kênh với mô tả phù hợp từng nơi, để không mất cả buổi tối đăng bài | Chủ shop | ~20 phút/sản phẩm × 5 kênh |
| 7 | Tốn thời gian | Khi cuối ngày đối soát, chủ shop muốn khớp tiền COD về với danh sách đơn, để biết đơn nào chưa thu tiền | Chủ shop | ~30 phút/ngày |
| 8 | Pain từ người khác | Khi nhận đánh giá 1–2 sao trên sàn, chủ shop muốn phản hồi sớm, để không ảnh hưởng điểm shop | Chủ shop, khách | 10 đánh giá xấu/tháng |

**Nếu có dùng AI để gợi ý thêm:** sau khi tự scan 6 ý, tôi hỏi AI thêm góc nhìn. Giữ lại ý #7 và #8 (đã viết lại theo bối cảnh shop nhỏ). Bỏ ý "chatbot AI bán hàng 24/7" vì là solution trá hình, không mô tả pain cụ thể.

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
| Actor | Chủ shop nhỏ (1–3 người), bán thời trang/mỹ phẩm qua Facebook Page và Zalo, ~20–50 tin nhắn/ngày `[xác nhận khi phỏng vấn]` |
| Thời điểm / bối cảnh | Buổi tối (giờ khách nhắn nhiều nhất) và sau mỗi buổi livestream |
| Quy trình hiện tại (3–7 bước) | 1. Mở inbox, lọc tin chưa đọc · 2. Trả lời câu hỏi giá/size/ship · 3. Kiểm tồn kho trong Sheet · 4. Xin tên, SĐT, địa chỉ · 5. Chép thông tin đơn sang Sheet/phần mềm vận chuyển · 6. Tạo vận đơn, gửi mã cho khách |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5: đọc lại đoạn chat, chép từng trường sang Sheet, ~1 phút/đơn, dễ chép sai SĐT/địa chỉ `[ĐO THẬT]` |
| Impact (nếu không giải thì sao) | ~___ phút/ngày; ___ đơn hoàn/tháng do sai thông tin (mất phí ship 2 chiều) |
| Success metric (baseline → target) | Thời gian từ "khách đồng ý mua" đến "đơn có trong Sheet": ~1 phút → ≤ 20 giây/đơn; đơn hoàn do sai thông tin: ___ → 0 |
| Phương án không dùng AI | Mẫu tin "xác nhận đơn" khách tự điền theo khuôn (Tên / SĐT / Địa chỉ / Sản phẩm / Size), hoặc gửi link Google Form |
| Giả thuyết về AI (nếu có) | AI đọc đoạn chat tự do, trích các trường đơn hàng thành 1 dòng; chủ shop duyệt rồi mới lưu |
| Cảm nhận nhanh | Rule hoặc Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 1 đơn, ~6 phút [ĐO THẬT]

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
| Impact (nếu không giải thì sao) | ___ lần/tháng hủy đơn vì hết hàng `[hỏi người bán]` |
| Success metric (baseline → target) | Số đơn hủy vì hết hàng: ___ → 0/tháng |
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
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: viết mô tả, ~5 phút/sản phẩm `[ĐO THẬT]` |
| Impact (nếu không giải thì sao) | ___ phút/tuần |
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
| Chưa có người bán thật nào xác nhận số liệu | Đồng ý | Đánh dấu mọi số là `[ĐO THẬT]`, lên kế hoạch phỏng vấn 2–3 chủ shop |
| Gợi ý chatbot tự chốt đơn và tự tạo vận đơn | Không đồng ý | Tạo vận đơn sai = mất tiền thật; giữ bước chủ shop duyệt trước khi lưu |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

> Tự điền bằng việc thật bạn đã làm trong buổi lab.

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Gợi ý thêm problem sau khi tự scan | Gợi ý đối soát COD, đánh giá xấu | Đưa ý "chatbot bán hàng 24/7" — solution trá hình | Bỏ ý đó |
| CP2 Problem Card | Đóng vai "PM hoài nghi" phản biện card #1 | Chỉ ra bước 2 tốn nhiều phút hơn bước 5 | Đề xuất chatbot tự tạo vận đơn | Giữ bước chủ shop duyệt |
| CP4 Research | Gợi ý công cụ có sẵn | Gợi ý Pancake, trả lời tự động của Meta, Shopee | Đưa link trang trợ giúp Meta bị lỗi 404 | Tự mở từng link, chỉ giữ link đã kiểm |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

> Tự viết, tối thiểu 200 từ cho 6.1–6.6. Không dùng AI viết thay (RUBRIC C4 = 0 nếu vi phạm).

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?**
*(Gợi ý tự soi: lúc đầu có nghĩ ngay tới "chatbot bán hàng" không?)*

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** *(tự viết 5–8 câu, không nhìn tài liệu: problem → quy trình → metric → boundary → mức can thiệp → quyết định)*

---

## 7. Tài liệu tham khảo

- Pancake: https://pancake.vn/
- Meta Business Suite — About Automated Responses: https://www.facebook.com/business/help/395965998733706
- Shopee Seller Education Hub — Auto-Reply in Chat Assistant: https://seller.shopee.com.my/edu/article/3719/auto-reply-in-chat-assistant
