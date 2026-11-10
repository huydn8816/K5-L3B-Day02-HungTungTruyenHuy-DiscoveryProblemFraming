# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: HungTungTruyenHuy
- Candidate problem nhóm chọn (1 câu): Agent giọng nói đa bước cho các ứng dụng thuộc hệ sinh thái của Vingroup
- Quyết định cuối (Go / Not Yet / No-Go): Go

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Đặng Nhật Huy| 2A202603822 | Trưởng nhóm | huydn8816 |
| 2 | Đoàn Anh Hùng | 2A202603880 | Thành viên | doananhhung |
| 3 | Nguyễn Thanh Tùng| 2A202603807 | Thành viên | thanhtung578804 |
| 4 | Nguyễn Trọng Truyền | 2A202603868 | Thành viên | truien |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Trọng Truyền | Nguyễn Thanh Tùng | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Nguyễn Thanh Tùng | Nguyễn Trọng Truyền | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Thanh Tùng | Nguyễn Trọng Truyền | Bảng research có link |
| CP5 — Quy trình trước/sau | Đoàn Anh Hùng | Đặng Nhật Huy | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Đoàn Anh Hùng | Đặng Nhật Huy| Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Đặng Nhật Huy | Đoàn Anh Hùng | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Đặng Nhật Huy | Đoàn Anh Hùng | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### HoVaTen-MSSV

#### DoanAnhHung-2A202603880

**Phần việc phụ trách:**

- Chịu trách nhiệm chính Checkpoint 5 (CP5): Thiết kế toàn bộ quy trình Trước / Sau (Mục 4) và soạn thảo Problem Statement v0 (Mục 5) trong `report/team/group_report.md`.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Phân rã quy trình hiện tại 6 bước thủ công với thời gian thực tế 18–28 phút, làm rõ 2 bottleneck chính: phân mảnh ứng dụng (Vinhomes, VinID, Green SM) và điểm mù thi công nội khu.
- Thiết kế sơ đồ quy trình tương lai bằng cú pháp Mermaid chuẩn (`flowchart LR`), phân định rạch ròi 3 tầng: Rule (truy vấn API WinMart, BQL), AI (bóc tách ý định câu nói tự nhiên) và Human-in-the-loop (Financial Gate xác nhận giá tiền cuốc xe).
- Tích hợp 2 vòng lặp phản hồi (Feedback Loops): Vòng lặp làm rõ ý định khi ASR nhiễu và Vòng lặp điều chỉnh phương án khi người dùng đổi ý (ghé quán khác hoặc đi thẳng).
- Hoàn thiện bảng so sánh Before / After chứng minh việc giảm 95% thời gian thao tác và loại bỏ nguy cơ tài xế bị kẹt cổng thi công.
- Soạn thảo Problem Statement v0 với 6 trường chuẩn mực, thiết lập Success Metric đo lường qua 10 chuyến xe thử nghiệm thực tế và xây dựng 3 rào chắn an toàn (Boundary) nghiêm ngặt (loại trừ quyền can thiệp vào khóa cửa thông minh Smart Lock).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Toàn bộ Mục 4 (Quy trình trước/sau) và Mục 5 (Problem Statement v0) trong `report/team/group_report.md`.
- Tệp báo cáo cá nhân `report/individual/2A202603880_DoanAnhHung.md` (Mục 4 và Mục 5).

**Điều mình học được từ phần nhóm:**

- Nhận thức rõ ràng sự khác biệt giữa một "Macro/Shortcut đơn giản" và một "Agentic Workflow": Nếu chỉ dừng lại ở lệnh bật điều hòa và đặt xe thì chỉ cần rule cố định; chỉ khi giải quyết bài toán đa ngữ cảnh (tối ưu lộ trình ghé siêu thị có khuyến mãi, né cổng trường thi công) thì AI mới thực sự phát huy giá trị vượt trội.
- Tầm quan trọng của ranh giới an toàn (Boundary) và Human-in-the-loop: Với các tác vụ liên quan đến tiền tệ (đặt xe) hoặc an ninh nhà ở (khóa cửa), tuyệt đối không để AI tự quyết định hoàn toàn mà phải luôn có bước xác nhận rõ ràng của con người.

#### NguyenThanhTung-2A202603807

**Phần việc phụ trách:**

- Phụ trách chính Checkpoint 4 (CP4): Lập Assumption Map (Mục 3.1), phỏng vấn kiểm chứng và khảo sát (Mục 3.2), research các giải pháp đã có (Mục 3.3) trong `report/team/group_report.md`.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Lập bảng 5 giả định của nhóm theo 4 loại rủi ro; chọn ra 2 giả định quan trọng nhất (#1 và #2) về nhu cầu ra lệnh gộp và mức độ tin tưởng khi giao dịch tiền qua AI để kiểm chứng trước.
- Thu thập phản bác quan trọng: 2/3 người kịch liệt phản đối việc để Agent tự động chốt cuốc và trừ tiền trong thẻ mà không hỏi lại. Từ đó đề xuất nhóm đổi sang mô hình có bước xác nhận bằng giọng nói (HITL).
- Làm poll nhanh 5 bạn trong lớp: 3/5 bạn muốn ra lệnh 1 câu xử lý xuyên app, 2/5 bạn thấy dùng phím tắt/widget trên màn hình khóa là đủ.
- Research 3 giải pháp thị trường (Apple Shortcuts, trợ lý ViVi trên xe VinFast, Rabbit R1); chỉ ra bài học dùng Function Calling qua API chính thức thay vì cho AI tự bấm màn hình.
- Viết và hoàn thiện toàn bộ Mục 3 trong `report/team/group_report.md`.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- Toàn bộ Mục 3 (Kiểm chứng + research giải pháp đã có) trong `report/team/group_report.md`.
- Tệp báo cáo cá nhân `report/individual/2A202603807_NguyenThanhTung.md` .
**Điều mình học được từ phần nhóm:**

- Biết cách hỏi theo The Mom Test để tìm ra sự thật: Không hỏi "bạn thấy ý tưởng này thế nào", mà đào sâu vào lần gần nhất họ gặp khó khăn và đang tự xoay xở ra sao. Nhờ đó nhóm mới phát hiện ra lỗ hổng về việc đặt xe trước khi bắt tay vào vẽ quy trình.
- Hiểu được nguyên tắc cốt lõi khi làm AI Agent: Tự động hóa hoàn toàn không đồng nghĩa với trải nghiệm tốt. Một Agent thông minh phải biết phân định ranh giới — việc an toàn thì chủ động làm ngay, nhưng đụng đến tiền bạc hay quyền riêng tư thì bắt buộc phải dừng lại xin xác nhận (Human-in-the-loop) để người dùng luôn giữ quyền kiểm soát.

#### NguyenTrongTruyen-2A202603868
Phần việc phụ trách:
- CP3: Đóng góp Problem Cards, phản biện candidate của thành viên khác và tham gia so sánh shortlist.
- CP6 : Phụ trách đánh giá mức can thiệp AI, xây dựng AI Canvas và hoàn thiện Problem Statement v1 cùng tiêu chí đánh giá tại Mục 6–7 trong report/team/group_report.md.
Đóng góp cụ thể và sản phẩm bàn giao:
- CP3: Đóng góp ba candidate về nhập đơn vào ERP, đối chiếu hóa đơn và ghép phiếu giao hàng; đặt câu hỏi phản biện cho candidate #1, #4, #11, tập trung vào lợi ích so với công cụ hiện có. Candidate nhập đơn ERP được đưa vào shortlist.
- CP6: Lập ma trận độ mơ hồ × độ phức tạp; so sánh No AI / Rule / Workflow / Agent và giải thích lý do chọn.
- Xây dựng AI Canvas, xác định đầu vào, đầu ra của AI, quyết định của người dùng và cách lấy phản hồi.
- Hoàn thiện Problem Statement v1 từ v0 của Hùng; bổ sung điểm can thiệp AI, rủi ro, người kiểm tra và phương án xử lý lỗi.
- Xây dựng tiêu chí đánh giá: hiểu đúng ý định, hỏi lại khi thiếu thông tin, xác nhận trước khi đặt xe và báo đúng trạng thái từng tác vụ.
- Soạn tình huống kiểm thử: đổi giờ, đổi điểm đón, nhận dạng giọng nói sai, API lỗi và chỉ một trong hai tác vụ thành công.
Bằng chứng / vị trí bàn giao:
- CP3 đã có: Mục 2.1 của report/team/group_report.md, các candidate #7–#9 và câu hỏi phản biện tại #1, #4, #11; Mục 2.4, candidate #7 trong shortlist.
- CP6: Mục 6.1–6.4 và Mục 7 của báo cáo nhóm.

Điều mình học được từ phần nhóm:
- Cần làm rõ actor, bottleneck và bằng chứng trước khi chọn giải pháp; số liệu ước tính cần được kiểm chứng.
- Phân biệt trường hợp quy tắc hoặc workflow cố định đã đủ với trường hợp cần agent.
- Chuyển yêu cầu thành tiêu chí kiểm tra cụ thể, giữ bước xác nhận của người dùng đối với thao tác phát sinh chi phí.

#### DangNhatHuy-2A202603822
**Phần việc phụ trách:** Nhóm trưởng. Fork và quản lý repo nhóm, điều phối phân công, tổng hợp và viết toàn bộ báo cáo nhóm (mục 1–10), làm file phụ trong `report/assets/` và bộ slide thuyết trình.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- **Quản lý repo:** fork repo `K5-L3B-Day02-HungTungTruyenHuy-DiscoveryProblemFraming`, tạo nhánh cho từng thành viên, review và merge pull request từ các nhánh vào `main`.
- **CP2–CP3:** pitch 3 candidate (#1 bật điều hòa và đặt xe khi bận tay, #2 tủ đổi pin còn pin khi tới nơi, #3 hiểu cảnh báo xe điện và tìm gara); đặt câu hỏi phản biện cho #6, #9, #12; gom 12 candidate thành 6 cluster; vẽ OST; chấm điểm shortlist và viết lý do chọn #1.
- **CP4:** lập Assumption Map 5 giả định; tổng hợp Interview Snapshot và kết quả micro-poll; viết bảng research 3 giải pháp đã có (Apple Shortcuts, trợ lý ViVi, Rabbit R1); ghi lại cách nhóm sửa problem sau kiểm chứng (thêm cổng xác nhận tiền, thêm Action Card).
- **CP5:** viết quy trình hiện tại, quy trình tương lai (sơ đồ Mermaid có boundary, HITL và phương án quay về), bảng before/after và Problem Statement v0.
- **CP6:** viết ma trận mơ hồ × phức tạp, so sánh 4 mức can thiệp, AI Canvas, 2 câu hỏi Google PAIR, Problem Statement v1, 5 tiêu chí eval, chấm 4 rủi ro và quyết định Not Yet kèm ngưỡng dừng.
- **Rà soát và sửa:** sửa Job Story chứa sẵn giải pháp; thống nhất actor với quy trình; bổ sung tiêu đề mục 3 bị thiếu; sửa quyết định ở mục 1 cho khớp với mục 8; điền bằng chứng phỏng vấn vào mục 6.4 và 8.1.
- **File phụ và thuyết trình:** `cp2-workflow-card-1.png`, `cp4-interview-snapshot-1.md`, `cp4-survey-result.png`, `cp5-workflow-future.png`; bộ slide 10 trang.

**Bằng chứng**
- Repo nhóm: `https://github.com/huydn8816/K5-L3B-Day02-HungTungTruyenHuy-DiscoveryProblemFraming`
- Lịch sử commit trên `main` (hơn 18 commit) và pull request đã merge, ví dụ PR #2 từ nhánh `truien`: [link PR]
- File báo cáo nhóm: `report/[tên thư mục]/group_report.md`
- File phụ: thư mục `report/assets/`
- Slide thuyết trình: [link slide]

**Điều mình học được từ phần nhóm:**
Làm nhóm trưởng và viết toàn bộ báo cáo giúp mình thấy rõ nhất là các mục phải khớp với nhau. Khi đọc lại cả báo cáo, mình phát hiện mục 4–5 đã trôi sang kịch bản nhiều điểm dừng trong khi mục 2 và mục 7 vẫn là kịch bản 2 việc, và mục 1 ghi Go trong khi mục 8 kết luận Not Yet. Từng phần riêng lẻ đều ổn, nhưng ghép lại thì mâu thuẫn. Bài học thứ hai là bằng chứng quan trọng hơn lập luận. Trước khi phỏng vấn, mình tin agent tự làm hết là tốt nhất; sau khi 2/3 người nói họ "ghê tay" nếu agent tự đặt xe trừ tiền, nhóm phải thêm cổng xác nhận và chọn Agent có giới hạn. Cuối cùng, câu hỏi phản biện của Truyền về Siri Shortcuts buộc mình chỉ ra được điểm khác biệt thật: không phải "có giọng nói", mà là xử lý được yêu cầu thay đổi mỗi lần.