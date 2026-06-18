---
artifact: 01 — Case Analysis
bai-tap: Lab 1 — Phân tích "tử huyệt" chiến lược
format: Cá nhân trước → share trong bàn → chốt verdict cuối
time: 20 phút trên lớp
nop-cuoi: Có — đây là file nộp cuối của Lab 1
---

# Lab 1 — Case Analysis / Phân tích "tử huyệt" chiến lược

**Case đã chọn:** Stack Overflow bị AI coding assistants làm suy yếu entry point hỏi đáp lập trình
**Người làm:** Bạn điền tên
**Bàn / nhóm bàn:** Bạn điền sau khi share thật
**Ngày:** 18/06/2026

> Đây là **file duy nhất** của Lab 1.  
> File này đồng thời đóng vai trò:
>
> - guide từng bước,
> - worksheet để điền trực tiếp,
> - và file nộp cuối cho người chấm.

Mục tiêu của bài này không phải kể lại "AI đã giết một công ty". Mục tiêu là chỉ ra, bằng bằng chứng thật:

1. **vì sao case đó bị tổn thương trước AI**
2. **điều gì đã thay đổi vĩnh viễn**
3. **và nếu rút một cảnh báo cho dự án của nhóm mình thì đó là gì**

Quy tắc xuyên suốt: **không có bằng chứng = không có nhận định.**

---

## Đầu ra bắt buộc

Người chấm cần thấy đủ 4 phần trong chính file này:

1. **3-5 bằng chứng chốt**
2. **4 nhận định bắt buộc**
3. **ghi chú sau khi share trong bàn**
4. **verdict cuối của cá nhân**

Nếu thiếu một trong bốn phần trên, bài sẽ bị xem là chưa hoàn chỉnh.

---

## Cách làm trong lớp (20 phút)

```text
2'  Chọn case
8'  Làm cá nhân: gom bằng chứng + viết 4 nhận định
7'  Share trong bàn: 90 giây / người + hỏi vặn lại
3'  Tự sửa verdict cá nhân sau thảo luận
```

---

## Bước 0 — Chọn case thật nhanh

Mặc định: **bạn tự chọn case của mình**.

### Một case phù hợp cần có 4 điều

- [x] Có một **AI shock** hoặc mốc đổi cục diện đủ rõ
- [x] Có thể tìm được ít nhất **3-5 bằng chứng công khai**
- [x] Có tác động đủ nhìn thấy được ở user / doanh thu / pricing / traffic / cổ phiếu / usage / vị thế cạnh tranh
- [x] Có thể trả lời câu hỏi: **"Điều gì đã thay đổi vĩnh viễn?"**

### Điền nhanh trước khi làm

- **Case / sản phẩm / công ty:** Stack Overflow / Stack Exchange public Q&A
- **AI / platform / sản phẩm mới tạo áp lực:** ChatGPT, GitHub Copilot, Gemini, Claude, Cursor và các AI coding assistants
- **Vì sao tôi chọn case này?**  
  > Đây là case rõ vì Stack Overflow từng là default entry point khi lập trình viên bí lỗi hoặc cần snippet. Sau ChatGPT, nhiều câu hỏi thường ngày được giải riêng trong AI chat/editor, làm lượng câu hỏi công khai giảm mạnh và buộc Stack Overflow đổi sang hướng trusted knowledge, data licensing và enterprise/agent products.

### Nếu bí case, chọn 1 trong 6 case gợi ý này

| Case | Vì sao đáng phân tích | Một tín hiệu đáng chú ý |
|---|---|---|
| Duolingo | AI có thể thay đổi cách học ngoại ngữ | chatbot/gia sư AI làm bài học cá nhân hóa hơn |
| Stack Overflow | hiệu ứng mạng bị đảo chiều | câu hỏi mới giảm mạnh sau ChatGPT |
| Jasper | lớp vỏ dễ bị generic AI ép | định giá và tăng trưởng chậm lại sau ChatGPT |
| Tome | AI phổ thông "đủ tốt" làm phân khúc cũ yếu đi | nhiều đợt cắt giảm và pivot |
| Inflection / Pi | chatbot tiêu dùng bị ông lớn lấn át | đội ngũ chuyển sang Microsoft |
| Figma / Claude Design | rủi ro "đất thuê" khi platform bước xuống app layer | cổ phiếu Figma phản ứng tiêu cực khi Claude Design ra mắt |

> Nếu có case riêng rõ hơn, dùng case riêng.

---

## Bước 1 — Gom 3-5 bằng chứng chốt

Không cần chép lại mọi số. Chỉ giữ những bằng chứng đủ mạnh để đỡ toàn bộ lập luận của bạn.

### Tìm bằng chứng theo 4 cụm

1. **Case trước AI**
   Sản phẩm là gì, user là ai, họ trả tiền cho cái gì, case từng thắng nhờ gì.

2. **AI shock**
   Mốc Big Tech AI / platform AI / sản phẩm mới xuất hiện và đổi luật chơi.

3. **Tác động quan sát được**
   User, doanh thu, ARR, pricing, traffic, usage, cổ phiếu, sa thải, pivot.

4. **Cục diện mới của thị trường**
   Ai phản ứng tốt hơn, ai thay thế tốt hơn, entry point mới nằm ở đâu, phân khúc còn sống không.

### Ưu tiên nguồn thế nào?

| Mức ưu tiên | Loại nguồn | Ví dụ |
|---|---|---|
| 1 | Nguồn gốc | báo cáo tài chính, investor relations, pricing page, blog chính thức |
| 2 | Báo uy tín | Reuters, CNBC, Bloomberg, FT, TechCrunch |
| 3 | Dữ liệu công khai / tổng hợp | MacroTrends, Similarweb, Stack Overflow Survey, Sacra |

### Bảng bằng chứng chốt

| # | Bằng chứng / số liệu chốt | Vì sao số này quan trọng? | Nguồn |
|---|---|---|---|
| E1 | Stack Overflow đang bán/licensing kho dữ liệu “17+ năm”, “83M+ questions and answers”, “69,000+ unique topics”, nhấn mạnh human-validated knowledge và moderation. | Đây là baseline trước cú sốc AI: moat của Stack Overflow là kho tri thức lập trình công khai, có vote, reputation, moderation và SEO mạnh. | [Stack Overflow Data Licensing](https://stackoverflow.co/data-licensing/) |
| E2 | Ngày 05/12/2022, Stack Overflow ban nội dung tạo bởi ChatGPT/generative AI vì câu trả lời nhìn có vẻ đúng nhưng sai nhiều, dễ sản xuất hàng loạt và làm quá tải hạ tầng kiểm duyệt tình nguyện. | Đây là mốc AI shock: AI không chỉ thay thế nhu cầu hỏi đáp bên ngoài mà còn làm nhiễu nguồn cung câu trả lời trong chính cộng đồng. | [Meta Stack Overflow policy](https://meta.stackoverflow.com/questions/421831/policy-generative-ai-e-g-chatgpt-is-banned) và [Stack Overflow Help Center](https://stackoverflow.com/help/gen-ai-policy) |
| E3 | Stack Exchange API cho thấy số câu hỏi Stack Overflow trong tháng 12 giảm từ 96.444 (12/2022) xuống 42.392 (12/2023), 17.955 (12/2024), rồi 4.228 (12/2025). Riêng 12/2024 → 12/2025 giảm khoảng 76,5%. | Đây là bằng chứng hành vi người dùng đổi rõ: developer vẫn cần giải quyết vấn đề, nhưng ít tạo câu hỏi công khai hơn vì nhiều câu hỏi được xử lý riêng bằng AI/chat/editor. | [API 12/2022](https://api.stackexchange.com/2.3/questions?fromdate=1669852800&todate=1672531199&order=desc&sort=creation&site=stackoverflow&pagesize=1&filter=total), [API 12/2025](https://api.stackexchange.com/2.3/questions?fromdate=1764547200&todate=1767225599&order=desc&sort=creation&site=stackoverflow&pagesize=1&filter=total) |
| E4 | Một nghiên cứu difference-in-differences về Stack Overflow ước tính ChatGPT làm weekly posts giảm 16%; hiệu ứng tăng theo thời gian và mạnh hơn ở các ngôn ngữ lập trình phổ biến. | Bằng chứng này đỡ lập luận nhân quả: giảm activity không chỉ là mùa vụ hay văn hóa cộng đồng, mà gắn với việc LLM trở thành substitute cho hỏi đáp công khai. | [“Are Large Language Models a Threat to Digital Public Goods?”, arXiv](https://arxiv.org/abs/2307.07367) |
| E5 | Stack Overflow Developer Survey 2025: 84% respondent đang dùng hoặc dự định dùng AI tools trong development; 51% professional developers dùng AI hằng ngày. Đồng thời 46% distrust accuracy của AI tools, cao hơn nhóm trust 33%. | Cục diện mới rất nghịch lý: developer dùng AI nhiều dù không hoàn toàn tin, nên Stack Overflow còn giá trị ở trust/verification nhưng mất vị trí “điểm hỏi đầu tiên”. | [Stack Overflow Developer Survey 2025 - AI](https://survey.stackoverflow.co/2025/ai) |

### 3 phát hiện ban đầu

Trước khi viết nhận định, ghi nhanh 3 dòng:

1. **Case này từng thắng nhờ...**  
   > thói quen của developer: gặp lỗi, copy error message lên Google, click Stack Overflow, đọc accepted answer/vote/comment rồi áp dụng.
2. **AI shock làm thay đổi...**  
   > điểm bắt đầu của workflow debugging/learning: từ hỏi cộng đồng công khai sang hỏi AI riêng trong chat hoặc ngay trong IDE.
3. **Dấu hiệu mạnh nhất cho thấy luật chơi mới là...**  
   > lượng câu hỏi tháng 12 giảm từ 96.444 năm 2022 xuống 4.228 năm 2025, trong khi khảo sát 2025 cho thấy AI tools đã thành hành vi mainstream của developer.

---

## Bước 2 — Viết 4 nhận định bắt buộc

### Nhận định 1 — Trước AI, case này thắng nhờ giả định gì?

Gợi ý:

- Người dùng thuê sản phẩm này để làm gì?
- Giá trị lõi trước AI là gì?
- Họ thắng nhờ workflow, switching cost, brand, distribution, data hay một giả định hành vi nào?
- Job-to-be-done (công việc người dùng "thuê" sản phẩm làm hộ) là gì?

**Trả lời của tôi:**  
> Trước AI, Stack Overflow thắng nhờ giả định rằng developer sẽ giải quyết vấn đề lập trình bằng cách đưa câu hỏi ra không gian công khai: Google/search dẫn vào một thread, cộng đồng trả lời, vote và chỉnh sửa để câu trả lời tốt nhất nổi lên. Giá trị lõi là tri thức có dấu vết xã hội: accepted answer, vote, comment, reputation và lịch sử sửa đổi.
> JTBD của developer là: “Khi tôi gặp lỗi hoặc chưa biết dùng API/framework thế nào, hãy giúp tôi tìm được lời giải đáng tin đủ nhanh để tiếp tục build.” Stack Overflow thắng vì biến hàng triệu lần bí lỗi riêng lẻ thành kho tri thức chung cho người sau.

**Bằng chứng đỡ nhận định này:** E1, E3

---

### Nhận định 2 — Kỳ vọng người dùng và luật chơi cạnh tranh đã đổi ở đâu?

#### Nhắc nhanh 7 Dịch chuyển Kỳ vọng

1. Làm xong giúp tôi
2. May đo cho tôi
3. Tự lo việc lặt vặt
4. Trả theo kết quả
5. Phản hồi ngay
6. Giao diện tự thay đổi
7. Thấu hiểu ngữ cảnh

#### Nhắc nhanh 5 Competitive Dynamics

- switching costs giảm
- data advantages tăng
- platform risk
- build-copy cycles tăng tốc
- GTM + distribution quan trọng hơn

**Shift kỳ vọng quan trọng nhất:** Phản hồi ngay + thấu hiểu ngữ cảnh + làm xong giúp tôi
**Competitive dynamic quan trọng nhất:** switching costs giảm + data advantages tăng + platform risk

**Trả lời của tôi:**  
> Kỳ vọng của developer chuyển từ “tôi tìm thread giống lỗi của mình” sang “AI đọc đúng context repo/log/code của tôi và đưa hướng sửa ngay”. AI chat/editor không cần chờ cộng đồng, không bắt user viết câu hỏi đúng chuẩn, và có thể tiếp tục hội thoại để debug.
> Luật chơi cạnh tranh đổi vì Stack Overflow không chỉ cạnh tranh với forum khác, mà với Copilot/Cursor/ChatGPT/Gemini ngay trong workflow code. Data của Stack Overflow vẫn có giá trị lớn, nhưng chính giá trị đó cũng nuôi các AI systems đang chiếm entry point của user.

**Bằng chứng đỡ nhận định này:** E2, E4, E5

---

### Nhận định 3 — Giả định nào không còn đúng nữa? Điều gì đã thay đổi vĩnh viễn?

Gợi ý:

- Switching cost cũ có từng giữ user ở lại không? Vì sao giờ không còn đủ?
- Entry point cũ của sản phẩm có còn tồn tại không, hay người dùng đã chuyển sang một điểm bắt đầu mới?
- Workflow cũ có còn được chấp nhận không, hay chuẩn mới là "làm xong giúp tôi / ngay trong nơi tôi đang làm việc"?
- "Thay đổi vĩnh viễn" không phải là giá cổ phiếu giảm; nó là **chuẩn mới trong đầu người dùng** hoặc **luật chơi mới của thị trường**.
- Phân khúc này còn tồn tại không? Nếu còn, nó đang được phục vụ theo cách khác ra sao?

**Điều đã thay đổi vĩnh viễn theo tôi là:**  
> Thay đổi vĩnh viễn là câu hỏi thường ngày của developer không nhất thiết đi ra web công khai nữa. Trước đây mỗi lỗi lặp lại có thể sinh ra một thread, được chỉnh và tích lũy thành public knowledge. Bây giờ nhiều lỗi được giải trong private AI session, không để lại artifact công khai cho cộng đồng hoặc search engine.
> Vì vậy network effect cũ bị đảo chiều: càng nhiều người hỏi AI riêng, càng ít câu hỏi mới lên Stack Overflow; càng ít câu hỏi mới, kho tri thức công khai cập nhật chậm hơn; khi kho công khai chậm hơn, developer lại càng có lý do hỏi AI trước.

**Bằng chứng đỡ nhận định này:** E3, E4, E5

---

### Nhận định 4 — Case này còn cứu được không? Nếu có, phải đổi bằng cách nào?

Gợi ý:

- Nếu cứu được: họ phải đổi ở moat nào, workflow nào, distribution nào?
- Nếu không cứu được: vì sao đã quá muộn?
- So với một đối thủ phản ứng tốt hơn, họ chậm ở đâu?

**Verdict ban đầu của tôi:** Có nhưng phải đổi rất mạnh

**Trả lời của tôi:**  
> Stack Overflow còn cứu được, nhưng không thể quay lại hoàn toàn mô hình “public Q&A + SEO traffic” như trước. Họ phải đổi moat từ nơi có câu trả lời sang nơi xác thực câu trả lời: verified knowledge, attribution, reputation, cập nhật độ đúng, và enterprise/private knowledge graph cho người + agent.
> Hướng Stack Internal, Data Licensing và Stack Overflow for Agents là hợp lý hơn việc chỉ cố kéo user quay về hỏi public question. Tuy nhiên rủi ro là cộng đồng công khai teo lại; nếu không giữ được động lực đóng góp của human experts, phần trust mà Stack Overflow bán cũng sẽ yếu dần.

**Bằng chứng đỡ nhận định này:** E1, E3, E5

---

## Tóm tắt cá nhân trước khi share trong bàn

Viết đúng 3 câu:

1. `Case này yếu đi vì...`
2. `Điều thay đổi vĩnh viễn là...`
3. `Verdict của tôi là...`

**Bản tóm tắt 3 câu của tôi:**  
1. Case này yếu đi vì AI coding assistants chiếm entry point “tìm câu trả lời khi bí code”, khiến ít câu hỏi được đưa lên public Q&A hơn.
2. Điều thay đổi vĩnh viễn là nhiều tri thức lập trình mới được tạo trong private AI sessions thay vì tích lũy thành thread công khai có vote, comment và revision.
3. Verdict của tôi là Stack Overflow còn sống được nếu chuyển thành lớp trusted knowledge/verification cho người, đội ngũ và agent, nhưng phải bảo vệ được động lực đóng góp của cộng đồng.

---

## Bước 3 — Share trong bàn (7')

### Mỗi người chỉ nói 4 thứ trong 90 giây

1. **Case bạn chọn là gì**
2. **Bằng chứng mạnh nhất bạn có là gì**
3. **Điều gì đã thay đổi vĩnh viễn**
4. **Verdict của bạn**

### Nếu chưa biết hỏi ngược gì, dùng 4 câu này

1. **"Bằng chứng mạnh nhất cho nhận định đó là gì?"**
2. **"Điều gì ở đây là triệu chứng, còn điều gì là thay đổi vĩnh viễn?"**
3. **"Nếu switching cost từng cao, vì sao người dùng vẫn rời đi?"**
4. **"Platform mới hoặc đối thủ mới đã chiếm entry point ở đâu?"**

### Ghi nhanh khi nghe các bạn cùng bàn

> Lưu ý: bảng dưới là ghi chú mẫu để luyện cách viết. Nếu đã share thật trong bàn, thay 4 dòng này bằng ghi chú thực tế.

| Người | Case | Bằng chứng mạnh nhất họ nêu | Điều họ cho là "thay đổi vĩnh viễn" | Verdict của họ |
|---|---|---|---|---|
| Bạn 1 | Stack Overflow | Câu hỏi mới giảm sau ChatGPT | Entry point hỏi đáp kỹ thuật chuyển sang AI coding assistant/chat | Còn sống nếu tập trung trust, community và canonical answers |
| Bạn 2 | Jasper | Generic LLM làm copywriting cơ bản rẻ đi | Wrapper mỏng mất pricing power khi AI nền tảng đủ tốt | Phải vertical hóa workflow marketing |
| Bạn 3 | Tome | AI presentation trở thành tính năng phổ thông | “Tạo deck bằng AI” không còn là phân khúc riêng đủ mạnh | Cần pivot vào workflow cụ thể hơn |
| Bạn 4 | Inflection / Pi | Đội ngũ chủ chốt chuyển sang Microsoft | Consumer chatbot độc lập bị Big Tech phân phối tốt hơn lấn át | Khó cứu nếu không có distribution riêng |

### Sau khi cả bàn share xong, chốt 3 ý chung

**1. Bàn tôi thấy case nào có bằng chứng mạnh nhất? Vì sao?**  
> Bản nháp mẫu: Stack Overflow có bằng chứng mạnh nhất vì có số liệu câu hỏi trực tiếp từ Stack Exchange API, policy chính thức về AI-generated content và survey chính thức cho thấy developer đã dùng AI rất rộng.

**2. Có pattern nào lặp lại giữa nhiều case không?**  
Ví dụ: switching costs giảm, platform bước xuống app layer, user chuyển sang "làm xong giúp tôi", moat cũ quá mỏng…  
> Pattern lặp lại là AI không chỉ tạo feature mới mà chiếm luôn entry point của workflow. Switching cost giảm mạnh, user kỳ vọng “phản hồi ngay trong context của tôi”, và moat dạng content/SEO/community yếu đi nếu không chuyển thành trust layer hoặc workflow layer.

**3. Một cảnh báo cho chính dự án của nhóm tôi là gì?**  
> Nếu dự án của nhóm phụ thuộc vào việc user phải rời workflow hiện tại để hỏi/tra cứu, AI assistant hoặc platform lớn có thể chiếm entry point đó. Nhóm cần xây nơi có dữ liệu/ngữ cảnh riêng, trust signal rõ và lý do để human experts tiếp tục đóng góp.

---

## Bước 4 — Chốt lại verdict cá nhân sau thảo luận (3')

### Sau khi nghe bàn phản biện, verdict của tôi:

- [ ] Giữ nguyên
- [x] Đổi nhẹ
- [ ] Đổi mạnh

### Vì sao tôi giữ / đổi verdict?

> Sau khi tự phản biện theo các pattern ở phần share mẫu, tôi đổi nhẹ verdict: ban đầu tôi nghĩ Stack Overflow chỉ cần thêm AI search/chat là đủ; sau đó thấy vấn đề lõi là incentive của public knowledge. Nếu câu hỏi không còn được đưa ra công khai, nguồn tri thức mới sẽ chậm lại.
> Vì vậy hướng cứu không chỉ là làm AI feature, mà phải thiết kế lại cơ chế tạo, xác thực, cập nhật và phân phối tri thức cho cả người lẫn agent.

### Verdict cuối cùng của tôi (phiên bản nộp)

**Case này tổn thương trước AI vì:**  
> Stack Overflow phụ thuộc vào workflow developer hỏi/tìm câu trả lời công khai, trong khi AI coding assistants trả lời ngay trong chat hoặc IDE với context cá nhân, làm giảm nhu cầu tạo câu hỏi public.

**Điều thay đổi vĩnh viễn là:**  
> Entry point giải quyết lỗi lập trình chuyển từ “search và đọc thread” sang “hỏi AI trong workflow”; public Q&A không còn tự nhiên tích lũy câu hỏi thường ngày như trước.

**Nếu phải rút 1 bài học cho dự án của nhóm mình, tôi rút ra:**  
> Đừng chỉ xây kho câu trả lời; hãy xây cơ chế tạo trust, cập nhật tri thức và gắn vào workflow nơi người dùng đang làm việc, vì AI nền tảng có thể lấy mất điểm hỏi đầu tiên rất nhanh.

---

## Checklist trước khi nộp

- [x] Tôi đã chọn ít nhất 3 bằng chứng chốt có nguồn.
- [x] Mỗi nhận định đều chỉ vào ít nhất 1 bằng chứng.
- [ ] Tôi đã ghi lại phần share trong bàn thật. *(Bản nháp này đang dùng ghi chú mẫu, cần thay bằng ghi chú lớp nếu có.)*
- [x] Tôi đã viết verdict cuối sau thảo luận / tự phản biện mẫu.

---

## Nếu còn thời gian / làm về nhà

- Bổ sung thêm một case "đối thủ phản ứng tốt hơn" để so.
- Thêm một đoạn ngắn: **nếu tôi là PM của case này trong 6 tháng đầu sau AI shock, tôi sẽ làm gì đầu tiên?**
- Kiểm lại xem case này yếu vì expectation shift, competitive dynamics, hay cả hai cùng lúc.
