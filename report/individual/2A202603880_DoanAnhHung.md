# Báo cáo cá nhân — 2A202603880_DoanAnhHung

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đoàn Anh Hùng
- MSSV: 2A202603880
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: HungTungTruyenHuy
- Link repo nhóm: https://github.com/huydn8816/K5-L3B-Day02-HungTungTruyenHuy-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi cần ôn tập khối lượng lớn kiến thức lý thuyết từ các bài giảng dài (50–100 trang slide) vào những khoảng thời gian di chuyển hoặc nghỉ giải lao, tôi muốn tiếp thu được các khái niệm cốt lõi theo dạng tóm tắt cô đọng, để ghi nhớ được hệ thống kiến thức mà không bị mỏi mắt hay quá tải thông tin. | Cá nhân tôi và các bạn học trong lớp. | Mất 3–4 tiếng đọc lướt qua hàng trăm slide trước mỗi buổi học nhưng chỉ nhớ được dưới 30%; tồn đọng 2–3 bài giảng chưa kịp đọc. |
| 2 | Tốn thời gian | Khi bắt đầu một bài tập lớn/sprint mới cùng 3–4 thành viên, tôi muốn phân rã yêu cầu thành các đầu việc độc lập kèm quy ước bàn giao rõ ràng, để cả nhóm chủ động thực hiện song song mà không bị chồng chéo hay đùn đẩy trách nhiệm. | Tôi và các thành viên trong nhóm. | Mất 60–90 phút mỗi buổi đầu sprint để tranh luận phân công; 1–2 thành viên hay bị nghẽn (block) do chờ đầu việc của nhau. |
| 3 | Lặp lại | Khi chạy thử mã nguồn hoặc notebook của thành viên khác trên máy tính của mình, tôi muốn tái lập chính xác môi trường thực thi và các gói thư viện tương thích, để chạy được chương trình ngay mà không phải mất hàng giờ tra cứu lỗi xung đột phiên bản. | Cả nhóm (đặc biệt khi khác OS Windows/Mac). | Mất 45–60 phút mỗi lần kéo repo mới chỉ để fix lỗi `ModuleNotFoundError`, xung đột Python/CUDA; thường xuyên bị tình trạng "chạy máy tôi được nhưng máy bạn lỗi". |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi nhận đề bài lab gồm nhiều file tài liệu (README, RULES, RUBRIC, CHECKPOINTS), tôi muốn tổng hợp nhanh danh sách tiêu chí bắt buộc và các mốc deadline, để không bỏ sót yêu cầu kỹ thuật dẫn đến bị trừ điểm oan. | Cả nhóm. | Mất 30–45 phút đọc lướt 5 file markdown; từng có lần quên quy tắc đặt tên repo hoặc file làm mất điểm. |
| 5 | Pain từ người khác | Khi 4 thành viên cùng commit nội dung vào các file chung (`group_report.md`, `TEAM.md`), tôi muốn phát hiện và xử lý sớm các xung đột (conflict) nội dung, để không làm ghi đè hay mất phần viết của bạn khác. | Cả nhóm. | Ít nhất 1 lần/tuần gặp conflict git khi nộp bài; mất 20–30 phút giải quyết và có nguy cơ mất đoạn văn của đồng đội. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- **Ý giữ lại:** Ý về "Đồng bộ môi trường và dependencies giữa các máy" (Vấn đề 3) và "Phân rã công việc nhóm" (Vấn đề 2). Lý do giữ lại: Đây là các rào cản kỹ thuật và điều phối có thật, xảy ra liên tục trong các buổi thực hành nhóm.
- **Ý loại bỏ:** Ý ban đầu định đưa vào là "Muốn tạo audio tóm tắt bài giảng" và "Chatbot kiểm tra bài nộp". Đã chủ động loại bỏ vì đây là các giải pháp trá hình (solution-first), vi phạm nguyên tắc "Problem first, not AI first" của môn học. Đã sửa lại thành mô tả nỗi đau quá tải thông tin và nhu cầu ôn tập linh hoạt.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Ôn tập kiến thức bài giảng dài trong thời gian rảnh / di chuyển (Vấn đề 1) | Nhu cầu cấp thiết hàng tuần, khối lượng tài liệu lớn, tốn nhiều thời gian đọc slide; có tiềm năng ứng dụng cao và phù hợp để xây dựng quy trình rõ ràng. | Làm sao đảm bảo nội dung tóm tắt/audio không bỏ sót công thức toán học hoặc sơ đồ kỹ thuật trực quan. |
| 2 | Phân rã công việc và thiết lập workflow cho nhóm (Vấn đề 2) | Nỗi đau điều phối lặp lại ở mọi bài lab, ảnh hưởng trực tiếp đến hiệu suất và tâm lý làm việc của cả 4 người. | Mỗi bài lab có tính chất kỹ thuật khác nhau, khó tạo một khung chia việc cố định cho mọi tình huống. |
| 3 | Đồng bộ môi trường và dependencies giữa các máy (Vấn đề 3) | Lãng phí nhiều thời gian thiết lập thay vì tập trung vào logic bài lab; gây ức chế khi làm việc nhóm đa nền tảng. | Sự khác biệt phần cứng (chip Apple Silicon M-series vs Intel x86, GPU rời NVIDIA) rất khó giải quyết nếu không dùng môi trường ảo hóa sâu. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần ôn tập khối lượng lớn kiến thức lý thuyết từ các bài giảng dài (50–100 trang slide) vào những khoảng thời gian di chuyển hoặc nghỉ giải lao, tôi muốn tiếp thu được các khái niệm cốt lõi theo dạng tóm tắt cô đọng, để ghi nhớ được hệ thống kiến thức mà không bị mỏi mắt hay quá tải thông tin. |
| Actor | Sinh viên, học viên các khóa học kỹ thuật chuyên sâu (VinUni, AI thực chiến). |
| Thời điểm / bối cảnh | 1–2 ngày trước buổi lab thực hành, trước kỳ thi, hoặc trong lúc di chuyển xe buýt/đi bộ và giờ nghỉ giải lao 15–30 phút. |
| Quy trình hiện tại (3–7 bước) | 1. Tải slide bài giảng từ LMS (PDF, 60–100 trang): 5'<br>2. Mở máy tính, đọc lướt qua toàn bộ slide để nắm mục lục: 30'<br>3. Đọc chi tiết từng slide, tra cứu các khái niệm mới: 90'<br>4. Ghi chép / tóm tắt thủ công ra sổ tay hoặc Notion: 45' [BOTTLENECK]<br>5. Đọc lại bản tóm tắt trước giờ thi/lab: 20' |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: Ghi chép / tóm tắt thủ công ra sổ tay hoặc Notion (45 phút/lần). Đòi hỏi phải vừa đọc vừa chắt lọc từ văn bản dài, rất tốn sức và thường bị bỏ dở khi thiếu thời gian. |
| Impact (nếu không giải thì sao) | Bỏ sót 50–70% kiến thức nền tảng; vào buổi thực hành không hiểu bản chất thuật toán, làm bài theo dạng sao chép máy móc; giảm kết quả đánh giá môn học. |
| Success metric (baseline → target) | Baseline: Mất 190 phút để đọc và tóm tắt 1 bài giảng 80 trang; tỷ lệ nhớ kiến thức sau 3 ngày dưới 30% (tự đánh giá qua quiz đầu giờ).<br>Target: Giảm thời gian hấp thụ kiến thức cốt lõi xuống dưới 45 phút/bài giảng; tỷ lệ làm đúng bài quiz kiểm tra khái niệm đầu giờ đạt $\ge 80\%$.<br>Cách đo: Bấm giờ thực tế trong 3 buổi học tiếp theo và đo điểm số bài quiz đầu giờ. |
| Phương án không dùng AI | In slide ra giấy dạng 4 slide/trang để gạch chân nhanh; lập nhóm học tập chia nhau mỗi người tóm tắt 1 chương; dùng sơ đồ tư duy (mindmap) mẫu có sẵn. |
| Giả thuyết về AI (nếu có) | Trích xuất nội dung slide $\to$ LLM chuyển hóa thành bài giảng độc thoại sư phạm cô đọng (1 giọng đọc chuẩn), giải thích trực giác bản chất khái niệm; đối với các phần lý thuyết/toán phức tạp không thể tóm tắt hết, AI tóm lược tổng quan và chèn các câu hỏi gợi mở đào sâu (inquiry anchors) $\to$ Xuất file audio 10–12 phút kèm Cheat Sheet 1 trang định vị đúng sơ đồ, công thức và tài liệu tự tra cứu. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 190 phút/bài giảng

[Tải slide LMS: 5'] 
→ [Đọc lướt mục lục: 30'] 
→ [Đọc chi tiết từng slide: 90'] 
→ [Tóm tắt thủ công ra Notion: 45'] ← BOTTLENECK
→ [Đọc lại ôn tập: 20']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi bắt đầu một bài tập lớn/sprint mới cùng 3–4 thành viên, tôi muốn phân rã yêu cầu thành các đầu việc độc lập kèm quy ước bàn giao rõ ràng, để cả nhóm chủ động thực hiện song song mà không bị chồng chéo hay đùn đẩy trách nhiệm. |
| Actor | Trưởng nhóm hoặc thành viên điều phối dự án học tập. |
| Thời điểm / bối cảnh | Ngày đầu tiên nhận đề bài lab mới hoặc bắt đầu đồ án môn học. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc lướt đề bài và tài liệu hướng dẫn: 20'<br>2. Họp nhóm online thảo luận cách làm: 40'<br>3. Liệt kê các đầu việc ra giấy/tin nhắn chat: 30'<br>4. Tranh luận phân chia ai làm phần nào và mốc bàn giao: 45' [BOTTLENECK]<br>5. Tạo task trên Trello/Notion: 15' |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: Tranh luận phân chia công việc và xác định chuẩn bàn giao (45 phút/lần). Dễ phát sinh mâu thuẫn hoặc đùn đẩy phần việc khó. |
| Impact (nếu không giải thì sao) | Các thành viên bị nghẽn (block) việc lẫn nhau; tiến độ bị đình trệ; dồn toàn bộ áp lực hoàn thiện vào 2 tiếng trước hạn chót. |
| Success metric (baseline → target) | Baseline: Mất 150 phút cho phiên phân rã công việc; phát sinh 2 lần trễ mốc bàn giao chéo giữa các thành viên.<br>Target: Giảm thời gian phân chia xuống dưới 40 phút; 0 trường hợp bị chồng chéo hoặc nghẽn task quá 24h.<br>Cách đo: Bấm giờ cuộc họp phân công và theo dõi nhật ký hoàn thành task trên bảng Kanban. |
| Phương án không dùng AI | Sử dụng bảng ma trận RACI cố định; áp dụng template phân rã task chuẩn hóa cho từng dạng bài tập lớn. |
| Giả thuyết về AI (nếu có) | Đưa đề bài vào LLM để gợi ý phân rã cấu trúc công việc (WBS) thành các task nhỏ độc lập kèm tiêu chí nghiệm thu (Definition of Done). |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 150 phút/sprint

[Đọc lướt đề bài: 20'] 
→ [Họp thảo luận cách làm: 40'] 
→ [Liệt kê task thô: 30'] 
→ [Tranh luận chia việc & quy ước bàn giao: 45'] ← BOTTLENECK
→ [Ghi vào Trello/Notion: 15']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi chạy thử mã nguồn hoặc notebook của thành viên khác trên máy tính của mình, tôi muốn tái lập chính xác môi trường thực thi và các gói thư viện tương thích, để chạy được chương trình ngay mà không phải mất hàng giờ tra cứu lỗi xung đột phiên bản. |
| Actor | Lập trình viên / thành viên nhóm phụ trách chạy thử và tích hợp code. |
| Thời điểm / bối cảnh | Mỗi khi kéo mã nguồn mới từ Git về máy cá nhân (khác biệt môi trường Windows, macOS, Ubuntu). |
| Quy trình hiện tại (3–7 bước) | 1. Git pull code mới về máy: 2'<br>2. Mở file chạy thử và gặp lỗi thiếu thư viện/phiên bản: 5'<br>3. Tra cứu file requirements hoặc nhắn tin hỏi người viết code: 15'<br>4. Dò tìm, gỡ bỏ và cài đặt các phiên bản thư viện tương thích: 45' [BOTTLENECK]<br>5. Chạy lại kiểm thử mã nguồn: 10' |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4: Dò tìm và cài đặt các phiên bản package/driver tương thích (45 phút/lần), thường xuyên rơi vào tình trạng "dependency hell". |
| Impact (nếu không giải thì sao) | Lãng phí thời gian của cả người chạy và người viết code; giảm tinh thần hợp tác; chậm tiến độ bàn giao sản phẩm chung. |
| Success metric (baseline → target) | Baseline: Mất trung bình 60–75 phút mỗi lần cấu hình môi trường mới; tỷ lệ vấp lỗi khi chạy lần đầu lên đến 75%.<br>Target: Tái lập môi trường thành công trong dưới 10 phút; giảm tỷ lệ lỗi chạy lần đầu xuống dưới 10%.<br>Cách đo: Bấm giờ từ lúc git pull đến khi test script chạy trả về mã thoát 0. |
| Phương án không dùng AI | Bắt buộc sử dụng Dev Containers / Dockerfile hoặc xuất cấu hình môi trường chuẩn (`conda env export --no-builds`) ngay từ commit đầu tiên. |
| Giả thuyết về AI (nếu có) | Phân tích AST của code để nhận diện chính xác các import thực tế và tự động sinh tệp cấu hình môi trường tối giản. |
| Cảm nhận nhanh | Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 77 phút/lần đồng bộ

[Git pull code mới: 2'] 
→ [Chạy thử & vấp lỗi: 5'] 
→ [Nhắn tin hỏi người viết code: 15'] 
→ [Dò tìm & cài đặt thư viện/CUDA: 45'] ← BOTTLENECK
→ [Chạy kiểm thử lại: 10']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Nhu cầu học tập và ôn tập diễn ra liên tục hàng tuần; khối lượng bài giảng đồ sộ gây áp lực thực sự lên học viên; bài toán có đầu vào (slide PDF) và đầu ra (bài giảng audio cô đọng + cheat sheet) rất rõ ràng, hoàn toàn khả thi để xây dựng một quy trình tự động hóa có kiểm soát.
- Câu hỏi muốn nhóm phản biện: Liệu hình thức một người giảng bài kèm các câu hỏi gợi mở đào sâu có đủ giữ được sự chú ý của người nghe khi đang di chuyển không, và làm sao đảm bảo các câu hỏi mở rộng thực sự kích thích người học tự tra cứu thay vì bị bỏ quên sau khi tắt audio?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| **Audio bất lực trước công thức toán và sơ đồ kỹ thuật:** Slide bài giảng AI/kỹ thuật chứa nhiều công thức vi phân, ma trận và kiến trúc mạng. Nghe audio không thể hình dung được toán và code, nghe xong vẫn không làm được bài lab. | Đồng ý hoàn toàn | Không cố ép AI diễn giải công thức toán qua âm thanh. Chỉ dùng audio để giải thích trực giác bản chất (intuition) và bức tranh tổng thể; phần toán và sơ đồ phức tạp được tóm lược tổng quan kèm câu hỏi gợi mở đào sâu (inquiry anchors), đồng thời sinh file **Cheat Sheet 1 trang** định vị sẵn công thức/sơ đồ để học viên mở ra xem khi ngồi vào bàn học. |
| **Gợi ý làm Podcast 2 người gây loãng kiến thức:** AI ban đầu đề xuất kịch bản podcast 2 người thảo luận để bớt chán, nhưng hình thức này nhiều câu thoại xã giao rườm rà, làm giảm mật độ thông tin học thuật nghiêm túc. | Đồng ý | Bác bỏ gợi ý podcast 2 người; chốt chuyển sang mô hình **1 người giảng bài cô đọng (độc thoại sư phạm)**. Cắt bỏ 100% lời chào hỏi xã giao, đi thẳng vào bản chất khái niệm và khống chế thời lượng nghiêm ngặt dưới 12 phút để tránh mỏi tai. |
| **Success Metric đặt mục tiêu "nhớ $\ge 80\%$" không đo được:** Không thể đo lường trí nhớ dài hạn khách quan trong quy mô một buổi lab hoặc vài ngày ngắn ngủi. | Đồng ý | Chuẩn hóa lại phương pháp đo lường thực tế: Đo bằng **bộ mini-quiz 5 câu hỏi trắc nghiệm** kiểm tra trực giác khái niệm ngay trước giờ vào lớp (đo được định lượng ngay lập tức, không dựa vào cảm tính). |
| **Người nghe sẽ quên ngay câu hỏi mở rộng khi tắt audio:** Đang di chuyển hoặc đi bộ mà nghe câu hỏi mở rộng thì sẽ trôi tuột đi, không ai tự giác tìm hiểu thêm. | Đồng ý | Ghép nối trực tiếp câu hỏi mở rộng với bài lab thực hành: *"Câu hỏi này liên quan trực tiếp đến Task X trong buổi lab, hãy xem gợi ý giải tại Mục 2 trên Cheat Sheet"*, tạo động lực bắt buộc phải mở ra xem khi làm bài. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày bản pitch Problem Card #1 trong 90 giây: Bài toán quá tải kiến thức khi đọc bài giảng 80 slide, đề xuất giải pháp 1 người giảng bài cô đọng kết hợp câu hỏi gợi mở đào sâu và Cheat Sheet 1 trang. | Nhóm nắm được bản chất nỗi đau học tập và đưa vào danh sách rút gọn để cân nhắc ở bước gom cụm. |
| Phản biện bài của bạn khác | **Câu hỏi tôi đã đặt cho Huy (đề tài Agent Vingroup):** *"Nếu Agent tự động thực hiện nhiều bước xuyên app, làm sao kiểm soát rủi ro AI tự ý trừ tiền đặt xe khi người dùng chưa đồng ý, hoặc lỡ AI hiểu nhầm lệnh giọng nói mà mở khóa cửa thông minh (Smart Lock) gây mất an toàn nhà ở?"*<br>**Câu hỏi tôi đã đặt cho Tùng (đề tài lọc JD/CV):** *"Mỗi công ty viết JD một kiểu và yêu cầu kỹ năng quá rộng, làm sao chuẩn hóa tiêu chí để biết kỹ năng nào là bắt buộc (Must-have) và kỹ năng nào chỉ là điểm cộng (Nice-to-have)?"*<br>**Câu hỏi tôi đã đặt cho Truyền (đề tài xử lý hóa đơn lệch #8):** *"Nếu nhà cung cấp giao hàng làm nhiều đợt và hóa đơn lệch theo từng đợt giao thì hệ thống phân biệt ngoại lệ này thế nào để không giữ lại nhầm hóa đơn hợp lệ?"* | Huy đã tiếp thu và bổ sung bước Financial Gate (bắt buộc người dùng xác nhận tiền mới gọi xe) cùng rào chắn an toàn (Boundary loại trừ Smart Lock); Tùng đã bổ sung phân loại kỹ năng cốt lõi và bổ trợ; Truyền đã bổ sung quy tắc đối chiếu ba bên có dung sai và kiểm tra giao từng phần vào phương án Rule. |
| Nhận phản biện | **Câu hỏi tôi nhận được từ nhóm:** *"Slide bài giảng AI có nhiều công thức toán và sơ đồ mạng phức tạp, nếu chỉ nghe audio thì làm sao người học nắm được chi tiết kỹ thuật để làm bài lab?"*<br>**Tôi đã sửa gì:** Tôi làm rõ giới hạn của âm thanh và bổ sung cơ chế ghép đôi: Audio chỉ giải thích trực giác bản chất, phần toán và sơ đồ phức tạp được tóm lược tổng quan kèm câu hỏi gợi mở, đồng thời đính kèm "Cheat Sheet 1 trang" chứa sơ đồ và công thức để học viên mở ra xem khi ngồi vào bàn học. | Bảo vệ được tính khả thi của Problem Card #1 và giúp nhóm hiểu rõ ranh giới khi ứng dụng AI vào học tập kỹ thuật. |
| Gom cluster / cây OST | Thảo luận và chỉ ra điểm tương đồng giữa bài của tôi (đọc slide dài) và bài của Tùng (đọc paper ngoại ngữ dài) để gom thành cụm *"Quá tải thông tin khi đọc tài liệu học tập dài trước buổi học"*; cùng nhóm gạch bỏ các giải pháp trá hình trong cây OST. | Giúp nhóm phân định rạch ròi giữa Nỗi đau (Opportunity) và Giải pháp (Solution) trong cây OST. |
| Chọn candidate problem | Tham gia chấm điểm 3 candidate theo 7 tiêu chí trong bảng 2.4; đồng thuận chọn đề tài Agent Vingroup của Huy vì có hệ sinh thái đa dịch vụ rộng lớn và tính thực tế cao; nhận trách nhiệm phụ trách chính CP5. | Nhóm thống nhất 100% về bài toán chung mà không có bất đồng kéo dài; phân công công việc rõ ràng. |
| Kiểm chứng / research | Cung cấp góc nhìn về trải nghiệm cư dân và sinh viên khi di chuyển trong khuôn viên lớn; hỗ trợ rà soát đối thủ (Google Assistant, Apple Shortcuts) để chỉ ra khoảng trống về dữ liệu nội khu. | Củng cố luận điểm cho bảng Research ở Mục 3.3. |
| Quy trình nhóm | Thiết kế toàn bộ sơ đồ quy trình Hiện tại (6 bước) & Tương lai (Mục 4), phân định các tầng Rule (API WinMart, BQL), AI (bóc tách ý định) và HITL (Financial Gate); tích hợp 2 vòng lặp phản hồi (làm rõ ASR và đổi ý lộ trình). | Hoàn thiện Mục 4 trong `group_report.md` với sơ đồ Mermaid `flowchart LR` chuẩn xác. Tôi chủ động thiết kế kịch bản mở rộng (WinMart + né công trường VinUni) ở CP5 để chứng minh sự vượt trội của Agent so với phím tắt cố định (Rule); sau đó cùng nhóm thống nhất giữ kịch bản 2 việc cơ bản ở CP6 làm luồng thử nghiệm tối thiểu (MVP) để kiểm soát rủi ro. |
| Problem Statement | Soạn thảo Problem Statement v0 gồm 6 trường chuẩn (Mục 5), xác định Success Metric đo lường qua 10 chuyến xe thử nghiệm nội khu; thiết lập 3 boundary an toàn và bảo vệ phản biện kỹ thuật. | Hoàn thiện Mục 5 trong `group_report.md`, giải quyết dứt điểm các băn khoăn về rào cản API và cước phí chờ. |
| Mức can thiệp AI | Phản biện luận điểm lựa chọn mức can thiệp: Khẳng định nếu chỉ bật điều hòa thì Rule là đủ, nhưng vì bài toán đòi hỏi hiểu câu lệnh tự nhiên đa điều kiện, tối ưu lộ trình ghé siêu thị và xử lý dữ liệu cổng thi công thời gian thực nên bắt buộc cần mức Agent. | Đóng góp lập luận cốt lõi cho câu hỏi *"Vì sao không chọn mức đơn giản hơn"* ở Mục 6.2. |
| Quyết định | Tham gia đánh giá 4 loại rủi ro (Value, Usability, Feasibility, Viability); đề xuất ngưỡng dừng (Kill-switch) đo lường cụ thể cho dự án pilot. | Nhóm đồng thuận ra quyết định Not Yet (chỉ triển khai bản thử nghiệm hẹp 2 tuần tại VinUni / Vinhomes Ocean Park trước khi quyết định Go chính thức). |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tìm kiếm và mở rộng góc nhìn về các vấn đề thường gặp trong học tập kỹ thuật theo 4 lăng kính. | Gợi ý bối cảnh thực tế về sự cố xung đột môi trường/thư viện (CUDA, dependencies) và xung đột Git khi làm việc nhóm. | AI bị quán tính "solution-first", đưa ra các giải pháp trá hình gắn mác problem (như *"cần chatbot tóm tắt bài giảng"*, *"thiếu tool tự chia việc"*). Nếu chép vào sẽ vi phạm quy chế và bị trừ điểm nặng theo rubric C1. | Loại bỏ toàn bộ các từ khóa giải pháp; tự viết lại 100% theo đúng cú pháp Job Story (*Khi... tôi muốn... để...*); gán các con số đo lường thực tế từ trải nghiệm thật của bản thân (190 phút đọc slide, 60–90 phút tranh luận chia việc). |
| CP2 Problem Card | Đóng vai "PM hoài nghi" để bóc tách lỗ hổng logic của Problem Card #1 trước khi mang đi pitch với nhóm. | Chỉ ra rất đúng ranh giới của âm thanh: Audio không thể giải thích được công thức toán KaTeX và code; cảnh báo metric "tỷ lệ nhớ $\ge 80\%$" là bất khả thi để đo đạc khách quan trong ngắn hạn. | AI hời hợt khi rập khuôn gợi ý mô hình podcast 2 người nói chuyện (giống NotebookLM) mà không nhận ra nó làm loãng mật độ kiến thức và tốn thời gian vô ích với tài liệu học thuật kỹ thuật. | Bác bỏ mô hình 2 người; tự định hình cấu trúc 1 người giảng bài cô đọng kết hợp câu hỏi gợi mở đào sâu; thiết kế thêm Cheat Sheet 1 trang đi kèm để bù đắp điểm mù thị giác của audio; quy đổi cách đo metric sang bài mini-quiz 5 câu kiểm tra trước giờ học. |
| CP4 Research | Tra cứu các giải pháp trợ lý giọng nói trên xe điện và nền tảng điều phối đa dịch vụ. | Tìm kiếm thông tin về Google Assistant, Apple Shortcuts và các tính năng trợ lý ảo trên xe VinFast. | AI có xu hướng tổng hợp chung chung về tính năng trợ lý ảo toàn cầu mà bỏ qua ngữ cảnh bản địa tại Việt Nam. | Bổ sung phân tích về khoảng trống dữ liệu vi mô nội khu (micro-routing) và tính khép kín của hệ sinh thái Vingroup. |
| CP5 Quy trình | Chuyển đổi ý tưởng quy trình sang cú pháp sơ đồ Mermaid và bảng Before/After. | Hỗ trợ sinh nhanh cú pháp Mermaid rendering bằng elk và phân tầng Rule/AI/HITL. | Ban đầu AI chỉ đề xuất luồng đơn giản (về nhà bật điều hòa) thiếu tính thực tế và dễ bị coi là macro đơn giản. | Tự đưa vào bối cảnh thực tế: Lộ trình đa chặng ghé WinMart mua đồ giảm giá và bài toán giải quyết điểm mù thi công nội khu VinUni / Ocean Park. |
| CP5–6 Problem Statement | Soạn thảo 6 trường của Problem Statement v0 và phản biện tính khả thi của Boundary. | Gợi ý cấu trúc 6 trường theo chuẩn Lean UX & Google PAIR. | Boundary ban đầu AI gợi ý chưa chặt về mặt giao dịch tiền bạc và an toàn cổng trường. | Thiết lập Financial Gate bắt buộc con người xác nhận trước khi gọi xe và giới hạn AI chỉ định tuyến vào các cổng đã được BQL xác nhận an toàn. |
| CP6 Mức can thiệp / quyết định | Tham khảo các tiêu chí phân định Rule, Workflow, Agent và 4 loại rủi ro của Marty Cagan. | Cung cấp khung ma trận độ mơ hồ × độ phức tạp và cấu trúc AI Canvas chuẩn mực. | AI dễ đưa ra kết luận vội vàng khuyên chọn Agent toàn năng mà không xét kỹ chi phí và rủi ro trễ mạng API. | Nhấn mạnh việc chỉ chọn Agent cho khâu lập kế hoạch đa bước và xử lý ngữ cảnh động, còn các lệnh thiết bị và gọi xe cụ thể vẫn neo chặt vào Rule và xác nhận con người (HITL). |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi lắng nghe top 3 problems của các bạn trong nhóm, tôi nhận thấy sự phân mảnh thông tin và gánh nặng đọc hiểu là nỗi đau phổ biến ở nhiều hoàn cảnh khác nhau. Bạn Tùng gặp vấn đề khi phải đọc các paper nghiên cứu và tài liệu ngoại ngữ dài 15–20 trang trước buổi học mất tới 1–2 tiếng, điều này có cùng bản chất với nỗi đau đọc slide bài giảng 80 trang của tôi. Trong khi đó, bài toán của bạn Huy về Agent giọng nói trong hệ sinh thái Vingroup mở ra góc nhìn rộng lớn hơn về việc kết nối các dịch vụ rời rạc (Green SM, Vinhomes Smart Home, WinMart) để giải phóng thời gian cho người dùng bận rộn hoặc đang lái xe. Tôi học được rằng một vấn đề có giá trị cao không nhất thiết phải là bài toán kỹ thuật hàn lâm phức tạp, mà là bài toán chạm đúng vào các bước nghẽn gây lãng phí thời gian hàng ngày của người dùng.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm tôi đã bị cuốn vào tư duy "solution-first" ngay từ đầu buổi làm việc. Cả nhóm lập tức bàn luận về việc "xây dựng chatbot thông minh", "làm tool audio tự động" hay "tạo app gọi xe tích hợp trợ lý ảo". Chúng tôi nhận ra mình đang phạm luật khi đối chiếu lại với rubric và worksheet của môn học: chưa hề có dữ liệu về việc người dùng thực tế đang mất bao nhiêu phút và kẹt ở bước nào. Nhóm đã xử lý bằng cách dừng toàn bộ việc thảo luận về tính năng AI, cùng nhau phân rã quy trình hiện tại thành 6 bước thủ công, gắn số phút đo đạc thực tế cho từng bước. Nhờ đó, nhóm mới vỡ lẽ ra rằng bottleneck thực sự nằm ở việc chuyển đổi app và điểm mù thông tin công trường thi công nội khu, chứ không phải người dùng thiếu một giao diện chat.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tôi đã có hai lần đổi ý rất quan trọng trong buổi làm việc hôm nay:
1. *Ở bài cá nhân:* Ban đầu tôi định làm mô hình podcast 2 người đàm thoại giống NotebookLM. Nhưng sau khi nghe phản biện rằng format đối thoại 2 người có nhiều câu thoại xã giao rườm rà, làm loãng mật độ kiến thức của một bài giảng chuyên ngành, tôi đã đổi ý hoàn toàn sang mô hình 1 người giảng bài cô đọng (độc thoại sư phạm) kết hợp chèn các câu hỏi gợi mở đào sâu và đính kèm Cheat Sheet 1 trang để mắt nhìn song song.
2. *Ở bài nhóm:* Ban đầu kịch bản của Huy khá đơn giản, chỉ là câu lệnh "về nhà bật điều hòa và đặt xe". Tôi đã phản biện rằng bài toán này quá giống một macro/shortcut đơn giản của Google Assistant hay Siri và chưa đủ sức thuyết phục để cần đến Agent. Tôi đã đề xuất nâng tầm kịch bản thành bài toán thực tế: Lộ trình đa chặng ghé WinMart mua đồ giảm giá và xử lý điểm mù thi công cổng trường VinUni. Cả nhóm đã đồng thuận với đề xuất này và cập nhật lại toàn bộ quy trình CP5.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều làm tôi bất ngờ nhất khi đối chiếu nghiên cứu là việc ngay cả các gã khổng lồ công nghệ như Google Maps hay Apple Shortcuts đều hoàn toàn "mù" trước dữ liệu vi mô nội khu (micro-routing) của một khuôn viên lớn như VinUni hay Vinhomes Ocean Park. Một chiếc xe công nghệ không thể biết được cổng nào của trường đang bị rào chắn sửa chữa, dẫn đến việc tài xế thả khách cách xa cả cây số hoặc chạy lòng vòng gọi điện cãi nhau. Điều này chứng minh rằng việc kết hợp dữ liệu Ban Quản Lý nội bộ với Agent giọng nói không phải là một ý tưởng viển vông mà là một nhu cầu thực tế chưa có ai giải quyết trọn vẹn.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất khi viết Problem Statement là việc phân định rạch ròi giữa Nỗi đau và Giải pháp, đồng thời thiết lập các rào chắn an toàn (Boundary) chặt chẽ. Rất khó để không buột miệng đưa chữ "AI", "Agent" hay "tự động hóa" vào phần mô tả vấn đề. Ngoài ra, việc thiết lập Boundary đòi hỏi phải tư duy thực tế về các rủi ro nguy hiểm: tuyệt đối cấm AI tự động trừ tiền đặt xe nếu người dùng chưa xác nhận rõ ràng (Financial Gate), và tuyệt đối cấm AI can thiệp vào khóa cửa thông minh (Smart Lock) hay camera an ninh.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu có cơ hội làm lại từ đầu, tôi sẽ phản biện nhóm mạnh hơn ngay từ bước CP3 về tính khả thi kỹ thuật (Feasibility) của việc xin cấp quyền truy cập API dữ liệu thời gian thực từ Ban Quản Lý khu đô thị/trường học. Trong thực tế, các đơn vị vận hành thường rất chậm chạp trong việc mở API nội bộ. Do đó, việc xây dựng cơ chế cập nhật bán thủ công từ thông báo hàng ngày của BQL hoặc cho phép cộng đồng tài xế báo lỗi (crowdsourced) cần được đặt ra ngay từ đầu như một phương án cứu cánh bắt buộc, thay vì giả định rằng API luôn sẵn sàng.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Bài toán của nhóm xuất phát từ vấn đề người dùng mất từ 18 đến 28 phút để thao tác qua lại giữa 6 ứng dụng khác nhau và thường xuyên bị tài xế thả nhầm sảnh do công trường thi công nội khu. Quy trình mới giải quyết bằng cách nhận diện giọng nói, bóc tách câu lệnh đa điều kiện để tự động gửi lệnh ngầm bật điều hòa phòng khách 24°C, đồng thời tra cứu dữ liệu cổng trường thông thoáng và yêu cầu người dùng xác nhận cước phí trước khi chính thức gọi xe Green SM. Chỉ số đo lường thành công thực tế là rút ngắn thời gian thao tác xuống dưới 30 giây, kéo tỷ lệ tài xế gọi điện lạc đường xuống dưới 5% và đạt tỷ lệ bật điều hòa thành công từ 95% trở lên. Ranh giới an toàn được chốt cứng: AI không bao giờ được tự ý trừ tiền đặt xe khi người dùng chưa đồng ý, và tuyệt đối không được cấp quyền điều khiển khóa cửa thông minh. Nhóm chọn mức can thiệp Agent vì bài toán đòi hỏi tự động lập kế hoạch đa bước và xử lý linh hoạt dữ liệu động thời gian thực từ nhiều bên, điều mà các quy tắc tĩnh hay workflow cố định không thể đáp ứng. Quyết định cuối cùng là Not Yet, chỉ triển khai thử nghiệm hẹp 2 tuần tại khu vực VinUni và Vinhomes Ocean Park kèm ngưỡng dừng rõ ràng: nếu sau 2 tuần mà tỷ lệ tài xế gọi điện hỏi đường vẫn vượt quá 20% thì tạm dừng dự án để chuẩn hóa lại dữ liệu bản đồ nội khu.

---

## 7. Tài liệu tham khảo

- Jeff Gothelf & Josh Seiden, *Lean UX: Designing Great Products with Agile Teams*, O'Reilly Media.
- Rob Fitzpatrick, *The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you*.
- Google PAIR (People + AI Research), *People + AI Guidebook*, pair.withgoogle.com.
- Anthropic, *Building Effective Agents*, anthropic.com/research/building-effective-agents.
- Marty Cagan, *Inspired: How to Create Tech Products Customers Love*, Silicon Valley Product Group (SVPG).
- Teresa Torres, *Continuous Discovery Habits: Discover Products that Create Customer Value and Business Value*.
