---
artifact: 02 — JTBD Project Analysis
bai-tap: Lab 2 — Dùng JTBD để soi lại dự án nhóm
format: Theo nhóm dự án → share trong bàn → chốt hypothesis cuối
time: 25 phút trên lớp
nop-cuoi: Có — đây là file nộp cuối của Lab 2
companion-reference: Strategyn_JTBD_Playbook.pdf (giảng viên gửi kèm)
---

# Lab 2 — JTBD Project Analysis / Dùng JTBD để soi lại dự án nhóm

**Tên dự án / sản phẩm:** DebugMate - trợ lý xác thực và hướng dẫn sửa lỗi code cho junior developer

> Đây là **file duy nhất** của Lab 2.  
> File này đồng thời đóng vai trò:
>
> - guide từng bước,
> - worksheet để điền trực tiếp,
> - và file nộp cuối cho người chấm.

Mục tiêu của bài này không phải brainstorm thêm thật nhiều tính năng AI.
Mục tiêu là:

1. **xác định người dùng thực sự đang cố hoàn thành job gì**
2. **hiểu họ đang dùng giải pháp nào để hoàn thành job đó hôm nay**
3. **chỉ ra AI nên chen vào đúng bước nào trong workflow**
4. **viết ra product hypothesis và assumption còn phải validate**

Quy tắc xuyên suốt: **không rõ job thì đừng bàn feature.**

---

## Cần mở song song 2 thứ

1. **File này** — để điền trực tiếp
2. **`Strategyn_JTBD_Playbook.pdf`** — giảng viên gửi kèm

### Cách dùng playbook cho đúng

Bạn **không cần đọc hết 48 trang**.  
Trong bài này, playbook chủ yếu dùng để tra 4 thứ:

1. **Cách nhìn thị trường qua JTBD lens**
2. **`Job executor` là ai**
3. **Cách viết `job statement`: `verb + object + contextual clarifier`**
4. **8 bước của `job map`**:
   `define -> locate -> prepare -> confirm -> execute -> monitor -> modify -> conclude`

### 2 chương nên mở nhiều nhất

- **Chapter 2 — Define Your Market**
- **Chapter 3 — Build Your Job Map**

> Dùng playbook để **tra framework và ví dụ**.  
> Dùng file này để **làm bài và chốt output**.

---

## Đầu ra bắt buộc

Người chấm cần thấy đủ 6 phần trong chính file này:

1. **`Project slice` + market context**
2. **`Job executor` + `core JTBD`**
3. **3 `job stories`**
4. **`JTBD lite map` + pain points**
5. **`AI leverage point` + `product hypothesis`**
6. **`Assumptions to validate` + verdict cuối sau thảo luận**

Nếu thiếu một trong sáu phần trên, bài sẽ bị xem là chưa hoàn chỉnh.

---

## Cách làm trong lớp (25 phút)

```text
3'  Chốt 1 lát cắt cụ thể của dự án
7'  Viết market context + job executor + core JTBD
6'  Viết 3 job stories + current alternatives
6'  Điền JTBD lite map + AI leverage point + hypothesis
3'  Share trong bàn và sửa version cuối
```

> Nếu dự án làm theo nhóm, cả nhóm có thể thảo luận chung.  
> Nhưng file này vẫn nên có **version chốt rõ ràng** của người nộp.

---

## Bước 0 — Khoanh đúng 1 lát cắt của dự án

Phần lớn dự án nhóm viết quá rộng ở bước này, rồi sau đó mọi thứ mơ hồ theo.

### Khoanh đúng 1 lát cắt theo 4 điểm

- [x] **1 nhóm người dùng chính**
- [x] **1 hoàn cảnh / tình huống rõ**
- [x] **1 job cốt lõi**
- [x] **1 workflow đủ cụ thể để vẽ ra được**

### Điền nhanh trước khi làm

- **Dự án của nhóm tôi là:** DebugMate - công cụ giúp developer chẩn đoán lỗi, hiểu nguyên nhân và chọn hướng sửa có kiểm chứng.
- **Lát cắt tôi chọn để phân tích hôm nay là:** Junior developer trong 6 tháng đầu đi làm, đang bị lỗi build/test/runtime chặn task sprint và cần sửa đủ chắc để tạo pull request.
- **Vì sao tôi chọn lát cắt này:**  
  > Lát cắt này đủ hẹp để vẽ workflow: gặp lỗi, đọc log, tìm nguyên nhân, thử hướng sửa, chạy test, hỏi senior nếu chưa chắc, rồi commit/PR. Đây cũng là nơi AI có thể giúp mạnh nhưng rủi ro hallucination cao, nên cần JTBD để xác định AI nên chen vào bước nào.

### Viết quá rộng vs viết sắc hơn

| Viết quá rộng | Viết sắc hơn |
|---|---|
| Giúp SME dùng AI để marketing | Giúp chủ shop online phản hồi câu hỏi trước mua hàng nhanh và nhất quán trong giờ cao điểm |
| Dùng AI để làm slide | Tạo bản nháp deck nội bộ mạch lạc cho buổi họp gấp trong thời gian rất ngắn |
| AI cho tuyển dụng | Giúp recruiter sàng lọc CV đầu vào nhanh hơn trước vòng gọi sơ bộ |

> Nếu bạn không mô tả được **một hoàn cảnh cụ thể**, khả năng cao bạn đang viết quá rộng.

---

## Bước 1 — Viết `Project Snapshot`

### Tóm tắt dự án trong 3 dòng

1. **Nhóm tôi đang nghĩ mình đang giải quyết vấn đề gì?**  
   > Junior developer mất nhiều thời gian chuyển qua lại giữa IDE, Google, Stack Overflow, tài liệu, ChatGPT và senior để hiểu lỗi; họ thường có câu trả lời nhanh nhưng không biết câu nào đủ đúng với codebase hiện tại.

2. **Người dùng chính hiện nhóm đang nhắm tới là ai?**  
   > Junior developer, intern developer hoặc fresher developer trong team sản phẩm/web/backend nhỏ, phải tự xử lý bug/task hằng ngày nhưng chưa đủ kinh nghiệm để nhanh chóng xác định nguyên nhân gốc.

3. **Hiện tại người dùng đó đang giải quyết vấn đề này bằng cách nào?**  
   > Họ copy lỗi lên Google/Stack Overflow/ChatGPT, đọc docs, thử nhiều snippet, chạy test lại, rồi hỏi senior khi bị kẹt hoặc khi không đủ tự tin commit.

---

## Bước 2 — Viết `Market Context`

Ở đây chưa cần solution. Chỉ cần bối cảnh thị trường đủ để hiểu:
**ai đang gặp chuyện gì, trong hoàn cảnh nào, và vì sao bây giờ đáng giải.**

### Trả lời 4 câu ngắn

1. **Ai đang gặp vấn đề này?**  
   > Junior developer/fresher developer đang làm task thật trong sprint, đặc biệt là người chưa quen codebase, framework hoặc convention của team.

2. **Vấn đề xuất hiện trong hoàn cảnh nào?**  
   > Vấn đề xuất hiện khi code không chạy, build/test fail, API trả lỗi lạ, hoặc một thay đổi nhỏ làm hỏng flow khác ngay trước deadline PR/demo.

3. **Hiện tại họ đang dùng giải pháp thay thế nào?**  
   > Google, Stack Overflow, tài liệu chính thức, ChatGPT/Copilot/Cursor, search trong codebase, hỏi senior, hoặc trial-and-error bằng cách sửa rồi chạy lại.

4. **Vì sao đây là thời điểm đáng giải?**  
   > AI coding tools đã làm developer quen với câu trả lời tức thì, nhưng độ tin cậy vẫn là vấn đề lớn. Sau Lab 1, bài học từ Stack Overflow là entry point đã chuyển sang AI trong workflow, nên sản phẩm mới phải vừa nhanh vừa có cơ chế kiểm chứng.

### Tóm tắt market context trong 3-4 dòng

> Junior developer vẫn phải tự hoàn thành task, nhưng workflow debug hiện tại bị vỡ thành nhiều công cụ rời rạc: IDE, search, forum, docs, AI chat và senior.
> Thị trường đáng giải lúc này vì AI đã khiến kỳ vọng “trả lời ngay trong context của tôi” trở thành mặc định, nhưng câu trả lời nhanh chưa đồng nghĩa với câu trả lời đúng. Cơ hội của DebugMate là đứng ở lớp chẩn đoán và xác thực, không chỉ sinh thêm code.

---

## Bước 3 — Xác định `Job Executor`

`Job executor` là người **trực tiếp dùng một giải pháp để hoàn thành job**.

### Đừng nhầm với:

- người mua tiền nhưng không trực tiếp làm job
- người ảnh hưởng quyết định
- cả một công ty hay một phòng ban quá rộng

### Gợi ý viết cho đúng

- Sai hoặc quá rộng: `SME`, `doanh nghiệp`, `thị trường`
- Tốt hơn: `chủ shop online`, `nhân viên CSKH`, `recruiter`, `sales ops manager`

### Điền

- **Job executor của dự án này là:** Junior developer đang trực tiếp xử lý lỗi trong task được giao.
- **Vì sao tôi tin đây là người trực tiếp "thuê" giải pháp để làm job:**  
  > Đây là người trực tiếp mở IDE, đọc log, tìm nguyên nhân, thử fix, chạy test và quyết định có cần hỏi senior hay không. Tech lead có thể là buyer/influencer, nhưng người thực hiện job hằng ngày là junior developer.

---

## Bước 4 — Viết `Core JTBD`

`Core JTBD` là công việc cốt lõi người dùng đang cố hoàn thành.

### Công thức gợi ý

```text
[verb] + [object] + [contextual clarifier]
```

### Ví dụ

- Chưa tốt: `trả lời inbox bằng AI`
- Tốt hơn: `giải quyết câu hỏi trước mua hàng nhanh và chính xác trong giờ cao điểm`

- Chưa tốt: `dùng AI để viết nội dung`
- Tốt hơn: `tạo bản nháp nội dung chiến dịch phù hợp với brand trong thời gian rất ngắn`

### 3 tiêu chí tự kiểm

- [x] Nếu bỏ tool hiện tại đi, job này vẫn còn tồn tại
- [x] Trong câu không có tên sản phẩm, AI, chatbot, app, màn hình
- [x] Câu đang mô tả **điều user muốn hoàn thành**, không phải thứ product đang làm

### Bản nháp 1

**Core JTBD bản nháp:**  
> Sửa lỗi code nhanh hơn bằng AI để kịp hoàn thành task.

### Gạch bỏ từ solution nếu có

- Các từ solution tôi đang lỡ nhét vào câu: `AI`, `sửa bằng công cụ`, `nhanh hơn` theo kiểu mô tả feature thay vì job.

### Bản chốt

**Core JTBD cuối cùng:**  
> Chẩn đoán và sửa lỗi code đang chặn tiến độ trong lúc thực hiện task sprint với đủ độ tin cậy để đưa vào codebase.

---

## Bước 5 — Viết 3 `Job Stories`

Nếu `core JTBD` là job ở mức cốt lõi, thì `job story` giúp bạn thấy
**job này xuất hiện trong hoàn cảnh nào**.

### Format

```text
When [trigger], I want to [motivation], so I can [outcome].
```

### Ví dụ

`When inbox đổ dồn vào buổi tối, tôi muốn có câu trả lời nhất quán ngay lập tức, so I can không mất đơn vì phản hồi chậm.`

### Bảng 3 job stories

| # | Trigger / When | Motivation / I want to | Outcome / so I can | Điều story này cho thấy |
|---|---|---|---|---|
| JS1 | Khi build/test fail ngay trước lúc tôi cần tạo PR | Tôi muốn nhanh chóng biết lỗi đến từ file, config hay thay đổi nào | Tôi có thể sửa đúng chỗ và không trễ deadline sprint | Pain nằm ở chẩn đoán nguyên nhân, không chỉ ở viết code mới |
| JS2 | Khi tôi gặp lỗi từ framework/library chưa quen | Tôi muốn hiểu API, version hoặc config nào đang liên quan | Tôi tránh copy snippet sai hoặc sửa bừa làm phát sinh lỗi khác | User cần giải thích có ngữ cảnh và nguồn đáng tin |
| JS3 | Khi Google/Stack Overflow/ChatGPT đưa nhiều hướng sửa khác nhau | Tôi muốn biết hướng nào an toàn nhất với codebase hiện tại | Tôi commit tự tin hơn và giảm số lần phải hỏi senior | Giá trị chính là xác thực, không phải chỉ tạo thêm đáp án |

### Tự kiểm nhanh

- [x] Mỗi story là một **tình huống thật**, không phải slogan chung chung
- [x] 3 story không trùng hệt nhau
- [x] Sau khi đọc 3 story, tôi hình dung được lúc nào product của mình đáng xuất hiện

---

## Bước 6 — Liệt kê `Current Alternatives`

Qua JTBD lens, đối thủ không chỉ là app cùng ngành.
Đối thủ là **bất kỳ thứ gì user đang "thuê" để làm job**:

- thao tác tay
- file Excel / Google Sheets
- intern / nhân viên
- agency
- ChatGPT / Claude / Gemini
- công cụ chuyên dụng khác
- hoặc thậm chí là **không làm gì cả**

### Bảng alternatives

| Alternative hiện tại | User đang thuê nó để làm gì? | Nó làm tốt gì? | Nó fail ở đâu? | Switching cost hiện tại cao hay thấp? |
|---|---|---|---|---|
| Google / Stack Overflow / tài liệu chính thức | Tìm lỗi giống mình, đọc giải thích, lấy snippet hoặc cấu hình mẫu | Rộng, miễn phí, có nhiều dấu vết cộng đồng và tài liệu gốc | Không luôn khớp version/codebase; tốn thời gian lọc; nhiều thread cũ hoặc thiếu context | Thấp |
| ChatGPT / Copilot / Cursor | Giải thích lỗi, gợi ý nguyên nhân, sinh hướng sửa nhanh | Rất nhanh, hội thoại được, có thể cá nhân hóa theo prompt/code đang mở | Có thể hallucinate, thiếu nguồn, tự tin quá mức; user khó biết khi nào nên tin | Thấp đến trung bình |
| Hỏi senior / mentor trong team | Xác nhận nguyên nhân và hướng sửa phù hợp với codebase | Đáng tin, hiểu context team, giúp junior học nhanh | Senior là bottleneck; có social cost; không phải lúc nào cũng sẵn sàng | Cao về thời gian và quan hệ |

### Kết luận nhanh

**Nếu project của tôi biến mất hôm nay, user nhiều khả năng sẽ quay về:**  
> ChatGPT/Cursor để có câu trả lời nhanh, rồi hỏi senior để xác nhận khi không đủ tự tin. Google/Stack Overflow vẫn được dùng cho lỗi phổ biến hoặc để tìm nguồn kiểm chứng.

---

## Bước 7 — Điền `JTBD Lite Map`

Đây là bản rút gọn của `job map` trong playbook.

### Mục tiêu

Không phải để làm consultant workshop hoàn chỉnh.  
Mục tiêu là nhìn ra:

1. workflow hiện tại của user đi qua những bước nào
2. bước nào đang đau nhất
3. AI có nên chen vào đó không

### 8 bước tham chiếu từ playbook

1. `Define`
2. `Locate`
3. `Prepare`
4. `Confirm`
5. `Execute`
6. `Monitor`
7. `Modify`
8. `Conclude`

> Không nhất thiết bước nào cũng quan trọng như nhau trong dự án của bạn.  
> Nếu ít liên quan, ghi `N/A`, đừng để trống.

### Bảng JTBD Lite Map

| Step | Trong workflow này user đang cố làm gì? | Hôm nay họ đang dùng gì? | Friction / pain hiện tại | Mức đau |
|---|---|---|---|---|
| Define | Xác định lỗi nào đang chặn task và kết quả mong muốn sau khi sửa | Ticket/Jira, IDE, terminal, log, test report | Junior dễ nhầm triệu chứng với nguyên nhân; chưa biết lỗi nào quan trọng nhất | Med |
| Locate | Tìm file, function, config, dependency hoặc thread/docs liên quan | IDE search, grep, Google, Stack Overflow, docs | Mất thời gian lọc; kết quả ngoài web thường không khớp codebase/version | High |
| Prepare | Gom error message, stack trace, đoạn code, version, test fail để hỏi hoặc phân tích | Copy/paste thủ công vào ChatGPT/senior, screenshot, log | Context bị thiếu hoặc quá dài; dễ lộ thông tin nhạy cảm; prompt rời rạc | High |
| Confirm | Xác định nguyên nhân gốc và chọn hướng sửa đáng tin | Chạy test, đọc docs, hỏi senior, so nhiều câu trả lời AI | Khó biết AI/snippet có đúng không; user sợ sửa sai làm hỏng phần khác | High |
| Execute | Sửa code/config theo hướng đã chọn | IDE, Copilot/Cursor, manual edit | Viết code không phải điểm đau lớn nhất nếu nguyên nhân đã rõ | Med |
| Monitor | Chạy lại test/build/local flow để xem lỗi còn không | Terminal, test runner, CI, log | Test lâu, lỗi phụ xuất hiện, khó đọc log tiếp theo | Med |
| Modify | Điều chỉnh hướng sửa khi test vẫn fail hoặc phát sinh lỗi mới | Trial-and-error, hỏi AI tiếp, hỏi senior | Dễ vòng lặp sửa bừa; mất tự tin; context hội thoại bị trôi | High |
| Conclude | Viết commit/PR note, giải thích nguyên nhân và cách test | Git, GitHub/GitLab, Jira | Ít đau hơn, nhưng junior đôi khi giải thích thiếu rõ ràng | Low |

### Chốt 2 bước đau nhất

**Bước đau nhất #1:** Confirm - xác nhận nguyên nhân gốc và hướng sửa đáng tin
**Bước đau nhất #2:** Locate / Prepare - tìm và gom đúng context trước khi phân tích

**Vì sao đây là nơi đáng chú ý nhất:**  
> Nếu locate/prepare sai, AI hoặc senior đều nhận context thiếu và trả lời lệch.
> Nếu confirm sai, user có thể sửa nhanh nhưng sai hướng, tạo bug mới hoặc mất thêm thời gian hỏi lại senior. Đây là điểm product nên thắng bằng trust, không chỉ bằng tốc độ sinh code.

---

## Bước 8 — Chỉ ra `AI Leverage Point`

Sau khi map workflow, mới hỏi:
**AI nên vào đâu, với vai trò gì, và vì sao là ở đó?**

### Nhắc nhanh

- Đừng nhét AI vào chỉ vì "có AI thì nghe hay"
- Nếu pain lớn nhất không nằm ở chỗ AI giải tốt, hãy thành thật ghi ra
- Nếu current alternative đã đủ tốt, project cần xem lại

### Bảng leverage point

| Step | AI nên giúp bằng cách nào? | Vì sao AI hợp ở đây? | Rủi ro chính nếu dùng AI |
|---|---|---|---|
| Locate / Prepare | Tự gom stack trace, file liên quan, dependency/version và lịch sử thay đổi gần nhất thành một debugging brief ngắn | AI mạnh ở việc đọc nhiều ngữ cảnh rời rạc, tóm tắt và phát hiện pattern ban đầu | Lấy thiếu context, lộ thông tin nhạy cảm, hoặc tóm tắt sai mức ưu tiên |
| Confirm / Modify | Đề xuất 1-3 giả thuyết nguyên nhân, hướng sửa tối thiểu, nguồn/docs liên quan và test cần chạy để kiểm chứng | AI tạo giá trị khi biến câu trả lời thành kế hoạch kiểm chứng, giúp junior không chỉ “tin đại” | Hallucination, overconfidence, đề xuất fix không phù hợp convention/codebase |

### Kết luận nhanh

**AI leverage point quan trọng nhất của dự án tôi là:**  
> Dùng AI để chẩn đoán có kiểm chứng: gom đúng context, nêu giả thuyết nguyên nhân, đề xuất hướng sửa tối thiểu và kèm bước test/xác minh.

**Vì sao không phải ở bước khác:**  
> Nếu chỉ dùng AI ở bước execute để sinh code, sản phẩm sẽ giống Copilot/Cursor và dễ bị thay thế. Điểm đau lớn hơn nằm ở việc junior không biết nên tin hướng sửa nào và cần kiểm chứng ra sao trước khi đưa vào codebase.

---

## Bước 9 — Viết `Product Hypothesis`

Bây giờ mới đến lúc viết hypothesis.

### Công thức gợi ý

```text
Nếu chúng ta giúp [job executor] làm [job / sub-job] tốt hơn ở bước [x],
bằng cách [AI leverage],
thì họ sẽ chuyển từ [current alternative] sang [hướng giải pháp của nhóm],
vì [giá trị rõ nhất].
```

### Bản hypothesis của tôi

> Nếu chúng ta giúp junior developer chẩn đoán và xác minh hướng sửa lỗi ở bước Locate/Prepare và Confirm,
> bằng cách AI đọc error, log, code context, docs liên quan và đề xuất test kiểm chứng, thì họ sẽ chuyển từ Google/Stack Overflow/ChatGPT rời rạc sang DebugMate trong workflow IDE/PR, vì họ nhận được câu trả lời nhanh hơn nhưng vẫn có traceability và giảm số lần phải hỏi senior.

### Tín hiệu sớm nếu hypothesis này đúng

1. Trong pilot, junior developer giải quyết được phần lớn lỗi phổ biến trong vòng 15-20 phút mà không cần hỏi senior ngay từ đầu.
2. User quay lại dùng cho nhiều bug/task trong tuần và chủ động chạy test/đọc nguồn kiểm chứng do sản phẩm gợi ý trước khi tạo PR.

---

## Bước 10 — Liệt kê `Assumptions to Validate`

Job story chưa có research vẫn chỉ là **giả thuyết tốt hơn**, chưa phải sự thật.

### 5 assumption thường đáng kiểm

- Tôi đã chọn đúng `job executor`
- Pain này thật sự đủ đau và xảy ra đủ thường xuyên
- User sẽ đổi khỏi alternative hiện tại nếu có giải pháp tốt hơn
- AI thực sự tạo giá trị ở step tôi chọn
- User đủ tin kết quả AI để đưa vào workflow thật

### Bảng assumptions

| Assumption | Vì sao assumption này rủi ro? | Tôi đang có bằng chứng gì? | Cần validate bằng cách nào tiếp theo? |
|---|---|---|---|
| A1: Junior developer là job executor đúng | Có thể người ra quyết định thật là tech lead, còn junior chỉ dùng theo tool team chọn | Workflow debug hằng ngày do junior trực tiếp làm; họ là người cảm pain đầu tiên | Phỏng vấn 5-7 junior/fresher và 2-3 tech lead để tách user, buyer, influencer |
| A2: Pain đủ thường xuyên và đủ đau | Nếu lỗi khó không xảy ra thường xuyên, sản phẩm chỉ là tiện ích phụ | Bug/build/test fail là hoạt động thường ngày trong dev workflow, nhưng mức đau thay đổi theo team | Diary study 1 tuần: ghi số lần bị block, thời gian mất, số lần hỏi senior |
| A3: User tin AI hơn nếu có nguồn và test kiểm chứng | Có nguồn/test chưa chắc đủ để user tin, nhất là code production | Lab 1 cho thấy developer dùng AI nhiều nhưng vẫn nghi ngờ accuracy; trust là khoảng trống thật | Prototype có citation/test plan, đo mức confidence trước/sau và tỷ lệ accept suggestion |
| A4: AI có đủ context codebase để chẩn đoán đúng | Nếu không truy cập đúng file/log/dependency, output vẫn chung chung như ChatGPT | Current alternatives fail nhiều vì thiếu context riêng của repo | Thử trên 20 lỗi thật đã có lời giải, so accuracy giữa ChatGPT thường và bản có context repo |
| A5: Giá trị đủ mạnh để thắng current alternatives miễn phí | Google/Stack Overflow/ChatGPT/Cursor có sẵn và switching cost thấp | Pain lớn nhất không phải “không có câu trả lời” mà là “không biết câu nào đáng tin” | Test willingness-to-switch: cho user xử lý cùng bug bằng alternative hiện tại và prototype, đo thời gian + niềm tin + ý định dùng lại |

### Assumption nguy hiểm nhất nếu tôi đang sai

> Nguy hiểm nhất là A3: junior developer không đủ tin kết quả AI dù có citation và test plan. Nếu trust không tăng, DebugMate sẽ chỉ là một AI answer generator khác và khó thắng ChatGPT/Cursor.

---

## Bước 11 — Share trong bàn (3')

### Mỗi người / mỗi nhóm chỉ nói 4 thứ

1. **Job executor của bạn là ai**
2. **Core JTBD của bạn là gì**
3. **Step đau nhất đang nằm ở đâu**
4. **AI leverage point + assumption rủi ro nhất là gì**

### Nếu chưa biết hỏi ngược gì, dùng 4 câu này

1. **"Câu JTBD này có đang lỡ nhét solution vào không?"**
2. **"Alternative hiện tại của user là gì, và tại sao họ chưa bỏ nó?"**
3. **"Pain mạnh nhất nằm ở bước nào trong workflow, có chắc AI giải tốt được không?"**
4. **"Assumption nào nếu sai thì cả hypothesis sẽ sập?"**

### Ghi nhanh sau khi nghe bàn phản biện

| Ý phản biện tôi nghe được | Nó chạm vào phần nào? | Tôi sẽ giữ / sửa gì? |
|---|---|---|
| Có thể người dùng thật không phải junior mà là tech lead muốn giảm thời gian review/hỗ trợ | Job executor / buyer | Giữ junior là job executor, nhưng ghi tech lead là buyer/influencer cần validate |
| Current alternative mạnh nhất có thể là hỏi senior, không phải Stack Overflow hay ChatGPT | Alternatives / switching cost | Sửa hypothesis để nhấn mạnh giảm số lần hỏi senior, không thay thế hoàn toàn senior |
| AI sinh code dễ bị trùng với Copilot/Cursor; khác biệt phải nằm ở kiểm chứng | AI leverage point | Giữ leverage point ở Confirm/Modify và thêm citation/test plan làm phần giá trị chính |

---

## Bước 12 — Chốt version cuối sau thảo luận

### Sau khi nghe phản biện, tôi thay đổi gì?

- [x] Giữ nguyên `job executor`
- [ ] Sửa `job executor`
- [ ] Giữ nguyên `core JTBD`
- [x] Sửa `core JTBD`
- [x] Giữ nguyên `AI leverage point`
- [ ] Sửa `AI leverage point`
- [ ] Giữ nguyên `product hypothesis`
- [x] Sửa `product hypothesis`

### Vì sao tôi giữ / sửa?

> Tôi giữ junior developer là job executor vì họ là người trực tiếp bị block, tự đọc lỗi và tự thử fix hằng ngày.
> Tôi sửa nhẹ core JTBD và hypothesis để tránh biến sản phẩm thành “AI viết code”; trọng tâm cuối cùng là chẩn đoán và xác minh hướng sửa đủ tin cậy, đồng thời giảm phụ thuộc vào senior ở các lỗi thường gặp.

### Version cuối cùng tôi nộp

**Job executor:**  
> Junior developer đang trực tiếp xử lý lỗi trong task được giao.

**Core JTBD:**  
> Chẩn đoán và sửa lỗi code đang chặn tiến độ trong lúc thực hiện task sprint với đủ độ tin cậy để đưa vào codebase.

**2 bước đau nhất trong workflow:**  
> Confirm - xác nhận nguyên nhân/hướng sửa đáng tin; Locate/Prepare - tìm và gom đúng context trước khi phân tích.

**AI leverage point chính:**  
> AI gom context, nêu giả thuyết nguyên nhân, đề xuất hướng sửa tối thiểu và kèm nguồn/test để user kiểm chứng trước khi commit.

**Product hypothesis:**  
> Nếu DebugMate giúp junior developer chẩn đoán và xác minh hướng sửa lỗi trong IDE/PR workflow, họ sẽ chuyển bớt từ Google/Stack Overflow/ChatGPT rời rạc sang DebugMate vì nhận được câu trả lời nhanh hơn, có ngữ cảnh codebase hơn và giảm số lần phải hỏi senior.

**Assumption cần validate đầu tiên:**  
> Junior developer có thực sự tin và dùng đề xuất AI nhiều hơn khi output có nguồn, context repo và test plan kiểm chứng hay không.

---

## Checklist trước khi nộp

- [x] Tôi đã khoanh đúng 1 lát cắt cụ thể của dự án.
- [x] Tôi đã phân biệt được `job executor` với buyer / influencer.
- [x] `Core JTBD` của tôi không nhét solution vào câu.
- [x] Tôi đã viết đủ 3 `job stories`.
- [x] Tôi đã điền `JTBD lite map` và khoanh ra 2 bước đau nhất.
- [x] Tôi đã chỉ ra `AI leverage point` thay vì nhảy thẳng vào feature list.
- [x] Tôi đã ghi rõ `assumptions to validate`.
- [ ] Tôi đã sửa version cuối sau khi share trong bàn. *(Bản này đang dùng phản biện mẫu; nếu đã share thật, thay bảng phản biện bằng ghi chú lớp.)*

---

## Nếu còn thời gian / làm về nhà

- Phỏng vấn nhanh 1 người dùng thật để kiểm xem `job story` nào là sát nhất.
- So sánh `current alternatives` với project của nhóm theo 3 tiêu chí: nhanh hơn, rẻ hơn, tin hơn.
- Tự hỏi lại một câu khó: **nếu không dùng AI, project này còn tạo giá trị không?**
- Nếu câu trả lời là "không", hãy xem lại liệu nhóm đang giải **job thật** hay chỉ đang tìm chỗ để nhét AI.
