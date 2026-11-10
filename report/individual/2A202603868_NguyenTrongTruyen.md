# Báo cáo cá nhân — Nguyễn Trọng Truyền — 2A202603868

> Báo cáo Day 02 — Discovery & Problem Framing, nhóm HungTungTruyenHuy, lớp L3B.
> Mục 4–5 được tổng hợp từ nội dung đã ghi trong repo và lượt hỗ trợ hoàn thiện file này. Phần reflection 6.1–6.6 là **bản nháp minh họa do AI hỗ trợ**, không phải xác nhận về trải nghiệm thực tế của học viên; cần được người học tự viết lại theo trải nghiệm của mình trước khi nộp.

## 1. Thông tin học viên

- Họ tên: Nguyễn Trọng Truyền
- MSSV: 225748020110258
- Mã học viên dùng trong repo và tên file: 2A202603868
- Email trường (không bắt buộc, repo có thể để public): Không cung cấp.
- Lớp: K5 — L3B
- Tên nhóm: HungTungTruyenHuy
- Link repo nhóm: https://github.com/huydn8816/K5-L3B-Day02-HungTungTruyenHuy-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

### Năm điểm nghẽn vận hành

**Cơ sở ước tính:** Các khối lượng và thời gian dưới đây là kịch bản dùng để so sánh bài toán, chưa có nhật ký xử lý hoặc bộ chứng từ thực tế để xác nhận. Chi phí công được quy đổi theo giả định **150.000 đồng/giờ**. Tổng 150,5 giờ, tương đương khoảng 22,6 triệu đồng/tháng, là công sức hiện tại trong kịch bản, chưa phải khoản tiền có thể tiết kiệm nhờ AI.

| # | Lăng kính | Job Story (Khi… tôi muốn… để…) | Ai chịu ảnh hưởng? | Bước nghẽn và công sức ước tính |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | **Soạn bảng đáp ứng yêu cầu chào thầu.** Khi nhận hồ sơ có nhiều tiêu chí kỹ thuật, tôi muốn tìm đúng dòng thông số và tài liệu của từng model, để nộp bảng đáp ứng đúng hạn và có căn cứ. | Nhân viên kinh doanh dự án, kỹ sư giải pháp | Mở từng PDF, đối chiếu tiêu chí như PoE, số cổng và tốc độ, rồi chép thông số vào bảng. **6 hồ sơ/tháng × 4 giờ tra cứu và nhập lại = 24 giờ/tháng (3,6 triệu đồng).** |
| 2 | Lặp lại · Tốn thời gian | **Nhập đơn đặt hàng vào ERP.** Khi nhận đơn từ khách dưới dạng PDF hoặc Excel, tôi muốn xác định đúng mã hàng, số lượng và đơn vị tính, để kho soạn đúng và đơn kịp chuyến giao. | Nhân viên xử lý đơn, kho, khách hàng | Đọc từng dòng, tra mã theo tên hàng của khách và nhập lại vào ERP. Mã hoặc đơn vị tính sai khiến kho phải dừng để xác nhận. **600 đơn/tháng × 6 phút = 60 giờ/tháng (9 triệu đồng).** |
| 3 | Lặp lại · Pain từ người khác | **Gắn phiếu giao hàng đã ký vào đúng đơn.** Khi tài xế gửi ảnh phiếu giao hàng, tôi muốn biết phiếu thuộc chuyến nào và có ghi giao thiếu hay không, để chốt trạng thái giao hàng trong ngày. | Điều phối, tài xế, bộ phận đối soát | Mở ảnh trong nhóm chat, dò mã phiếu hoặc tên khách trong ERP và hỏi lại khi ảnh mờ hoặc thiếu mã. **240 phiếu ảnh/tháng × 5 phút = 20 giờ/tháng (3 triệu đồng).** |
| 4 | Cần đọc, tổng hợp nhiều thông tin · Pain từ người khác | **Kiểm tra hồ sơ bảo hành thiết bị.** Khi khách gửi ảnh tem và mô tả lỗi, tôi muốn tìm đúng số sê-ri, giao dịch bán và thời hạn bảo hành, để phản hồi khách ngay lần đầu hoặc yêu cầu đúng giấy tờ còn thiếu. | Nhân viên bảo hành, kỹ thuật viên, khách hàng | Gõ lại số sê-ri, tìm hóa đơn và tra chính sách của hãng. Nếu đọc nhầm ký tự, nhân viên phải dò lại hoặc yêu cầu khách chụp lại. **180 hồ sơ/tháng × 8 phút = 24 giờ/tháng (3,6 triệu đồng).** |
| 5 | Lặp lại · Tốn thời gian | **Xử lý hóa đơn nhà cung cấp bị lệch.** Khi hóa đơn lệch so với đơn mua hoặc phiếu nhập, tôi muốn biết dòng nào sai và còn thiếu chứng từ gì, để xác minh trước hạn thanh toán. | Kế toán công nợ, mua hàng, kho | Mở ba chứng từ, dò từng dòng và liên hệ kho hoặc mua hàng để xác nhận trường hợp giao từng phần hay sai đơn vị tính. **500 hóa đơn/tháng × 18% có ngoại lệ × 15 phút = 22,5 giờ/tháng (~3,38 triệu đồng).** |

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

Ưu tiên bài toán có người chịu trách nhiệm rõ, bước nghẽn đo được, dữ liệu để kiểm tra kết quả và phương án đơn giản có thể thử trong một buổi lab. Khối lượng và thời gian gốc lấy từ kịch bản CP1. Thời lượng các bước còn lại và các ngưỡng mục tiêu là giả định để thiết kế phép thử.

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | CP1 #2 — Nhập đơn đặt hàng vào ERP | Bước nhập chiếm 60 giờ/tháng theo kịch bản, cao nhất trong năm bài toán. Đơn gốc, danh mục hàng và bản ghi ERP cho phép so thời gian và lỗi trên cùng bộ đơn. | Bao nhiêu đơn dùng mẫu cố định hoặc có mã khách hàng ánh xạ được? Sai mã, sai số lượng và lỡ chuyến giao hiện xảy ra bao nhiêu lần? |
| 2 | CP1 #5 — Xử lý hóa đơn nhà cung cấp bị lệch | Có ba chứng từ để đối chiếu và quy tắc nghiệp vụ rõ cho nhiều trường hợp. Bỏ sót một khoản lệch có thể dẫn đến thanh toán sai hoặc thanh toán chậm. | Hóa đơn có trường tham chiếu đơn mua hay phải dò tay? ERP có ghi giao từng phần, đơn vị quy đổi và dung sai đã duyệt không? |
| 3 | CP1 #3 — Gắn phiếu giao hàng đã ký vào đúng đơn | Mã lần giao có thể gắn ngay khi tài xế gửi ảnh. Thử được với một tuyến giao và đo trực tiếp tỷ lệ phiếu chốt đúng ngày. | Tài xế có thể gửi qua biểu mẫu trên tuyến không? Bao nhiêu đơn giao nhiều lần và bao nhiêu phiếu có ghi giao thiếu? |

Hai bài toán còn lại được giữ làm ứng viên sau. Với **#1 chào thầu**, danh mục thông số có cấu trúc và mẫu bảng theo model có thể điền các tiêu chí lặp lại bằng quy tắc. Tiêu chí viết tự do vẫn cần kỹ sư thẩm định, nên phải đo riêng phần tra cứu có thể chuẩn hóa. Với **#4 bảo hành**, biểu mẫu bắt buộc số sê-ri và bảng chính sách theo hãng có thể xử lý hồ sơ đủ dữ liệu bằng tra cứu chính xác. Cần xác minh hệ thống có liên kết số sê-ri với hóa đơn bán và lưu đúng phiên bản chính sách trước khi chọn.

### Problem Card #1 — Nhập đơn đặt hàng vào ERP

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách gửi đơn đặt hàng qua email, tôi muốn đưa đúng mã hàng, số lượng và đơn vị tính vào ERP, để kho soạn đúng và kịp chuyến giao. |
| Actor | Nhân viên xử lý đơn là người nhập và kiểm. Nhân viên kho nhận đơn đã xác nhận để soạn hàng. |
| Thời điểm / bối cảnh | Khi đơn PDF hoặc Excel đến gần giờ chốt chuyến, tên hàng trên đơn có thể khác tên trong danh mục nội bộ. |
| Quy trình hiện tại (3–7 bước) | Mở email và đơn gốc → xác định khách và báo giá → đọc dòng hàng, tra mã, nhập ERP → so lại bản nháp với đơn gốc → lưu đơn để kho nhận. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 mất khoảng 6 phút/đơn theo CP1. Nhân viên phải dò tên viết tắt, mã và quy cách trước khi nhập từng dòng. |
| Impact (nếu không giải thì sao) | 600 đơn × 6 phút = 60 giờ/tháng tại bước 3. Sai mã hoặc đơn vị tính khiến kho phải dừng để xác nhận, có thể lỡ chuyến. Chưa có số đo về tần suất lỡ chuyến. |
| Success metric (baseline → target) | Thời gian công trung bình từ lúc bắt đầu đọc dòng hàng đến khi đã so và sửa xong bản nháp (bước 3–4) **8 phút giả định → ≤5 phút/đơn**. Tính cả đơn phải nhập tay. Theo dõi tỷ lệ đơn kịp giờ chốt chuyến. Trên cùng tập đơn, tỷ lệ sai mã, số lượng hoặc đơn vị sau khi lưu phải bằng hoặc thấp hơn phương án nhập tay. |
| Phương án không dùng AI | Cung cấp mẫu Excel có mã và đơn vị tính bắt buộc, đọc các mẫu có cấu trúc bằng bộ nhập, ánh xạ tên hàng theo từng khách. ERP kiểm tra mã, quy đổi đơn vị và chặn trùng theo khách + số đơn. Đưa trường hợp thiếu dữ liệu hoặc có nhiều mã khả dĩ về hàng chờ xử lý tay. |
| Giả thuyết về AI (nếu có) | Chỉ thử trích xuất hoặc gợi ý mã cho phần PDF nhiều bố cục hay tên hàng chưa có trong bảng ánh xạ. Đo phần cải thiện thêm so với phương án quy tắc, gồm thời gian người duyệt và sửa lỗi. |
| Cảm nhận nhanh | **Rule trước.** Nếu đầu vào chuẩn hoặc tra được bằng bảng mã, kết quả có thể kiểm lại từng dòng và dùng lại ở lần sau. |

Quy trình nháp hiện tại:

```text
[1. Mở email và đơn gốc: 1 phút]
→ [2. Tìm hồ sơ khách và báo giá: 1 phút]
→ [3. Đọc dòng hàng, tra mã và nhập ERP: 6 phút] ← BƯỚC NGHẼN
→ [4. So bản nháp với đơn gốc: 2 phút]
→ [5. Lưu đơn và chuyển kho: 1 phút]
```

### Problem Card #2 — Xử lý hóa đơn nhà cung cấp bị lệch

| Trường | Nội dung |
|---|---|
| Job Story | Khi hóa đơn không khớp đơn mua hoặc phiếu nhập, tôi muốn thấy dòng chênh lệch và chứng từ còn thiếu, để xác minh trước hạn thanh toán. |
| Actor | Kế toán công nợ xử lý ngoại lệ, mua hàng và kho xác nhận đơn mua và số thực nhận. |
| Thời điểm / bối cảnh | Khi ghi nhận hóa đơn, nhất là giao từng phần hoặc hóa đơn và phiếu nhập dùng đơn vị tính khác nhau. |
| Quy trình hiện tại (3–7 bước) | Mở hóa đơn đã bị đánh dấu lệch → tìm đơn mua và phiếu nhập → rà từng dòng và so chênh lệch → gửi yêu cầu xác minh → cập nhật kết quả khi có phản hồi. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 mất khoảng 15 phút công/hóa đơn ngoại lệ theo CP1. Kế toán phải dò từng dòng để tìm lệch số lượng, đơn giá hoặc chứng từ. Thời gian đợi phản hồi được ghi riêng. |
| Impact (nếu không giải thì sao) | 500 hóa đơn × 18% ngoại lệ × 15 phút = 22,5 giờ/tháng cho bước rà lệch theo giả định. Một khoản lệch bị bỏ qua có thể dẫn đến trả tiền cho hàng chưa nhận hoặc giữ lại nhầm hóa đơn hợp lệ. |
| Success metric (baseline → target) | Thời gian công trung bình để phát hiện và ghi lý do lệch **15 phút giả định → ≤8 phút/hóa đơn ngoại lệ đã xác minh**. Kiểm tra trên cả hóa đơn khớp và lệch. Báo riêng tỷ lệ ngoại lệ bị bỏ sót và tỷ lệ hồ sơ khớp bị giữ nhầm, theo bộ đáp án kế toán xác nhận. Không bỏ sót sai lệch trọng yếu trong bộ thử theo ngưỡng do kế toán xác định trước. |
| Phương án không dùng AI | Đối chiếu ba bên theo mã đơn mua, mã dòng hàng và đơn vị quy đổi. Cộng số đã nhận và trừ phần đã lập hóa đơn theo từng dòng để xử lý giao từng phần. Áp dụng dung sai số lượng và đơn giá đã duyệt. Ghi trường lệch, dữ liệu gốc và quy tắc bị vi phạm. Thiếu tham chiếu hoặc nhiều dòng có thể khớp thì chuyển kế toán xác minh. |
| Giả thuyết về AI (nếu có) | Nếu nhiều chứng từ chỉ có ảnh hoặc mô tả không có mã, thử đọc trường và gợi ý dòng có thể liên quan. Quy tắc vẫn tính chênh lệch, kế toán xác nhận chứng từ và quyết định thanh toán. |
| Cảm nhận nhanh | **Rule.** Khi có dữ liệu có cấu trúc, phép đối chiếu và dung sai cho kết quả nhất quán, giải thích được khi kiểm toán. |

Quy trình nháp hiện tại:

```text
[1. Mở hóa đơn ngoại lệ: 1 phút]
→ [2. Tìm đơn mua và phiếu nhập: 3 phút]
→ [3. Rà từng dòng, xác định khoản lệch: 15 phút] ← BƯỚC NGHẼN
→ [4. Gửi yêu cầu xác minh: 2 phút]
→ [5. Ghi kết quả sau phản hồi: 2 phút]
```

### Problem Card #3 — Gắn phiếu giao hàng đã ký vào đúng đơn

| Trường | Nội dung |
|---|---|
| Job Story | Khi tài xế gửi ảnh phiếu giao có chữ ký, tôi muốn xác định đúng lần giao và biết có giao thiếu hay không, để chốt trạng thái trong ngày. |
| Actor | Nhân viên điều phối đối soát phiếu, tài xế nộp ảnh và ghi tình trạng giao thực tế. |
| Thời điểm / bối cảnh | Cuối chuyến, ảnh được gửi vào nhóm chat. Một đơn có thể chia nhiều lần giao và ảnh đôi khi thiếu mã phiếu. |
| Quy trình hiện tại (3–7 bước) | Tài xế chụp và gửi ảnh → điều phối mở ảnh, dò lần giao trong ERP và hỏi lại nếu thiếu mã → kiểm chữ ký và tình trạng giao thiếu → gắn ảnh và cập nhật trạng thái. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 mất khoảng 5 phút công/ảnh theo CP1. Thiếu mã lần giao khiến điều phối phải tìm theo tên khách hoặc hỏi lại tài xế. |
| Impact (nếu không giải thì sao) | 240 ảnh × 5 phút = 20 giờ/tháng cho bước tìm và ghép. Gắn sai phiếu hoặc chốt muộn khiến bộ phận đối soát thiếu bằng chứng giao đúng chuyến. |
| Success metric (baseline → target) | Thời gian công trung bình cho việc dò và gắn ảnh (bước 2 và 4, kể cả trường hợp cần thao tác tay) **6 phút giả định → ≤3 phút/phiếu**. Đo thêm tổng phút của tài xế và điều phối để phát hiện chuyển việc sang tài xế, cùng tỷ lệ lần giao đủ hồ sơ trước giờ chốt ngày. Không có phiếu gắn nhầm trong bộ thử đã đối chiếu với dữ liệu chuyến. |
| Phương án không dùng AI | Sinh mã duy nhất cho mỗi lần giao và gửi tài xế liên kết có điền sẵn mã. Bắt buộc ảnh và trạng thái giao đủ/thiếu. Xác thực mã và tuyến theo dữ liệu phân công, chặn nộp trùng, chuyển phiếu giao thiếu hoặc thiếu bằng chứng sang điều phối kiểm. |
| Giả thuyết về AI (nếu có) | Thử đọc mã và ghi chú viết tay trên ảnh cũ hoặc ảnh từ đối tác chưa dùng được biểu mẫu. Điều phối xác nhận khi thiếu mã, ảnh mờ hoặc nhiều lần giao có thể khớp. |
| Cảm nhận nhanh | **No AI + Rule.** Ghi mã có cấu trúc ngay lúc nộp ảnh giúp bỏ bước dò tên và giảm rủi ro nhầm hai chuyến của cùng khách. |

Quy trình nháp hiện tại:

```text
[1. Chụp và gửi ảnh vào nhóm chat: 2 phút]
→ [2. Mở ảnh và dò đúng lần giao: 5 phút] ← BƯỚC NGHẼN
→ [3. Kiểm chữ ký và ghi chú giao thiếu: 1 phút]
→ [4. Gắn ảnh và cập nhật ERP: 1 phút]
```

### Card muốn pitch nhất

- **Card số 1 — Nhập đơn đặt hàng vào ERP.**
- **Vì sao:** Có khối lượng lớn và dữ liệu gốc để so ba cách trên 50 đơn chia theo loại đầu vào. Nếu đạt mức 8 → 5 phút trên toàn bộ đơn, kịch bản 600 đơn cho khoảng 30 giờ công giải phóng mỗi tháng. Đây là cơ sở để đánh giá lợi ích trước khi tính chi phí triển khai và vận hành.
- **Câu hỏi muốn nhóm phản biện:** Nếu phần lớn đơn nhập được bằng mẫu chuẩn và bảng ánh xạ tên hàng, nhóm sẽ dùng kết quả nào trên phần đơn còn lại để chứng minh AI giúp giảm công mà vẫn giữ đúng mã, số lượng và đơn vị tính?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| **1. Logic tài chính — CFO:** 22,6 triệu đồng/tháng của CP1 là giá trị quy đổi từ giờ công giả định. Dùng toàn bộ số đó làm lợi ích của AI sẽ tính luôn thời gian bắt buộc phải rà soát và bỏ qua chi phí triển khai, duy trì bảng mã, sửa lỗi. Thời gian giải phóng cũng chỉ chuyển thành tiền khi giảm được chi thực tế hoặc có cách sử dụng công suất đó. | Có | Ghi rõ số nào là giả định. Tính giờ giải phóng từ chênh lệch thời gian trước và sau trên cùng phạm vi, gồm công kiểm tra và xử lý tay. Khi xét ROI, quy đổi phần công suất thực sự dùng được rồi trừ chi phí triển khai phân bổ và vận hành. |
| **2. Metric vận hành — Trưởng phòng Vận hành:** Phút trung bình không cho biết đơn có kịp giờ chốt, hàng có bị soạn sai hay phiếu có gắn đúng chuyến. Chỉ đo hồ sơ hệ thống xử lý được sẽ bỏ qua ngoại lệ. Giảm công của điều phối bằng cách tăng công của tài xế cũng dễ tạo ra số đẹp trên một bộ phận. | Có | Xác định điểm bắt đầu và kết thúc theo từng card. Dùng cùng mẫu có cả ca thường và ngoại lệ, tính cả xử lý tay, theo dõi thời gian công và chỉ số lỗi riêng. Mẫu 50 đơn dùng để sàng lọc cách làm, cần dữ liệu rộng hơn để kết luận về lỗi hiếm. |
| **3. Logic giải pháp — CFO và Trưởng phòng Vận hành:** CP1 mô tả AI có thể hỗ trợ nhưng chưa chứng minh cần AI ở bước gây tốn công. Các thao tác có khóa định danh, phép tính và điều kiện nghiệp vụ ổn định có thể xử lý bằng mã quy tắc. Kết quả có thể tái hiện và truy vết từng quyết định, thuận tiện khi sửa lỗi hoặc kiểm toán. | Có | Mỗi card có phương án quy tắc để so: bảng mã và kiểm tra trường khi nhập đơn, mã lần giao có sẵn khi nộp phiếu, đối chiếu ba chứng từ khi xử lý hóa đơn. Đo độ bao phủ và chi phí duy trì trước. Chỉ thử AI trên nhóm dữ liệu khó chuẩn hóa còn tốn công sau bước này. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

**Căn cứ tổng hợp:** Phần cá nhân của Nguyễn Trọng Truyền trong [TEAM.md](../../TEAM.md) ghi nhận đóng góp CP3 và CP6; sản phẩm tương ứng nằm ở mục 2 và mục 6–7 của [báo cáo nhóm](../team/group_report.md). Các câu hỏi dưới đây được chép từ bảng pitch; bảng đó hiện ghi tên người hỏi là phân công đề xuất, nên chưa đủ để xác nhận câu hỏi đã được nói trực tiếp tại lớp.

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Đóng góp ba candidate: #7 nhập đơn ERP, #8 đối chiếu hóa đơn lệch, #9 ghép phiếu giao hàng. Card muốn pitch nhất là nhập đơn ERP, có bottleneck 6 phút/đơn theo kịch bản. | Ba candidate có mặt ở mục 2.1; #7 vào shortlist với 27 điểm. Bài cá nhân làm rõ phương án Rule trước khi thử thêm AI. |
| Phản biện bài của bạn khác | Câu hỏi gắn tên tôi cho #1 của Huy: “So với Siri Shortcuts, agent của nhóm xử lý tốt hơn thế nào khi người dùng vừa yêu cầu bật điều hòa, vừa đổi giờ hoặc điểm đón xe trong cùng một câu?” Hai câu hỏi khác cho #4 của Tùng và #11 của Hùng tập trung vào lợi ích so với Jobscan và checklist Trello. | Câu hỏi buộc đề xuất nêu tình huống mà công cụ hiện có chưa xử lý đủ tốt. Phép so sánh ở mục 2.4 có cả nút “Về nhà”, luồng giọng nói cố định và Agent; mục 6.2 có điều kiện hạ mức. |
| Nhận phản biện | Câu hỏi của Tùng ghi cho #7: “So với luồng nhập đơn của Dynamics 365, cách của nhóm tiết kiệm được bao nhiêu thời gian cho đơn PDF nhiều mẫu khi tính cả công sửa sai mã hàng?” Hùng hỏi #8 về giao từng phần; Huy hỏi #9 về ảnh thiếu mã chuyến. | Bản card hiện tại tính cả công kiểm và sửa, so với cách nhập có quy tắc, không lấy toàn bộ 60 giờ nhập đơn làm lợi ích AI. Mục tiêu 8 → 5 phút/đơn là giả định cần thử; phương án nhập tay và lỗi mã hàng vẫn được tính trong kết quả. |
| Gom cluster / cây OST | Đưa #7–#9 vào cluster D: đối chiếu dữ liệu giữa các nguồn. Đối chiếu cây OST để tách nhu cầu người dùng khỏi các ý như Agent giọng nói hoặc nút “Về nhà”. | Mục 2.2 có sáu cluster. Cây ở mục 2.3 dùng outcome về thời gian và hoàn thành công việc; các ý giải pháp được ghi riêng bên dưới cây. |
| Chọn candidate problem | Tham gia so shortlist #1, #6 và #7 theo actor, quy trình, bằng chứng, impact và khả năng thử. Ghi nhận #6 đạt 31 điểm, #1 đạt 29, #7 đạt 27. | Nhóm chọn #1 để so các mức can thiệp trong cùng một tình huống. #7 chưa được chọn vì thiếu đơn thực tế và danh mục hàng; #6 dễ kiểm bằng script. Điểm tổng là đầu vào thảo luận, lý do chọn được ghi riêng tại mục 2.4. |
| Kiểm chứng / research | Vai trò hỗ trợ CP4 theo TEAM.md; dùng kết quả do nhóm ghi nhận để xem lại nhu cầu và ranh giới an toàn. Phỏng vấn và research do Tùng phụ trách; báo cáo này không bổ sung cuộc phỏng vấn nào. | Tổng hợp nhóm ghi 2/3 người phản đối tự chốt giao dịch khi chưa xác nhận và 2/5 người trong poll thấy phím tắt đã đủ. Đây là lý do giữ xác nhận tiền và tiếp tục so với Rule; poll về sở thích chưa chứng minh người dùng sẽ sử dụng. |
| Quy trình nhóm | Phần CP5 do Hùng phụ trách. Ở phần CP6, làm rõ AI hiểu và lập kế hoạch, Workflow thực thi, Rule kiểm tra điều kiện và người dùng xác nhận trước khi đặt xe. | Các tình huống bàn giao trong TEAM.md gồm đổi giờ, đổi điểm đón, nhận dạng sai, API lỗi và chỉ một tác vụ thành công. Đây là tình huống cần kiểm thử, chưa phải kết quả chạy thử. |
| Problem Statement | Theo phần đóng góp cá nhân trong TEAM.md, phụ trách hoàn thiện v1 và tiêu chí đánh giá ở mục 7: actor chính là nhân viên văn phòng, bottleneck là thao tác hai app khi bận tay; bổ sung metric, boundary và người kiểm tra. | V1 ghi mục tiêu thời gian ~2–3 phút → dưới 20 giây, số lần chạm 15–20 → 0 và trạng thái cuối đúng ≥85%. Baseline vẫn là ước tính; các ngưỡng là mục tiêu, chưa phải kết quả đạt được. |
| Mức can thiệp AI | Xây dựng ma trận mơ hồ × phức tạp, so No AI / Rule / Workflow / Agent và AI Canvas theo phần việc cá nhân đã ghi. Đề xuất Agent có giới hạn ở bước hiểu yêu cầu và lập kế hoạch. | Không cần giao mọi bước cho Agent: Rule giữ giá trị mặc định và cổng xác nhận, Workflow gọi dịch vụ. Lý do dùng Agent phải được kiểm bằng lợi ích thêm so với các luồng đơn giản hơn. |
| Quyết định | Dùng phân tích Value, Usability, Feasibility và Viability để đối chiếu đề xuất ở CP6 với quyết định cuối do nhóm ghi tại mục 8. | **Not Yet**: cần đo baseline, so với nút “Về nhà”, kiểm tra an toàn và chi phí. Sau hai tuần, dừng hướng Agent nếu trạng thái cuối đúng dưới 70%, có giao dịch chưa xác nhận hoặc dưới 3/5 người thử chọn giọng nói. |

**Điểm còn cần thống nhất ở bài nhóm:** Mục 4–5 đang mô tả kịch bản mở rộng gồm ghé WinMart và tránh cổng thi công, với thời gian 18–28 phút; mục 7 quay về hai tác vụ bật điều hòa và đặt xe, với baseline 2–3 phút. Hai phạm vi này không dùng chung một phép so trước/sau. Phần thông tin chung trong TEAM.md cũng còn ghi “Go”, trong khi mục 1 và mục 8 của báo cáo nhóm ghi “Not Yet”. Báo cáo cá nhân này dùng phạm vi v1 tại mục 7 và quyết định tại mục 8; các điểm lệch trên chưa được coi là đã sửa trong bài nhóm.

---

## 5. Dùng AI

**Phạm vi nhật ký:** Mục 3 đã có nội dung phản biện AI cho CP2 nhưng chưa lưu hội thoại hoặc thời điểm sử dụng. Các dòng còn lại mô tả việc AI hỗ trợ đối chiếu và biên tập trong lượt hoàn thiện file này, không xác nhận học viên đã dùng AI tại từng checkpoint trong buổi học. Cột cuối ghi cách xử lý thể hiện trong bản báo cáo, cần người học rà lại trước khi nhận là quyết định của mình.

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Trong lượt hoàn thiện: kiểm tra năm Job Story, phép tính công sức và cách ghi độ tin cậy của số liệu. Không có nhật ký riêng về việc dùng AI khi scan ban đầu. | Phân biệt bước nghẽn cụ thể với mô tả chung; kiểm tra tổng 150,5 giờ/tháng và suất công 150.000 đồng/giờ. | Chưa có bằng chứng ngoài kịch bản để coi tần suất, thời gian hoặc chi phí là số đo thực tế. | Giữ các số làm giả định, ghi nguồn ước tính ngay trước bảng; không dùng chúng làm bằng chứng ROI. |
| CP2 Problem Card | Nội dung đã có: nhờ AI phản biện theo góc nhìn CFO và Trưởng phòng Vận hành. Lượt này rà lại tính nhất quán của phản biện với ba card. | Chỉ ra thiếu chi phí duyệt và sửa lỗi, nhầm giờ công với tiền tiết kiệm, và cần so với phương án Rule. | Phản biện vẫn chưa thay thế được mẫu đơn, dữ liệu ERP hoặc người xử lý thật; các ngưỡng 5, 8 và 3 phút chưa được thử. | Tính cả ngoại lệ, kiểm tra và nhập tay; so trên cùng phạm vi. Giữ mục tiêu là giả thuyết thử nghiệm và thêm điều kiện về lỗi. |
| CP4 Research | Trong lượt này: đối chiếu kết quả kiểm chứng đã ghi ở mục 3 của bài nhóm và snapshot trong repo. Không phỏng vấn, không khảo sát mới. | Nối tín hiệu phản bác với boundary và việc cần so với phím tắt. | Có ba người được báo cáo là đã phỏng vấn nhưng chỉ hai snapshot trong bài nhóm; poll năm người chưa đại diện cho thị trường. Lượt này chưa kiểm chứng các claim về sản phẩm bên ngoài. | Ghi rõ đây là dữ liệu nhóm báo cáo; không tạo snapshot thứ ba, không thêm số liệu thị trường và không suy rộng từ lời khen giải pháp. |
| CP5 Quy trình | Trong lượt hoàn thiện: so mô tả quy trình với actor, metric và phạm vi v1. Chưa có nhật ký xác nhận việc cá nhân dùng AI để vẽ CP5 tại lớp. | Phát hiện phạm vi 18–28 phút ở CP5 khác phạm vi 2–3 phút ở v1. | Nếu ghép số của hai kịch bản, bản so trước/sau sẽ cho tỷ lệ cải thiện không có căn cứ. | Dùng phạm vi hai tác vụ theo v1 trong báo cáo cá nhân và ghi rõ phần bài nhóm cần thống nhất. |
| CP5–6 Problem Statement | Trong lượt này: kiểm tra chuỗi actor → quy trình → bottleneck → metric → boundary dựa trên v1 đã có. | Nhắc phân biệt target với kết quả và yêu cầu xác nhận trước hành động có tiền. | Câu “không có lần chạm” không đồng nghĩa với “không cần xác nhận”; thời gian 20 giây chưa được đo. | Giữ xác nhận bằng giọng nói hoặc thao tác người dùng; đo cả thời gian hỏi lại, xác nhận và xử lý lỗi, ghi riêng thời gian chờ xe. |
| CP6 Mức can thiệp / quyết định | Trong lượt này: đối chiếu ma trận, AI Canvas, tiêu chí đánh giá và quyết định Not Yet. | Làm rõ vai trò riêng của hiểu yêu cầu, thực thi và kiểm tra điều kiện. | Lập luận trong bài nhóm rằng Workflow chỉ hiểu một ý và không hỏi lại là quá tuyệt đối; một luồng định sẵn vẫn có thể có nhiều bước và nhánh làm rõ. | Xem Agent là lựa chọn cần kiểm chứng bằng yêu cầu biến đổi, không chỉ bằng số app; giữ Rule và Workflow làm phương án so sánh. |
| CP7 Biên tập báo cáo | Trong lượt hoàn thiện này: AI soạn bản nháp minh họa cho mục 6.1–6.6 và phần diễn giải tham khảo 6.7. | Gợi ý cách gắn bài học với candidate ERP, phản biện về Shortcuts, metric và ranh giới xác nhận. | AI không biết trải nghiệm tại lớp hoặc cảm nhận thật của học viên; câu chuyện minh họa không phải bằng chứng cá nhân. | Gắn nhãn bản nháp minh họa; người học cần tự viết lại reflection theo trải nghiệm thật theo yêu cầu CP7. |

---

## 6. Reflection (CP7)

> **Bản nháp minh họa cho 6.1–6.6:** Các đoạn dưới đây dùng ngôi “tôi” để gợi ý cách diễn đạt từ tình huống trong repo, không xác nhận rằng người học đã có những suy nghĩ hoặc trao đổi này. CP7 yêu cầu câu trả lời bằng trải nghiệm thật, tối thiểu 200 từ cho 6.1–6.6; người học cần tự viết lại trước khi nộp. Mục 6.7 là phần giải thích tham khảo để tự luyện trình bày.

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi đối chiếu ba bài toán của tôi với các candidate của Huy, Tùng và Hùng, tôi thấy công việc tốn thời gian chưa chắc đã cần AI. Kiểm tra tên file có thể dùng script; ghép phiếu giao có thể bắt đầu bằng mã lần giao; bật điều hòa và gọi xe có thể dùng một nút cài sẵn nếu ngày nào cũng giống nhau. Điều cần làm rõ là actor đang bị nghẽn ở bước nào và phương án đơn giản xử lý được đến đâu. Vì vậy, tôi ưu tiên câu hỏi về lợi ích thêm so với công cụ đã có, thay vì chỉ hỏi giải pháp dùng công nghệ gì.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Một dấu hiệu solution-first là gọi ngay đề tài là “Agent giọng nói đa bước”, trong khi nhu cầu thực sự là chuẩn bị nhà và xe khi đang bận tay. Cách gọi đầu tiên dễ khiến nhóm mặc định phải chọn Agent. Tôi sẽ diễn đạt lại Job Story theo kết quả người dùng muốn đạt, sau đó so thao tác hiện tại, nút “Về nhà”, Workflow và Agent trên cùng tình huống. Một điểm khác cần sửa là phạm vi CP5 mở rộng sang WinMart và cổng thi công, trong khi v1 chỉ tập trung hai tác vụ. Không thống nhất phạm vi thì metric dễ bị chọn theo hướng có lợi cho giải pháp.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Tình huống minh họa là phản biện của Tùng đối với card nhập đơn ERP: tiết kiệm được bao nhiêu khi tính cả công sửa sai mã hàng? Nếu chỉ nhìn 600 đơn nhân 6 phút, tôi dễ coi 60 giờ là phần có thể tự động hóa hết. Sau phản biện đó, cách đánh giá hợp lý hơn là tính cả bước nhập và kiểm tra, dùng baseline giả định 8 phút rồi thử mục tiêu 5 phút trên cùng bộ đơn. Tôi cũng cần so với mẫu Excel và bảng ánh xạ mã trước. Phần PDF khó đọc chỉ đáng thử AI khi tổng công duyệt, sửa và xử lý ngoại lệ thực sự giảm mà lỗi không tăng.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điểm đáng chú ý trong kết quả nhóm ghi lại là có người gặp bất tiện khi chuyển app nhưng vẫn không muốn giao toàn bộ quyền cho Agent. Hai trong ba người được báo cáo là phản đối tự chốt giao dịch khi chưa xác nhận; hai trong năm người ở poll cho rằng phím tắt đã đủ. Điều này cho thấy xác nhận được pain chưa đồng nghĩa với xác nhận được giải pháp. Tôi cần phân biệt lời kể về lần gần nhất gặp khó khăn, ý kiến về một ý tưởng và hành vi chọn dùng trong thử nghiệm. Những tỷ lệ từ mẫu nhỏ giúp đặt câu hỏi tiếp theo, chưa đủ để kết luận cho toàn bộ nhóm người dùng.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là giữ actor, bottleneck, metric và boundary cùng nói về một bài toán. Với phạm vi bật điều hòa và đặt xe, tôi cần đo từ khi bắt đầu thao tác đến khi có trạng thái xác nhận của cả hai việc, tính cả hỏi lại và xác nhận giá. Thời gian chờ tài xế nhận cuốc phải được ghi riêng để không lẫn với công thao tác. Mục tiêu dưới 20 giây cũng chỉ có ý nghĩa nếu đặt đúng xe, bật đúng thiết bị và không bỏ qua sự đồng ý của người dùng. Các mức 85%, 90% và 100% trong bộ tiêu chí là ngưỡng cần đánh giá, chưa phải chất lượng hệ thống đã đạt.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ thu hẹp actor và tình huống trước khi vẽ quy trình tương lai, rồi đo thao tác thật trên một nhóm nhỏ thay vì bắt đầu từ số phút ước tính. Tôi sẽ yêu cầu có phương án so sánh dùng Rule và Workflow, kể cả nhánh hỏi lại khi thiếu thông tin. Tôi cũng sẽ chuẩn bị các ca đổi điểm đón, nhận sai địa chỉ, API lỗi và chỉ một tác vụ thành công để kiểm tra cách báo trạng thái. Điểm tôi muốn phản biện mạnh hơn là bằng chứng nào đủ để chọn Agent, quyền tích hợp dịch vụ đã có chưa và tiêu chí nào buộc nhóm dừng hoặc hạ mức.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Nhân viên văn phòng sống tại Vinhomes, khi tan họp và đang bận tay, cần bật điều hòa ở nhà và đặt xe Green SM với ít thao tác. Quy trình hiện tại là mở app nhà thông minh, bật điều hòa, chuyển sang app gọi xe, nhập thông tin rồi kiểm tra kết quả hai việc; bước nghẽn là chuyển app và nhập lại khi đang di chuyển. Nhóm đặt mục tiêu từ baseline ước tính 2–3 phút và 15–20 lần chạm xuống dưới 20 giây và 0 lần chạm khi dùng giọng nói, đồng thời trạng thái cuối đúng đạt ít nhất 85%; cần bấm giờ và chấm trên cùng bộ tình huống để kiểm chứng. Ranh giới là không tự đặt xe hoặc thanh toán khi chưa xác nhận, không đoán thông tin bắt buộc, không mở khóa cửa và phải báo rõ tác vụ nào thất bại. Mức đề xuất là Agent có giới hạn để hiểu và lập kế hoạch, Workflow để thực thi, Rule để kiểm tra và giữ bước người dùng xác nhận. Agent chỉ có cơ sở được chọn nếu giúp hơn Rule hoặc Workflow trên các yêu cầu thay đổi, vì một kịch bản cố định có thể xử lý đơn giản hơn. Quyết định hiện tại là Not Yet vì chưa có số đo hành vi đủ mạnh, chưa xác minh khả năng tích hợp thật và chưa rõ chi phí vận hành. Bước tiếp theo là đo với năm người và thử trong hai tuần; dừng hướng Agent nếu trạng thái cuối đúng dưới 70%, có bất kỳ giao dịch chưa xác nhận hoặc dưới ba trong năm người chọn giọng nói thay vì nút cài sẵn.

---

## 7. Tài liệu tham khảo

- [TEAM.md — phân công và phần đóng góp của Nguyễn Trọng Truyền](../../TEAM.md): căn cứ tổng hợp vai trò CP3, hỗ trợ CP4 và sản phẩm CP6; phần thông tin chung còn cần thống nhất quyết định với báo cáo nhóm.
- [Báo cáo nhóm](../team/group_report.md): mục 2 về pitch, phản biện, cluster và shortlist; mục 3 về kết quả kiểm chứng do nhóm ghi nhận; mục 6–8 về mức can thiệp, Problem Statement v1, tiêu chí và quyết định Not Yet.
- [CP4 — Interview Snapshot #1](../assets/cp4-interview-snapshot-1.md): lời kể về thao tác hai app và việc quên bật điều hòa; thời gian theo lời kể, chưa phải số bấm giờ.
- [Worksheet Day 02](../../docs/01-worksheet.md): cấu trúc Job Story, Problem Card, AI Canvas, bốn rủi ro và câu hỏi reflection.
- [Các framework quốc tế dùng trong lab](../../docs/03-international-frameworks.md): tài liệu học về The Mom Test, OST, Problem Statement, Google PAIR và các mức can thiệp.
- [RULES.md](../../RULES.md), [RUBRIC.md](../../RUBRIC.md) và [CHECKPOINTS.md](../../CHECKPOINTS.md): yêu cầu bằng chứng, cách khai báo AI, nội dung CP7 và tiêu chí đánh giá.

Không bổ sung số liệu thị trường hoặc kết quả phỏng vấn mới trong lượt hoàn thiện này. Các số vận hành CP1–CP2 là giả định đã ghi rõ; các kết quả CP4 được dẫn lại theo tài liệu nhóm, chưa được kiểm chứng độc lập trong báo cáo cá nhân.
