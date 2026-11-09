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
| CP1 Scan | Tìm kiếm và mở rộng góc nhìn về các vấn đề thường gặp trong học tập kỹ thuật theo 4 lăng kính. | Gợi ý bối cảnh thực tế về sự cố xung đột môi trường/thư viện (CUDA, dependencies) và xung đột Git khi làm việc nhóm. | AI bị quán tính "solution-first", đưa ra các giải pháp trá hình gắn mác problem (như *"cần chatbot tóm tắt bài giảng"*, *"thiếu tool tự chia việc"*). Nếu chép vào sẽ vi phạm quy chế và bị trừ điểm nặng theo rubric C1. | Loại bỏ toàn bộ các từ khóa giải pháp; tự viết lại 100% theo đúng cú pháp Job Story (*Khi... tôi muốn... để...*); gán các con số đo lường thực tế từ trải nghiệm thật của bản thân (190 phút đọc slide, 60–90 phút tranh luận chia việc). |
| CP2 Problem Card | Đóng vai "PM hoài nghi" để bóc tách lỗ hổng logic của Problem Card #1 trước khi mang đi pitch với nhóm. | Chỉ ra rất đúng ranh giới của âm thanh: Audio không thể giải thích được công thức toán KaTeX và code; cảnh báo metric "tỷ lệ nhớ $\ge 80\%$" là bất khả thi để đo đạc khách quan trong ngắn hạn. | AI hời hợt khi rập khuôn gợi ý mô hình podcast 2 người nói chuyện (giống NotebookLM) mà không nhận ra nó làm loãng mật độ kiến thức và tốn thời gian vô ích với tài liệu học thuật kỹ thuật. | Bác bỏ mô hình 2 người; tự định hình cấu trúc 1 người giảng bài cô đọng kết hợp câu hỏi gợi mở đào sâu; thiết kế thêm Cheat Sheet 1 trang đi kèm để bù đắp điểm mù thị giác của audio; quy đổi cách đo metric sang bài mini-quiz 5 câu kiểm tra trước giờ học. |
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

-
