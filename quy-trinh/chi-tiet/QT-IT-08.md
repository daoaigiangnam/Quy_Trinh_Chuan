# QT-IT-08 — Hỗ trợ khách hàng

Tài liệu chi tiết được quản lý trong danh mục quy trình Mstar.

## QT-IT-08 — Hỗ trợ khách hàng

**Mục đích:** Tiếp nhận, phân loại, xử lý, cập nhật và đóng yêu cầu theo phạm vi hợp đồng, mức ưu tiên và SLA.

**Kích hoạt:** Khi có yêu cầu/sự kiện thuộc phạm vi, khi có thay đổi đáng kể hoặc theo chu kỳ được quy định.

**Phạm vi:** Mstar và hoạt động IT Outsourcing trong phạm vi hợp đồng/ủy quyền. Phụ lục từng khách hàng phải xác định hệ thống, SLA, đầu mối, quyền truy cập, retention, thông báo và yêu cầu phục hồi riêng.

**Vai trò:** Người yêu cầu/đầu mối khách hàng; người thực hiện; người kiểm tra/chủ sở hữu hệ thống; chủ sở hữu quy trình; IT Lead; người phê duyệt theo ma trận thẩm quyền. Người thực hiện không tự phê duyệt rủi ro trọng yếu do chính mình tạo ra.

**Đầu vào:** Yêu cầu/ticket; hợp đồng/phụ lục; danh mục hệ thống/tài sản; quyền được ủy quyền; quy trình liên quan; dữ liệu/bằng chứng hiện có.

**Đầu ra:** Hồ sơ xử lý; kết quả đã xác minh; phê duyệt; ticket/biên bản đóng; việc tồn có owner và hạn.

### Trình tự thực hiện

| Bước | Hoạt động | Vai trò chính | Hướng dẫn và kiểm soát | Bằng chứng cần lưu |
|---:|---|---|---|---|
| 1 | Tiếp nhận và xác định phạm vi | Người tiếp nhận | Ghi nhận yêu cầu/sự kiện, xác minh khách hàng/hệ thống liên quan, mục tiêu, phạm vi hợp đồng, đầu mối và thông tin tối thiểu. Nếu thiếu thông tin hoặc thẩm quyền thì chưa thực hiện bước rủi ro. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 2 | Phân loại P1–P4 | Người thực hiện và người kiểm tra | Xác nhận phạm vi, tác động, khẩn cấp và SLA theo hợp đồng khách hàng. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 3 | Phân công và kiểm tra quyền | Người thực hiện và người kiểm tra | Gán kỹ thuật viên đủ năng lực; xác minh quyền và phê duyệt cần thiết. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 4 | Chẩn đoán/xử lý | Người thực hiện và người kiểm tra | Thu thập bằng chứng, thao tác được phép; change phải theo QT-IT-13; nghi ATTT chuyển QT-ATTT-04. | Ticket, log, phê duyệt hoặc biên bản tương ứng |
| 5 | Xác minh, đóng và lưu hồ sơ | Chủ sở hữu quy trình/IT Lead | Người kiểm tra xác nhận kết quả, quyền và phạm vi; ghi thời gian, bằng chứng, quyết định, thông báo và việc tồn. Chỉ đóng khi đủ hồ sơ hoặc có ngoại lệ được duyệt. | Ticket, log, phê duyệt hoặc biên bản tương ứng |

### Lưu đồ

```mermaid
flowchart TD
  A([Bắt đầu]) --> S1["Tiếp nhận và xác định phạm vi"]
  S1 --> D1{"Đủ thông tin và đúng thẩm quyền?"}
  D1 -- Không --> F1[/"Bổ sung thông tin hoặc xin phê duyệt"/]
  F1 --> S1
  D1 -- Có --> S2["Phân loại P1–P4"]
  S2 --> S3["Phân công và kiểm tra quyền"]
  S3 --> D2{"Phát hiện rủi ro/ngoại lệ?"}
  D2 -- Có --> RISK[/"Đánh giá, xử lý hoặc xin phê duyệt"/]
  RISK --> S4["Chẩn đoán/xử lý"]
  D2 -- Không --> S4
  S4 --> S5["Xác minh, đóng và lưu hồ sơ"]
  S5 --> D3{"Kết quả đạt, bằng chứng đủ?"}
  D3 -- Không --> R[/"Khắc phục hoặc mở lại công việc"/]
  R --> S3
  D3 -- Có --> Z([Kết thúc])
```

### Biểu mẫu và hồ sơ

- FR-QTIT08-01: Phiếu yêu cầu/checklist khởi tạo.
- FR-QTIT08-02: Hồ sơ đánh giá, phê duyệt hoặc xác minh.
- FR-QTIT08-03: Nhật ký thực hiện/biên bản/báo cáo.
- FR-QTIT08-04: Xác nhận hoàn tất và theo dõi việc tồn.

*Mã biểu mẫu là mã đề xuất; khi ban hành cần đưa vào danh mục tài liệu, xác định chủ sở hữu, nơi lưu, quyền truy cập và thời hạn lưu giữ.*

### KPI và giám sát

- Tỷ lệ hồ sơ có đủ thông tin đầu vào và phê duyệt.
- Tỷ lệ bước/công việc hoàn thành đúng hạn theo quy trình hoặc hợp đồng.
- Số lỗi, ngoại lệ, sự cố hoặc hồ sơ phải làm lại.
- Tỷ lệ hành động khắc phục đóng đúng hạn.

Chủ sở hữu quy trình phải xác định nguồn dữ liệu, công thức, chu kỳ đo và ngưỡng cảnh báo trước khi áp dụng.

### Ngoại lệ và an toàn thông tin

Thu thập bằng chứng, thao tác được phép; change phải theo QT-IT-13; nghi ATTT chuyển QT-ATTT-04.

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

## Bộ biểu mẫu đi kèm

Biểu mẫu trống, trường điền, nhật ký xử lý, phần rà soát/phê duyệt và checklist đóng hồ sơ: [Mở bộ biểu mẫu QT-IT-08](../../bieu-mau/QT-IT-08-Bieu-mau.md).
