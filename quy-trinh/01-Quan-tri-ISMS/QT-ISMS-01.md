# QT-ISMS-01 — Đánh giá và xử lý rủi ro an toàn thông tin

> **Trạng thái:** Dự thảo chờ rà soát và phê duyệt  
> **Đơn vị sở hữu:** Chủ sở hữu ISMS  
> **Nhóm:** Quan tri ISMS  
> **Phiên bản:** 0.1 | **Ngày soạn:** 2026-10-14  
> **Phạm vi áp dụng:** Mstar và các hoạt động dịch vụ IT Outsourcing trong phạm vi hợp đồng/ủy quyền. Phụ lục khách hàng có thể bổ sung yêu cầu chặt chẽ hơn.

## 1. Mục đích

Áp dụng phương pháp nhất quán để nhận diện, phân tích, đánh giá, xử lý và chấp nhận rủi ro ATTT đối với hệ thống, dịch vụ, dữ liệu và hoạt động Mstar.

## 2. Phạm vi và thời điểm áp dụng

- **Đối tượng/phạm vi:** Chủ sở hữu ISMS; IT Lead; chủ sở hữu tài sản/dịch vụ; đầu mối khách hàng khi liên quan; Ban Giám đốc/người có thẩm quyền chấp nhận rủi ro.
- **Kích hoạt quy trình:** Định kỳ theo kế hoạch; trước dịch vụ/hệ thống mới; khi có thay đổi trọng yếu, sự cố, phát hiện kiểm toán hoặc thay đổi nghĩa vụ khách hàng.
- **Không được tự suy diễn thẩm quyền:** Mọi thao tác trong môi trường khách hàng phải nằm trong phạm vi hợp đồng và quyền được ủy quyền.
- **Nguyên tắc dùng chung:** Quy trình lõi áp dụng chung; SLA, đầu mối, hệ thống, quyền, thời hạn lưu giữ và yêu cầu thông báo phải được cấu hình trong phụ lục từng khách hàng.

## 3. Căn cứ và tài liệu liên quan

ISO/IEC 27001:2022 điều khoản 6.1.2, 6.1.3, 8.2–8.3; Annex A theo SoA.

Tài liệu liên quan tùy trường hợp: chính sách an toàn thông tin tổng thể; QT-ISMS-01 (rủi ro); QT-ISMS-02 (tài liệu/hồ sơ); QT-ISMS-03 (nghĩa vụ hợp đồng); QT-ISMS-04 (ngoại lệ); QT-IT-08 (ticket); QT-IT-11 (quyền truy cập); QT-IT-13 (thay đổi); QT-ATTT-04 (sự cố); và phụ lục khách hàng liên quan.

> Mapping ISO trong tài liệu là **tham chiếu định hướng ban đầu**, không phải tuyên bố phù hợp/chứng nhận. Phải xác nhận theo phạm vi ISMS, đánh giá rủi ro và Statement of Applicability (SoA).

## 4. Vai trò và trách nhiệm

| Vai trò | Trách nhiệm tối thiểu |
|---|---|
| Người yêu cầu/đầu mối khách hàng | Cung cấp yêu cầu chính xác, xác nhận phạm vi và phê duyệt khi hợp đồng quy định. |
| Người thực hiện | Thực hiện đúng quy trình, trong phạm vi quyền; ghi nhận thao tác và báo cáo rủi ro/sự cố. |
| Người kiểm tra/chủ sở hữu hệ thống | Xác minh tính đúng, an toàn, đầy đủ và phù hợp với yêu cầu nghiệp vụ. |
| Chủ sở hữu quy trình (Chủ sở hữu ISMS) | Duy trì quy trình, phân công, xử lý ngoại lệ, theo dõi KPI và cải tiến. |
| IT Lead | Phê duyệt kỹ thuật theo thẩm quyền, quản lý rủi ro kỹ thuật và bảo đảm năng lực vận hành. |
| Ban Giám đốc/người được ủy quyền | Phê duyệt chính sách, cam kết thương mại, nguồn lực hoặc rủi ro thuộc thẩm quyền. |

Người thực hiện không tự phê duyệt thay đổi/rủi ro trọng yếu do chính mình đề xuất nếu việc đó làm mất kiểm soát độc lập.

## 5. Đầu vào và đầu ra

**Đầu vào:** Danh mục tài sản/dữ liệu; sơ đồ hệ thống; yêu cầu pháp lý/hợp đồng; sự cố; lỗ hổng; biện pháp kiểm soát hiện hữu.

**Đầu ra tối thiểu:** Phương pháp và tiêu chí rủi ro; sổ đăng ký rủi ro; kế hoạch xử lý; rủi ro tồn dư được chấp nhận; đầu vào cho SoA.

## 6. Trình tự thực hiện

| Bước | Hoạt động | Người chịu trách nhiệm | Hướng dẫn và kiểm soát | Hồ sơ/đầu ra |
|---:|---|---|---|---|
| 1 | Xác định phạm vi đánh giá | Chủ sở hữu ISMS/IT Lead | Chốt dịch vụ, tài sản, dữ liệu, quy trình, bên liên quan, ranh giới hệ thống và tiêu chí tác động. | Phạm vi và tiêu chí |
| 2 | Nhận diện rủi ro | Chủ sở hữu tài sản/dịch vụ | Xác định tài sản, mối đe dọa, lỗ hổng, sự kiện rủi ro, nguyên nhân và hậu quả về bảo mật/vận hành/hợp đồng. | Danh sách kịch bản rủi ro |
| 3 | Phân tích và chấm điểm | Nhóm đánh giá rủi ro | Ước lượng khả năng xảy ra và tác động theo thang điểm đã phê duyệt; ghi rõ căn cứ và kiểm soát đang có. | Điểm rủi ro vốn có/hiện tại |
| 4 | Đánh giá và ưu tiên | Chủ sở hữu ISMS | So sánh với tiêu chí chấp nhận; xác định mức cần xử lý, người chịu trách nhiệm và hạn xử lý. | Sổ đăng ký rủi ro đã xếp hạng |
| 5 | Chọn phương án xử lý | Chủ sở hữu rủi ro/IT Lead | Chọn giảm thiểu, tránh, chuyển giao hoặc chấp nhận; xác định kiểm soát, chi phí, thời hạn và rủi ro tồn dư. | Kế hoạch xử lý rủi ro |
| 6 | Phê duyệt, theo dõi và rà soát | Người có thẩm quyền/Chủ sở hữu ISMS | Phê duyệt phương án và rủi ro tồn dư theo thẩm quyền; cập nhật tiến độ, kiểm tra hiệu lực và đánh giá lại khi thay đổi. | Quyết định chấp nhận và hồ sơ theo dõi |

### Quy tắc vận hành chung

1. Ghi nhận yêu cầu/hoạt động trên hệ thống quản lý công việc được Mstar phê duyệt (ví dụ Bitrix24/Ticket) khi phù hợp.
2. Xác minh danh tính, thẩm quyền, phạm vi và mức độ tác động trước khi thao tác.
3. Không ghi mật khẩu, token, khóa API, mã khôi phục hoặc secret dạng rõ trong ticket, README, email thông thường hay tài liệu bàn giao.
4. Nếu có thay đổi cấu hình, áp dụng quy trình quản lý thay đổi; nếu nghi ngờ sự cố ATTT, kích hoạt quy trình ứng cứu sự cố.
5. Nếu thiếu dữ liệu, quyền hoặc phê duyệt, tạm dừng bước rủi ro, ghi nhận blocker và yêu cầu bổ sung; không tự ý mở rộng phạm vi.
6. Kết thúc khi kết quả được xác minh, hồ sơ đủ và các việc tồn được giao owner/hạn rõ ràng.

## 7. Lưu đồ quy trình

```mermaid
flowchart TD
  S1["Xác định phạm vi đánh giá"]
  S2["Nhận diện rủi ro"]
  S3["Phân tích và chấm điểm"]
  S4["Đánh giá và ưu tiên"]
  S5["Chọn phương án xử lý"]
  S6["Phê duyệt, theo dõi và rà soát"]
  START([Bắt đầu]) --> S1
  S1 --> S2
  S2 --> D1{"Đủ thông tin và đúng thẩm quyền?"}
  D1 -- Không --> FIX[/Bổ sung thông tin hoặc xin phê duyệt/]
  FIX --> S2
  D1 -- Có --> S3
  S3 --> S4
  S4 --> S5
  S5 --> S6
  S6 --> D2{"Kết quả đạt và hồ sơ đủ?"}
  D2 -- Không --> REWORK[/"Khắc phục, xử lý ngoại lệ hoặc mở lại" /]
  REWORK --> S5
  D2 -- Có --> END([Kết thúc và lưu hồ sơ])
```

Lưu đồ thể hiện luồng chuẩn và các nhánh kiểm tra điều kiện, bổ sung thông tin, khắc phục và đóng hồ sơ. Khi điều chỉnh nội dung quy trình, phải cập nhật lưu đồ đồng thời để tránh sai lệch.

## 8. Biểu mẫu và hồ sơ

FR-RISK-01 Tiêu chí đánh giá; FR-RISK-02 Sổ đăng ký rủi ro; FR-RISK-03 Kế hoạch xử lý; FR-RISK-04 Chấp nhận rủi ro tồn dư.

Các biểu mẫu trên là mã đề xuất. Khi ban hành chính thức, đưa từng biểu mẫu vào danh mục tài liệu, xác định chủ sở hữu, phiên bản, nơi lưu, quyền truy cập và thời hạn lưu giữ.

## 9. Bằng chứng bắt buộc lưu

- Yêu cầu/ticket và thông tin đầu vào liên quan.
- Phê duyệt của đúng người có thẩm quyền, bao gồm phê duyệt khách hàng khi cần.
- Nhật ký thực hiện, kết quả kiểm tra và thông báo.
- Biên bản bàn giao/nghiệm thu/đóng việc hoặc quyết định ngoại lệ nếu có.
- Các hành động còn tồn, người phụ trách và hạn hoàn thành.

**Kho lưu chính thức:** QT-ISMS-01 phải được cấu hình theo danh mục tài liệu/hồ sơ của Mstar và phụ lục khách hàng. Không lưu hồ sơ nhạy cảm ở kho công khai hoặc repository mã nguồn nếu chưa được phân loại và phê duyệt.

## 10. KPI và giám sát tuân thủ

100% rủi ro cao có chủ sở hữu và kế hoạch; không có rủi ro tồn dư vượt ngưỡng được chấp nhận không có phê duyệt; tỷ lệ hành động đúng hạn.

Chủ sở hữu quy trình xác định nguồn dữ liệu, chu kỳ đo, người kiểm tra và ngưỡng cảnh báo trước khi áp dụng. Không tự thay đổi công thức hoặc loại trừ dữ liệu mà không có căn cứ và lịch sử phê duyệt.

## 11. Ngoại lệ và xử lý không phù hợp

Không tự hạ mức rủi ro để đạt mục tiêu KPI. Việc chấp nhận rủi ro phải đúng thẩm quyền; rủi ro liên quan tài sản/dữ liệu khách hàng cần có sự tham gia hoặc chấp thuận của khách hàng khi hợp đồng yêu cầu.

Mọi ngoại lệ phải có lý do, phạm vi, đánh giá rủi ro, biện pháp bù trừ, người phê duyệt, thời hạn hết hiệu lực và kế hoạch đóng theo QT-ISMS-04. Sự cố ATTT phải được ghi nhận và xử lý theo QT-ATTT-04.

## 12. Phụ lục cần cấu hình theo từng khách hàng

| Thông tin | Nội dung cần điền |
|---|---|
| Khách hàng/mã hợp đồng | Điền theo hợp đồng |
| Phạm vi hệ thống/dịch vụ | Liệt kê hệ thống, tenant, site, tài sản và loại dịch vụ |
| SLA/lịch hỗ trợ | Theo hợp đồng/phụ lục, không dùng mặc định chung |
| Đầu mối yêu cầu/phê duyệt | Tên chức danh, kênh liên hệ và người thay thế |
| Quyền truy cập/kênh kỹ thuật | Chỉ định quyền được ủy quyền, MFA, VPN và thời hạn |
| Yêu cầu dữ liệu/lưu giữ | Phân loại, nơi lưu, thời hạn, trả/xóa và ngoại lệ |
| Thông báo sự cố | Kênh, người nhận và thời hạn theo hợp đồng/pháp luật |
| RTO/RPO/backup (nếu liên quan) | Theo thỏa thuận và kết quả kiểm thử |
| Ngoại lệ/rủi ro tồn dư | Ghi mã hồ sơ, phê duyệt, biện pháp bù trừ và hạn |

## 13. Phê duyệt và lịch sử sửa đổi

| Vai trò | Người ký/tên | Ngày | Trạng thái |
|---|---|---|---|
| Người soạn | Chưa phân công | — | Dự thảo |
| Người kiểm tra | IT Lead/chủ sở hữu liên quan | — | Chờ rà soát |
| Người phê duyệt | Theo ma trận thẩm quyền Mstar | — | Chờ phê duyệt |

| Phiên bản | Ngày | Nội dung thay đổi | Người cập nhật |
|---|---|---|---|
| 0.1 | 2026-10-14 | Tạo bản dự thảo chuẩn hóa; cần rà soát với thực tế vận hành, rủi ro, hợp đồng và SoA. | Mstar |

---
**Lưu ý:** Đây là tài liệu dự thảo để xây dựng và rà soát. Chỉ ban hành sau khi Mstar xác định phạm vi, thẩm quyền, bằng chứng vận hành và phê duyệt chính thức.
