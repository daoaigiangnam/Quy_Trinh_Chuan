# Nhóm F — Kết thúc hợp đồng và cải tiến

Bộ quy trình chuẩn Mstar — bản dự thảo ngày 2026-10-14. Tài liệu được thiết kế dùng chung cho dịch vụ IT Outsourcing; các yêu cầu cụ thể được cấu hình trong phụ lục khách hàng.

## Quy tắc áp dụng

- Quy trình lõi dùng chung; phụ lục khách hàng xác định phạm vi, SLA, đầu mối, quyền, retention, thông báo sự cố và yêu cầu phục hồi.
- Mọi thao tác trên hệ thống khách hàng phải được hợp đồng/ủy quyền cho phép.
- Bằng chứng phải có thể truy nguyên: ticket, phê duyệt, log, biên bản, kết quả kiểm tra.
- Không lưu mật khẩu, token, API key hoặc secret dạng rõ trong ticket/repository thông thường.
- Quy trình chỉ có hiệu lực sau khi được rà soát và phê duyệt; đây không phải tuyên bố Mstar đã được chứng nhận ISO.
- Tham chiếu: ISO/IEC 27001:2022 và ISO/IEC 27002:2022; mapping cuối cùng cần căn cứ risk assessment và SoA.

## Danh mục trong nhóm

| Mã | Quy trình | Mục đích |
|---|---|---|
| [QT-CS-01](#qt-cs-01) | Kết thúc hợp đồng dịch vụ khách hàng | Kết thúc dịch vụ có kiểm soát, xử lý ticket tồn, dữ liệu, quyền, tài sản và nghĩa vụ còn lại. |
| [QT-CS-02](#qt-cs-02) | Bàn giao hệ thống cho khách hàng/nhà cung cấp mới | Chuyển giao hồ sơ, cấu hình, dữ liệu và quyền hợp lệ để bên nhận tiếp quản an toàn, giảm gián đoạn. |
| [QT-CS-03](#qt-cs-03) | Thu hồi quyền và xóa dữ liệu sau hợp đồng | Ngăn quyền và dữ liệu khách hàng tồn ngoài mục đích/thời hạn, đồng thời giữ dữ liệu có nghĩa vụ lưu hợp lệ. |
| [QT-QL-01](#qt-ql-01) | Quản lý KPI và cải tiến dịch vụ | Chuẩn hóa KPI, nguồn dữ liệu, báo cáo, phân tích nguyên nhân và hành động cải tiến dịch vụ. |

---
## QT-CS-01 — Kết thúc hợp đồng dịch vụ khách hàng

**Mục đích:** Kết thúc dịch vụ có kiểm soát, xử lý ticket tồn, dữ liệu, quyền, tài sản và nghĩa vụ còn lại.

**Kích hoạt:** Khi có yêu cầu/sự kiện thuộc phạm vi, khi có thay đổi đáng kể hoặc theo chu kỳ được quy định.

**Phạm vi:** Mstar và hoạt động IT Outsourcing trong phạm vi hợp đồng/ủy quyền. Phụ lục từng khách hàng phải xác định hệ thống, SLA, đầu mối, quyền truy cập, retention, thông báo và yêu cầu phục hồi riêng.

**Vai trò:** Người yêu cầu/đầu mối khách hàng; người thực hiện; người kiểm tra/chủ sở hữu hệ thống; chủ sở hữu quy trình; IT Lead; người phê duyệt theo ma trận thẩm quyền. Người thực hiện không tự phê duyệt rủi ro trọng yếu do chính mình tạo ra.

**Đầu vào:** Yêu cầu/ticket; hợp đồng/phụ lục; danh mục hệ thống/tài sản; quyền được ủy quyền; quy trình liên quan; dữ liệu/bằng chứng hiện có.

**Đầu ra:** Hồ sơ xử lý; kết quả đã xác minh; phê duyệt; ticket/biên bản đóng; việc tồn có owner và hạn.

### Trình tự thực hiện

| Bước | Hoạt động | Vai trò chính | Hướng dẫn và kiểm soát | Bằng chứng cần lưu |
|---:|---|---|---|---|
| 1 | Tiếp nhận và xác định phạm vi | Người tiếp nhận | Ghi nhận yêu cầu/sự kiện, xác minh hệ thống, mục tiêu, phạm vi hợp đồng, đầu mối và thông tin tối thiểu. Nếu thiếu thông tin hoặc thẩm quyền thì chưa thực hiện bước rủi ro. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 2 | Kiểm kê | Người thực hiện và người kiểm tra | Liệt kê ticket mở, tài sản, quyền, dữ liệu/bản sao, cấu hình, vendor và rủi ro. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 3 | Thống nhất bàn giao | Người thực hiện và người kiểm tra | Chốt dữ liệu trả/xóa/giữ, tài liệu, quyền, mốc chuyển và tiêu chí nghiệm thu. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 4 | Thực hiện chuyển giao/thu hồi | Người thực hiện và người kiểm tra | Bàn giao theo quyền; thu hồi tài khoản/token; xử lý dữ liệu theo hợp đồng. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 5 | Xác minh, đóng và lưu hồ sơ | Chủ sở hữu quy trình/IT Lead | Người kiểm tra xác nhận kết quả, quyền và phạm vi; ghi thời gian, bằng chứng, quyết định, thông báo và việc tồn. Chỉ đóng khi đủ hồ sơ hoặc có ngoại lệ được duyệt. | Ticket, log, phê duyệt hoặc biên bản tương ứng |

### Lưu đồ

```mermaid
flowchart TD
  A([Bắt đầu]) --> S1["Tiếp nhận và xác định phạm vi"]
  S1 --> D1{"Đủ thông tin và đúng thẩm quyền?"}
  D1 -- Không --> F1[/"Bổ sung thông tin hoặc xin phê duyệt"/]
  F1 --> S1
  D1 -- Có --> S2["Kiểm kê"]
  S2 --> S3["Thống nhất bàn giao"]
  S3 --> D2{"Có rủi ro/ngoại lệ cần xử lý?"}
  D2 -- Có --> S4["Thực hiện chuyển giao/thu hồi"]
  D2 -- Không --> S5["Xác minh, đóng và lưu hồ sơ"]
  S4 --> S5
  S5 --> D3{"Kết quả đạt, bằng chứng đủ?"}
  D3 -- Không --> R[/"Khắc phục hoặc mở lại công việc"/]
  R --> S3
  D3 -- Có --> Z([Kết thúc])
```

### Biểu mẫu và hồ sơ

- FR-QTCS01-01: Phiếu yêu cầu/checklist khởi tạo.
- FR-QTCS01-02: Hồ sơ đánh giá, phê duyệt hoặc xác minh.
- FR-QTCS01-03: Nhật ký thực hiện/biên bản/báo cáo.
- FR-QTCS01-04: Xác nhận hoàn tất và theo dõi việc tồn.

*Mã biểu mẫu là mã đề xuất; khi ban hành cần đưa vào danh mục tài liệu, xác định chủ sở hữu, nơi lưu, quyền truy cập và thời hạn lưu giữ.*

### KPI và giám sát

- Tỷ lệ hồ sơ có đủ thông tin đầu vào và phê duyệt.
- Tỷ lệ bước/công việc hoàn thành đúng hạn theo quy trình hoặc hợp đồng.
- Số lỗi, ngoại lệ, sự cố hoặc hồ sơ phải làm lại.
- Tỷ lệ hành động khắc phục đóng đúng hạn.

Chủ sở hữu quy trình phải xác định nguồn dữ liệu, công thức, chu kỳ đo và ngưỡng cảnh báo trước khi áp dụng.

### Ngoại lệ và an toàn thông tin

Bàn giao theo quyền; thu hồi tài khoản/token; xử lý dữ liệu theo hợp đồng.

- Không thao tác ngoài phạm vi hợp đồng/ủy quyền; khi thiếu quyền hoặc phê duyệt phải tạm dừng bước có rủi ro.
- Không ghi mật khẩu, API key, token, khóa riêng hoặc mã khôi phục dạng rõ trong ticket, README, email thường hay tài liệu bàn giao.
- Thay đổi hệ thống phải theo QT-IT-13; nghi ngờ sự cố ATTT phải theo QT-ATTT-04; ngoại lệ phải theo QT-ISMS-04.
- Mọi ngoại lệ phải có lý do, đánh giá rủi ro, biện pháp bù trừ, người phê duyệt, owner và hạn hết hiệu lực.

### Phụ lục cần cấu hình theo khách hàng

| Trường | Nội dung xác nhận |
|---|---|
| Khách hàng/mã hợp đồng | Theo hợp đồng đang hiệu lực |
| Phạm vi hệ thống/dịch vụ | Hệ thống, tenant, site, tài sản và loại dịch vụ |
| SLA/lịch hỗ trợ | Theo hợp đồng/phụ lục, không dùng mặc định chung |
| Đầu mối yêu cầu/phê duyệt | Chức danh, kênh liên hệ và người thay thế |
| Quyền/kênh kỹ thuật | Phạm vi ủy quyền, MFA, VPN, thời hạn |
| Dữ liệu/lưu giữ | Phân loại, nơi lưu, thời hạn, trả/xóa |
| Thông báo sự cố | Kênh, người nhận và thời hạn |
| Ngoại lệ/rủi ro tồn dư | Mã hồ sơ, phê duyệt, bù trừ, ngày hết hạn |

**Trạng thái:** Dự thảo v0.1 — chờ rà soát, thử nghiệm và phê duyệt. Mapping ISO chỉ mang tính định hướng; cần xác nhận theo phạm vi ISMS, đánh giá rủi ro và SoA.

---

## QT-CS-02 — Bàn giao hệ thống cho khách hàng/nhà cung cấp mới

**Mục đích:** Chuyển giao hồ sơ, cấu hình, dữ liệu và quyền hợp lệ để bên nhận tiếp quản an toàn, giảm gián đoạn.

**Kích hoạt:** Khi có yêu cầu/sự kiện thuộc phạm vi, khi có thay đổi đáng kể hoặc theo chu kỳ được quy định.

**Phạm vi:** Mstar và hoạt động IT Outsourcing trong phạm vi hợp đồng/ủy quyền. Phụ lục từng khách hàng phải xác định hệ thống, SLA, đầu mối, quyền truy cập, retention, thông báo và yêu cầu phục hồi riêng.

**Vai trò:** Người yêu cầu/đầu mối khách hàng; người thực hiện; người kiểm tra/chủ sở hữu hệ thống; chủ sở hữu quy trình; IT Lead; người phê duyệt theo ma trận thẩm quyền. Người thực hiện không tự phê duyệt rủi ro trọng yếu do chính mình tạo ra.

**Đầu vào:** Yêu cầu/ticket; hợp đồng/phụ lục; danh mục hệ thống/tài sản; quyền được ủy quyền; quy trình liên quan; dữ liệu/bằng chứng hiện có.

**Đầu ra:** Hồ sơ xử lý; kết quả đã xác minh; phê duyệt; ticket/biên bản đóng; việc tồn có owner và hạn.

### Trình tự thực hiện

| Bước | Hoạt động | Vai trò chính | Hướng dẫn và kiểm soát | Bằng chứng cần lưu |
|---:|---|---|---|---|
| 1 | Tiếp nhận và xác định phạm vi | Người tiếp nhận | Ghi nhận yêu cầu/sự kiện, xác minh hệ thống, mục tiêu, phạm vi hợp đồng, đầu mối và thông tin tối thiểu. Nếu thiếu thông tin hoặc thẩm quyền thì chưa thực hiện bước rủi ro. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 2 | Rà soát/phân loại | Người thực hiện và người kiểm tra | Kiểm tra cập nhật, quyền chia sẻ, dữ liệu nhạy cảm và mục không được phép chuyển. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 3 | Chuẩn bị gói an toàn | Người thực hiện và người kiểm tra | Làm sạch secret, mã hóa khi cần, kiểm tra file và dùng kênh được duyệt. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 4 | Chuyển giao/kiểm thử | Người thực hiện và người kiểm tra | Walkthrough, xác nhận nhận từng hạng mục và test quyền/runbook/dịch vụ. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 5 | Xác minh, đóng và lưu hồ sơ | Chủ sở hữu quy trình/IT Lead | Người kiểm tra xác nhận kết quả, quyền và phạm vi; ghi thời gian, bằng chứng, quyết định, thông báo và việc tồn. Chỉ đóng khi đủ hồ sơ hoặc có ngoại lệ được duyệt. | Ticket, log, phê duyệt hoặc biên bản tương ứng |

### Lưu đồ

```mermaid
flowchart TD
  A([Bắt đầu]) --> S1["Tiếp nhận và xác định phạm vi"]
  S1 --> D1{"Đủ thông tin và đúng thẩm quyền?"}
  D1 -- Không --> F1[/"Bổ sung thông tin hoặc xin phê duyệt"/]
  F1 --> S1
  D1 -- Có --> S2["Rà soát/phân loại"]
  S2 --> S3["Chuẩn bị gói an toàn"]
  S3 --> D2{"Có rủi ro/ngoại lệ cần xử lý?"}
  D2 -- Có --> S4["Chuyển giao/kiểm thử"]
  D2 -- Không --> S5["Xác minh, đóng và lưu hồ sơ"]
  S4 --> S5
  S5 --> D3{"Kết quả đạt, bằng chứng đủ?"}
  D3 -- Không --> R[/"Khắc phục hoặc mở lại công việc"/]
  R --> S3
  D3 -- Có --> Z([Kết thúc])
```

### Biểu mẫu và hồ sơ

- FR-QTCS02-01: Phiếu yêu cầu/checklist khởi tạo.
- FR-QTCS02-02: Hồ sơ đánh giá, phê duyệt hoặc xác minh.
- FR-QTCS02-03: Nhật ký thực hiện/biên bản/báo cáo.
- FR-QTCS02-04: Xác nhận hoàn tất và theo dõi việc tồn.

*Mã biểu mẫu là mã đề xuất; khi ban hành cần đưa vào danh mục tài liệu, xác định chủ sở hữu, nơi lưu, quyền truy cập và thời hạn lưu giữ.*

### KPI và giám sát

- Tỷ lệ hồ sơ có đủ thông tin đầu vào và phê duyệt.
- Tỷ lệ bước/công việc hoàn thành đúng hạn theo quy trình hoặc hợp đồng.
- Số lỗi, ngoại lệ, sự cố hoặc hồ sơ phải làm lại.
- Tỷ lệ hành động khắc phục đóng đúng hạn.

Chủ sở hữu quy trình phải xác định nguồn dữ liệu, công thức, chu kỳ đo và ngưỡng cảnh báo trước khi áp dụng.

### Ngoại lệ và an toàn thông tin

Walkthrough, xác nhận nhận từng hạng mục và test quyền/runbook/dịch vụ.

- Không thao tác ngoài phạm vi hợp đồng/ủy quyền; khi thiếu quyền hoặc phê duyệt phải tạm dừng bước có rủi ro.
- Không ghi mật khẩu, API key, token, khóa riêng hoặc mã khôi phục dạng rõ trong ticket, README, email thường hay tài liệu bàn giao.
- Thay đổi hệ thống phải theo QT-IT-13; nghi ngờ sự cố ATTT phải theo QT-ATTT-04; ngoại lệ phải theo QT-ISMS-04.
- Mọi ngoại lệ phải có lý do, đánh giá rủi ro, biện pháp bù trừ, người phê duyệt, owner và hạn hết hiệu lực.

### Phụ lục cần cấu hình theo khách hàng

| Trường | Nội dung xác nhận |
|---|---|
| Khách hàng/mã hợp đồng | Theo hợp đồng đang hiệu lực |
| Phạm vi hệ thống/dịch vụ | Hệ thống, tenant, site, tài sản và loại dịch vụ |
| SLA/lịch hỗ trợ | Theo hợp đồng/phụ lục, không dùng mặc định chung |
| Đầu mối yêu cầu/phê duyệt | Chức danh, kênh liên hệ và người thay thế |
| Quyền/kênh kỹ thuật | Phạm vi ủy quyền, MFA, VPN, thời hạn |
| Dữ liệu/lưu giữ | Phân loại, nơi lưu, thời hạn, trả/xóa |
| Thông báo sự cố | Kênh, người nhận và thời hạn |
| Ngoại lệ/rủi ro tồn dư | Mã hồ sơ, phê duyệt, bù trừ, ngày hết hạn |

**Trạng thái:** Dự thảo v0.1 — chờ rà soát, thử nghiệm và phê duyệt. Mapping ISO chỉ mang tính định hướng; cần xác nhận theo phạm vi ISMS, đánh giá rủi ro và SoA.

---

## QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng

**Mục đích:** Ngăn quyền và dữ liệu khách hàng tồn ngoài mục đích/thời hạn, đồng thời giữ dữ liệu có nghĩa vụ lưu hợp lệ.

**Kích hoạt:** Khi có yêu cầu/sự kiện thuộc phạm vi, khi có thay đổi đáng kể hoặc theo chu kỳ được quy định.

**Phạm vi:** Mstar và hoạt động IT Outsourcing trong phạm vi hợp đồng/ủy quyền. Phụ lục từng khách hàng phải xác định hệ thống, SLA, đầu mối, quyền truy cập, retention, thông báo và yêu cầu phục hồi riêng.

**Vai trò:** Người yêu cầu/đầu mối khách hàng; người thực hiện; người kiểm tra/chủ sở hữu hệ thống; chủ sở hữu quy trình; IT Lead; người phê duyệt theo ma trận thẩm quyền. Người thực hiện không tự phê duyệt rủi ro trọng yếu do chính mình tạo ra.

**Đầu vào:** Yêu cầu/ticket; hợp đồng/phụ lục; danh mục hệ thống/tài sản; quyền được ủy quyền; quy trình liên quan; dữ liệu/bằng chứng hiện có.

**Đầu ra:** Hồ sơ xử lý; kết quả đã xác minh; phê duyệt; ticket/biên bản đóng; việc tồn có owner và hạn.

### Trình tự thực hiện

| Bước | Hoạt động | Vai trò chính | Hướng dẫn và kiểm soát | Bằng chứng cần lưu |
|---:|---|---|---|---|
| 1 | Tiếp nhận và xác định phạm vi | Người tiếp nhận | Ghi nhận yêu cầu/sự kiện, xác minh hệ thống, mục tiêu, phạm vi hợp đồng, đầu mối và thông tin tối thiểu. Nếu thiếu thông tin hoặc thẩm quyền thì chưa thực hiện bước rủi ro. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 2 | Quyết định trả/xóa/giữ | Người thực hiện và người kiểm tra | Đối chiếu hợp đồng/pháp luật; xác định người phê duyệt, phạm vi và hạn. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 3 | Thu hồi quyền | Người thực hiện và người kiểm tra | Khóa tài khoản/session/token/key và quyền nhà cung cấp; kiểm tra tài khoản phụ thuộc. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 4 | Trả/xóa/giữ | Người thực hiện và người kiểm tra | Trả qua kênh an toàn hoặc xóa phù hợp; cô lập dữ liệu phải giữ và ghi căn cứ/hạn. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 5 | Xác minh, đóng và lưu hồ sơ | Chủ sở hữu quy trình/IT Lead | Người kiểm tra xác nhận kết quả, quyền và phạm vi; ghi thời gian, bằng chứng, quyết định, thông báo và việc tồn. Chỉ đóng khi đủ hồ sơ hoặc có ngoại lệ được duyệt. | Ticket, log, phê duyệt hoặc biên bản tương ứng |

### Lưu đồ

```mermaid
flowchart TD
  A([Bắt đầu]) --> S1["Tiếp nhận và xác định phạm vi"]
  S1 --> D1{"Đủ thông tin và đúng thẩm quyền?"}
  D1 -- Không --> F1[/"Bổ sung thông tin hoặc xin phê duyệt"/]
  F1 --> S1
  D1 -- Có --> S2["Quyết định trả/xóa/giữ"]
  S2 --> S3["Thu hồi quyền"]
  S3 --> D2{"Có rủi ro/ngoại lệ cần xử lý?"}
  D2 -- Có --> S4["Trả/xóa/giữ"]
  D2 -- Không --> S5["Xác minh, đóng và lưu hồ sơ"]
  S4 --> S5
  S5 --> D3{"Kết quả đạt, bằng chứng đủ?"}
  D3 -- Không --> R[/"Khắc phục hoặc mở lại công việc"/]
  R --> S3
  D3 -- Có --> Z([Kết thúc])
```

### Biểu mẫu và hồ sơ

- FR-QTCS03-01: Phiếu yêu cầu/checklist khởi tạo.
- FR-QTCS03-02: Hồ sơ đánh giá, phê duyệt hoặc xác minh.
- FR-QTCS03-03: Nhật ký thực hiện/biên bản/báo cáo.
- FR-QTCS03-04: Xác nhận hoàn tất và theo dõi việc tồn.

*Mã biểu mẫu là mã đề xuất; khi ban hành cần đưa vào danh mục tài liệu, xác định chủ sở hữu, nơi lưu, quyền truy cập và thời hạn lưu giữ.*

### KPI và giám sát

- Tỷ lệ hồ sơ có đủ thông tin đầu vào và phê duyệt.
- Tỷ lệ bước/công việc hoàn thành đúng hạn theo quy trình hoặc hợp đồng.
- Số lỗi, ngoại lệ, sự cố hoặc hồ sơ phải làm lại.
- Tỷ lệ hành động khắc phục đóng đúng hạn.

Chủ sở hữu quy trình phải xác định nguồn dữ liệu, công thức, chu kỳ đo và ngưỡng cảnh báo trước khi áp dụng.

### Ngoại lệ và an toàn thông tin

Trả qua kênh an toàn hoặc xóa phù hợp; cô lập dữ liệu phải giữ và ghi căn cứ/hạn.

- Không thao tác ngoài phạm vi hợp đồng/ủy quyền; khi thiếu quyền hoặc phê duyệt phải tạm dừng bước có rủi ro.
- Không ghi mật khẩu, API key, token, khóa riêng hoặc mã khôi phục dạng rõ trong ticket, README, email thường hay tài liệu bàn giao.
- Thay đổi hệ thống phải theo QT-IT-13; nghi ngờ sự cố ATTT phải theo QT-ATTT-04; ngoại lệ phải theo QT-ISMS-04.
- Mọi ngoại lệ phải có lý do, đánh giá rủi ro, biện pháp bù trừ, người phê duyệt, owner và hạn hết hiệu lực.

### Phụ lục cần cấu hình theo khách hàng

| Trường | Nội dung xác nhận |
|---|---|
| Khách hàng/mã hợp đồng | Theo hợp đồng đang hiệu lực |
| Phạm vi hệ thống/dịch vụ | Hệ thống, tenant, site, tài sản và loại dịch vụ |
| SLA/lịch hỗ trợ | Theo hợp đồng/phụ lục, không dùng mặc định chung |
| Đầu mối yêu cầu/phê duyệt | Chức danh, kênh liên hệ và người thay thế |
| Quyền/kênh kỹ thuật | Phạm vi ủy quyền, MFA, VPN, thời hạn |
| Dữ liệu/lưu giữ | Phân loại, nơi lưu, thời hạn, trả/xóa |
| Thông báo sự cố | Kênh, người nhận và thời hạn |
| Ngoại lệ/rủi ro tồn dư | Mã hồ sơ, phê duyệt, bù trừ, ngày hết hạn |

**Trạng thái:** Dự thảo v0.1 — chờ rà soát, thử nghiệm và phê duyệt. Mapping ISO chỉ mang tính định hướng; cần xác nhận theo phạm vi ISMS, đánh giá rủi ro và SoA.

---

## QT-QL-01 — Quản lý KPI và cải tiến dịch vụ

**Mục đích:** Chuẩn hóa KPI, nguồn dữ liệu, báo cáo, phân tích nguyên nhân và hành động cải tiến dịch vụ.

**Kích hoạt:** Khi có yêu cầu/sự kiện thuộc phạm vi, khi có thay đổi đáng kể hoặc theo chu kỳ được quy định.

**Phạm vi:** Mstar và hoạt động IT Outsourcing trong phạm vi hợp đồng/ủy quyền. Phụ lục từng khách hàng phải xác định hệ thống, SLA, đầu mối, quyền truy cập, retention, thông báo và yêu cầu phục hồi riêng.

**Vai trò:** Người yêu cầu/đầu mối khách hàng; người thực hiện; người kiểm tra/chủ sở hữu hệ thống; chủ sở hữu quy trình; IT Lead; người phê duyệt theo ma trận thẩm quyền. Người thực hiện không tự phê duyệt rủi ro trọng yếu do chính mình tạo ra.

**Đầu vào:** Yêu cầu/ticket; hợp đồng/phụ lục; danh mục hệ thống/tài sản; quyền được ủy quyền; quy trình liên quan; dữ liệu/bằng chứng hiện có.

**Đầu ra:** Hồ sơ xử lý; kết quả đã xác minh; phê duyệt; ticket/biên bản đóng; việc tồn có owner và hạn.

### Trình tự thực hiện

| Bước | Hoạt động | Vai trò chính | Hướng dẫn và kiểm soát | Bằng chứng cần lưu |
|---:|---|---|---|---|
| 1 | Tiếp nhận và xác định phạm vi | Người tiếp nhận | Ghi nhận yêu cầu/sự kiện, xác minh hệ thống, mục tiêu, phạm vi hợp đồng, đầu mối và thông tin tối thiểu. Nếu thiếu thông tin hoặc thẩm quyền thì chưa thực hiện bước rủi ro. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 2 | Thu thập/kiểm tra | Người thực hiện và người kiểm tra | Lấy dữ liệu nguồn được duyệt; kiểm tra trùng, thiếu, timestamp và quyền truy cập. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 3 | Tính toán/phân tích | Người thực hiện và người kiểm tra | Tính nhất quán; phân tích mục tiêu, xu hướng, dịch vụ và nguyên nhân. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 4 | Xác minh/báo cáo | Người thực hiện và người kiểm tra | Đối chiếu ticket gốc, xác minh ngoại lệ và phê duyệt trước khi phát hành. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 5 | Xác minh, đóng và lưu hồ sơ | Chủ sở hữu quy trình/IT Lead | Người kiểm tra xác nhận kết quả, quyền và phạm vi; ghi thời gian, bằng chứng, quyết định, thông báo và việc tồn. Chỉ đóng khi đủ hồ sơ hoặc có ngoại lệ được duyệt. | Ticket, log, phê duyệt hoặc biên bản tương ứng |

### Lưu đồ

```mermaid
flowchart TD
  A([Bắt đầu]) --> S1["Tiếp nhận và xác định phạm vi"]
  S1 --> D1{"Đủ thông tin và đúng thẩm quyền?"}
  D1 -- Không --> F1[/"Bổ sung thông tin hoặc xin phê duyệt"/]
  F1 --> S1
  D1 -- Có --> S2["Thu thập/kiểm tra"]
  S2 --> S3["Tính toán/phân tích"]
  S3 --> D2{"Có rủi ro/ngoại lệ cần xử lý?"}
  D2 -- Có --> S4["Xác minh/báo cáo"]
  D2 -- Không --> S5["Xác minh, đóng và lưu hồ sơ"]
  S4 --> S5
  S5 --> D3{"Kết quả đạt, bằng chứng đủ?"}
  D3 -- Không --> R[/"Khắc phục hoặc mở lại công việc"/]
  R --> S3
  D3 -- Có --> Z([Kết thúc])
```

### Biểu mẫu và hồ sơ

- FR-QTQL01-01: Phiếu yêu cầu/checklist khởi tạo.
- FR-QTQL01-02: Hồ sơ đánh giá, phê duyệt hoặc xác minh.
- FR-QTQL01-03: Nhật ký thực hiện/biên bản/báo cáo.
- FR-QTQL01-04: Xác nhận hoàn tất và theo dõi việc tồn.

*Mã biểu mẫu là mã đề xuất; khi ban hành cần đưa vào danh mục tài liệu, xác định chủ sở hữu, nơi lưu, quyền truy cập và thời hạn lưu giữ.*

### KPI và giám sát

- Tỷ lệ hồ sơ có đủ thông tin đầu vào và phê duyệt.
- Tỷ lệ bước/công việc hoàn thành đúng hạn theo quy trình hoặc hợp đồng.
- Số lỗi, ngoại lệ, sự cố hoặc hồ sơ phải làm lại.
- Tỷ lệ hành động khắc phục đóng đúng hạn.

Chủ sở hữu quy trình phải xác định nguồn dữ liệu, công thức, chu kỳ đo và ngưỡng cảnh báo trước khi áp dụng.

### Ngoại lệ và an toàn thông tin

Đối chiếu ticket gốc, xác minh ngoại lệ và phê duyệt trước khi phát hành.

- Không thao tác ngoài phạm vi hợp đồng/ủy quyền; khi thiếu quyền hoặc phê duyệt phải tạm dừng bước có rủi ro.
- Không ghi mật khẩu, API key, token, khóa riêng hoặc mã khôi phục dạng rõ trong ticket, README, email thường hay tài liệu bàn giao.
- Thay đổi hệ thống phải theo QT-IT-13; nghi ngờ sự cố ATTT phải theo QT-ATTT-04; ngoại lệ phải theo QT-ISMS-04.
- Mọi ngoại lệ phải có lý do, đánh giá rủi ro, biện pháp bù trừ, người phê duyệt, owner và hạn hết hiệu lực.

### Phụ lục cần cấu hình theo khách hàng

| Trường | Nội dung xác nhận |
|---|---|
| Khách hàng/mã hợp đồng | Theo hợp đồng đang hiệu lực |
| Phạm vi hệ thống/dịch vụ | Hệ thống, tenant, site, tài sản và loại dịch vụ |
| SLA/lịch hỗ trợ | Theo hợp đồng/phụ lục, không dùng mặc định chung |
| Đầu mối yêu cầu/phê duyệt | Chức danh, kênh liên hệ và người thay thế |
| Quyền/kênh kỹ thuật | Phạm vi ủy quyền, MFA, VPN, thời hạn |
| Dữ liệu/lưu giữ | Phân loại, nơi lưu, thời hạn, trả/xóa |
| Thông báo sự cố | Kênh, người nhận và thời hạn |
| Ngoại lệ/rủi ro tồn dư | Mã hồ sơ, phê duyệt, bù trừ, ngày hết hạn |

**Trạng thái:** Dự thảo v0.1 — chờ rà soát, thử nghiệm và phê duyệt. Mapping ISO chỉ mang tính định hướng; cần xác nhận theo phạm vi ISMS, đánh giá rủi ro và SoA.
