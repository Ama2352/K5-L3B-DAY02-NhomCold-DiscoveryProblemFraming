# Báo cáo cá nhân — 2A202603945_VuLuongDuy

> ⚠️ **Trước khi nộp:** mọi chỗ đánh dấu `[ĐO THẬT]` là số ước tính ban đầu — thay bằng số bạn tự bấm giờ / đếm được (tin nhắn, lịch sử nộp bài). Mục 4–6 phải tự viết bằng trải nghiệm thật (RULES §2, RUBRIC C4). Xóa khối ghi chú này khi xong.

## 1. Thông tin học viên

- Họ tên: Vũ Lương Duy
- MSSV: 2A202603945
- Email trường (không bắt buộc):
- Tên nhóm: NhomCold
- Link repo nhóm: https://github.com/Ama2352/K5-L3B-DAY02-NhomCold-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi một tuần có nhiều lab và thông báo mới trên LMS, Discord lớp, email và README repo, tôi muốn biết chắc mình còn những bài gì phải nộp và hạn lúc nào, để không trễ hay sót bài | Học viên, coach (phải trả lời câu hỏi lặp lại) | ~20 phút/ngày lướt lại các kênh `[ĐO THẬT]`; tuần trước có ___ thông báo đổi hạn/đổi yêu cầu trên Discord `[ĐẾM]` |
| 2 | Lặp lại | Khi sắp tới deadline lab, tôi muốn đối chiếu bài của mình với RUBRIC và checklist SUBMISSION, để không mất điểm vì lỗi hình thức (sai tên file, thiếu mục) | Học viên | ~25 phút mỗi lab đọc lại rubric + checklist `[ĐO THẬT]`; rubric phạt 5 điểm nếu sai tên repo/file |
| 3 | Pain từ người khác | Khi nhóm trưởng cần cả nhóm cùng làm trên repo fork, thành viên muốn được mời collaborator và commit được ngay, để không mất đầu giờ lab | Thành viên nhóm, nhóm trưởng | Đầu buổi Day 02 mất ~15 phút để mời và chấp nhận lời mời `[ĐO THẬT]` |
| 4 | Tốn thời gian | Khi cả nhóm cùng sửa `group_report.md`, tôi muốn tránh xung đột merge, để không mất thời gian gộp lại nội dung | Cả nhóm (4 người) | ___ lần conflict trong Day 02 `[ĐẾM từ git log]`, mỗi lần ~10 phút |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi xem lại bài giảng để làm lab, tôi muốn tìm nhanh đoạn slide/video nói về một khái niệm, để không tua cả buổi học | Học viên | ~10–15 phút/lần, 2–3 lần/tuần `[ĐO THẬT]` |
| 6 | Pain từ người khác | Khi nhiều học viên hỏi lại cùng một câu về deadline/cách nộp trên Discord, coach muốn chỉ trả lời một lần, để có thời gian hỗ trợ chuyên môn | Coach, học viên | Đếm câu hỏi trùng về deadline/nộp bài trên kênh lớp tuần này: ___ `[ĐẾM]` |
| 7 | Lặp lại | Khi bắt đầu mỗi lab, tôi muốn có nhanh cấu trúc file báo cáo đúng tên, để bắt tay vào nội dung luôn | Học viên | ~5–10 phút/lab đổi tên file, sửa tiêu đề `[ĐO THẬT]` |

**Nếu có dùng AI để gợi ý thêm:** sau khi tự scan 6 ý, tôi hỏi AI thêm góc nhìn. Giữ ý #7 (đã viết lại theo trải nghiệm của mình). Bỏ ý "trợ lý học tập cá nhân hóa cho mọi môn" vì quá rộng, không có quy trình cụ thể và là solution trá hình.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Theo dõi deadline rải rác nhiều kênh (#1) | Lặp lại hằng ngày, nhiều người gặp, đo được (thời gian lướt kênh, số bài trễ) | Bao nhiêu % deadline chỉ nằm ở chat, không có trên LMS? |
| 2 | Tự kiểm bài theo rubric trước khi nộp (#2) | Có tiêu chí đúng/sai rõ, phạt điểm thật | Có thể chỉ là vấn đề đọc kỹ, không phải bottleneck lớn |
| 3 | Câu hỏi trùng về deadline cho coach (#6) | Pain từ người khác, liên quan #1 | Chưa hỏi coach, chưa có số liệu |

### Problem Card #1 — Theo dõi deadline rải rác

| Trường | Nội dung |
|---|---|
| Job Story | Khi một tuần có nhiều lab và thông báo mới ở nhiều kênh, tôi muốn biết chắc mình còn bài gì phải nộp và hạn lúc nào, để không trễ hay sót bài |
| Actor | Học viên khóa K5 đang học song song nhiều lab/tuần |
| Thời điểm / bối cảnh | Tối mỗi ngày học, và đặc biệt sau khi coach thông báo đổi hạn / gia hạn |
| Quy trình hiện tại (3–7 bước) | 1. Mở LMS xem bài tập · 2. Lướt Discord/Zalo lớp tìm thông báo mới · 3. Mở email trường · 4. Đọc README/SUBMISSION trong repo lab để biết giờ hạn (sáng vs chiều/tối) · 5. Tự ghi vào note/lịch · 6. Hỏi lại bạn hoặc coach khi thấy thông tin mâu thuẫn |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2: lướt lại tin nhắn chat để tìm thông báo đổi hạn bị trôi, ~10 phút/ngày `[ĐO THẬT]` |
| Impact (nếu không giải thì sao) | ~20 phút/ngày ≈ 100 phút/tuần `[ĐO THẬT]`; nguy cơ nộp trễ = commit sau deadline không được chấm (RULES §6) |
| Success metric (baseline → target) | Thời gian kiểm tra deadline: ~20 → ≤ 5 phút/ngày; số bài trễ/sót do không biết hạn: ___ → 0 trong 2 tuần |
| Phương án không dùng AI | Đăng ký lịch LMS vào Google Calendar + 1 kênh "#thong-bao-deadline" chỉ coach được đăng, theo mẫu cố định |
| Giả thuyết về AI (nếu có) | AI đọc tin nhắn tự do trên Discord, trích ra (bài, hạn mới) để người duyệt rồi thêm vào lịch |
| Cảm nhận nhanh | Rule (có thể Workflow cho phần chat) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~20 phút/ngày [ĐO THẬT]

[1 Mở LMS: 3'] → [2 Lướt Discord/Zalo: 10'] ← BOTTLENECK
→ [3 Email: 2'] → [4 Đọc README/SUBMISSION: 2'] → [5 Ghi vào note: 2']
→ [6 Hỏi lại khi mâu thuẫn: ~5', 2–3 lần/tuần]
```

### Problem Card #2 — Tự kiểm bài theo rubric

| Trường | Nội dung |
|---|---|
| Job Story | Khi sắp tới deadline lab, tôi muốn đối chiếu bài với RUBRIC và SUBMISSION, để không mất điểm vì lỗi hình thức |
| Actor | Học viên / nhóm trưởng trước khi nộp |
| Thời điểm / bối cảnh | 1–2 giờ trước deadline |
| Quy trình hiện tại (3–7 bước) | 1. Mở RUBRIC · 2. Mở SUBMISSION checklist · 3. Đối chiếu tên repo, tên file · 4. Đọc lại từng mục báo cáo xem đủ trường chưa · 5. Sửa · 6. Commit + push |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: đọc lại từng mục so với rubric, ~15 phút `[ĐO THẬT]` |
| Impact (nếu không giải thì sao) | Sai tên file/repo: −5 điểm; thiếu mục: mất điểm tiêu chí tương ứng |
| Success metric (baseline → target) | 25 → 10 phút/lab; 0 lỗi hình thức bị trừ điểm |
| Phương án không dùng AI | Checklist in sẵn; script kiểm tên file theo regex `MSSV_HoTen.md` |
| Giả thuyết về AI (nếu có) | AI đọc báo cáo, chỉ ra mục còn trống hoặc thiếu baseline/target |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~25 phút/lab [ĐO THẬT]

[1 Mở RUBRIC: 2'] → [2 Mở SUBMISSION: 2'] → [3 Check tên: 2']
→ [4 Đọc lại từng mục: 15'] ← BOTTLENECK → [5 Sửa + push: 4']
```

### Problem Card #3 — Câu hỏi trùng cho coach

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhiều học viên hỏi cùng một câu về deadline/cách nộp, coach muốn chỉ trả lời một lần, để dành thời gian hỗ trợ chuyên môn |
| Actor | Coach / trợ giảng |
| Thời điểm / bối cảnh | Trong và sau giờ lab, gần deadline |
| Quy trình hiện tại (3–7 bước) | 1. Đọc câu hỏi trên Discord · 2. Kiểm tra lại thông báo cũ · 3. Trả lời / dán lại link · 4. Lặp lại với câu hỏi trùng |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: trả lời lặp lại, ~2 phút × ___ câu/ngày `[cần hỏi coach]` |
| Impact (nếu không giải thì sao) | Coach mất thời gian, học viên chờ câu trả lời |
| Success metric (baseline → target) | Số câu hỏi trùng/tuần: ___ → giảm 50% |
| Phương án không dùng AI | FAQ ghim + kênh thông báo một chiều |
| Giả thuyết về AI (nếu có) | Bot trả lời FAQ dựa trên README/SUBMISSION |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — ~2' × N câu/ngày [cần số thật từ coach]

[1 Đọc câu hỏi: 0.5'] → [2 Tìm lại thông báo cũ: 1'] → [3 Trả lời: 0.5']
→ [4 Lặp lại với câu trùng] ← BOTTLENECK
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: gặp hằng ngày, ảnh hưởng tới cả lớp, đo được, và có thể so sánh rõ No AI / Rule / Workflow / Agent.
- Câu hỏi muốn nhóm phản biện: "Nếu LMS đã có lịch, thì bao nhiêu deadline thật sự chỉ nằm trong chat? Pain có đủ lớn không?"

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Baseline "20 phút/ngày" là ước lượng theo trí nhớ | Đồng ý | Bấm giờ thật 2–3 buổi tối và ghi lại `[ĐIỀN SỐ]` |
| Có thể pain thật là "thông báo không có nguồn chính thức duy nhất", không phải "thiếu công cụ" | Đồng ý | Thêm phương án No AI (kênh thông báo một chiều) vào card |
| Gợi ý làm bot AI tự thêm mọi tin nhắn vào lịch | Không đồng ý | AI có thể hiểu nhầm tin nhắn bàn luận thành deadline; giữ bước người duyệt |

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
| CP1 Scan | Gợi ý thêm problem sau khi tự scan | Gợi ý ý "tạo cấu trúc file báo cáo" | Đưa ý quá rộng ("trợ lý học tập cho mọi môn") | Bỏ ý đó vì không có quy trình, không đo được |
| CP2 Problem Card | Đóng vai "PM hoài nghi" phản biện card #1 | Chỉ ra baseline dựa trên trí nhớ | Đề xuất bot tự thêm lịch, không có người duyệt | Giữ bước người duyệt làm boundary |
| CP4 Research | Gợi ý công cụ có sẵn | Gợi ý Moodle calendar export, Todoist | `[ghi chỗ AI sai, ví dụ link sai / tính năng không đúng gói]` | Tự mở từng link, chỉ giữ link đã kiểm |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

> Tự viết, tối thiểu 200 từ cho 6.1–6.6. Không dùng AI viết thay (RUBRIC C4 = 0 nếu vi phạm). Gợi ý câu hỏi tự soi nằm trong đề mục.

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?**
*(Gợi ý tự soi: bản đầu tiên của nhóm có chép hướng "báo cáo tuần PM" từ bài mẫu không? Vì sao đổi?)*

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** *(tự viết 5–8 câu, không nhìn tài liệu: problem → quy trình → metric → boundary → mức can thiệp → quyết định)*

---

## 7. Tài liệu tham khảo

- Moodle Docs — Calendar export: https://docs.moodle.org/en/Calendar_export
- Todoist Help — Quick Add: https://www.todoist.com/help/articles/use-task-quick-add-in-todoist-va4Lhpzz
- Google Calendar Help — Events from Gmail: https://support.google.com/calendar/answer/6084018
