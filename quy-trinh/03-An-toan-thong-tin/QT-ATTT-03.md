# QT-ATTT-03 — Phân loại và xử lý dữ liệu

> **Trạng thái:** Dự thảo chờ rà soát và phê duyệt  
> **Đơn vị sở hữu:** Data Owner/Chủ sở hữu dịch vụ  
> **Nhóm:** An toan thong tin  
> **Phiên bản:** 0.1 | **Ngày soạn:** 2026-10-14  
> **Phạm vi áp dụng:** Mstar và các hoạt động dịch vụ IT Outsourcing trong phạm vi hợp đồng/ủy quyền. Phụ lục khách hàng có thể bổ sung yêu cầu chặt chẽ hơn.

## 1. Mục đích

Áp dụng biện pháp bảo vệ tương ứng với mức nhạy cảm, quyền sở hữu, nghĩa vụ hợp đồng và vòng đời dữ liệu.

## 2. Phạm vi và thời điểm áp dụng

- **Đối tượng/phạm vi:** Data Owner; IT Lead; người xử lý dữ liệu; khách hàng; pháp chế/tuân thủ khi cần.
- **Kích hoạt quy trình:** Khi tạo/thu thập, truy cập, xuất, truyền, chia sẻ, lưu trữ, lưu giữ hoặc hủy dữ liệu.
- **Không được tự suy diễn thẩm quyền:** Mọi thao tác trong môi trường khách hàng phải nằm trong phạm vi hợp đồng và quyền được ủy quyền.
- **Nguyên tắc dùng chung:** Quy trình lõi áp dụng chung; SLA, đầu mối, hệ thống, quyền, thời hạn lưu giữ và yêu cầu thông báo phải được cấu hình trong phụ lục từng khách hàng.

## 3. Căn cứ và tài liệu liên quan

ISO/IEC 27002: phân loại, ghi nhãn, chuyển giao, xóa và bảo vệ thông tin theo SoA.

Tài liệu liên quan tùy trường hợp: chính sách an toàn thông tin tổng thể; QT-ISMS-01 (rủi ro); QT-ISMS-02 (tài liệu/hồ sơ); QT-ISMS-03 (nghĩa vụ hợp đồng); QT-ISMS-04 (ngoại lệ); QT-IT-08 (ticket); QT-IT-11 (quyền truy cập); QT-IT-13 (thay đổi); QT-ATTT-04 (sự cố); và phụ lục khách hàng liên quan.

> Mapping ISO trong tài liệu là **tham chiếu định hướng ban đầu**, không phải tuyên bố phù hợp/chứng nhận. Phải xác nhận theo phạm vi ISMS, đánh giá rủi ro và Statement of Applicability (SoA).

## 4. Vai trò và trách nhiệm

| Vai trò | Trách nhiệm tối thiểu |
|---|---|
| Người yêu cầu/đầu mối khách hàng | Cung cấp yêu cầu chính xác, xác nhận phạm vi và phê duyệt khi hợp đồng quy định. |
| Người thực hiện | Thực hiện đúng quy trình, trong phạm vi quyền; ghi nhận thao tác và báo cáo rủi ro/sự cố. |
| Người kiểm tra/chủ sở hữu hệ thống | Xác minh tính đúng, an toàn, đầy đủ và phù hợp với yêu cầu nghiệp vụ. |
| Chủ sở hữu quy trình (Data Owner/Chủ sở hữu dịch vụ) | Duy trì quy trình, phân công, xử lý ngoại lệ, theo dõi KPI và cải tiến. |
| IT Lead | Phê duyệt kỹ thuật theo thẩm quyền, quản lý rủi ro kỹ thuật và bảo đảm năng lực vận hành. |
| Ban Giám đốc/người được ủy quyền | Phê duyệt chính sách, cam kết thương mại, nguồn lực hoặc rủi ro thuộc thẩm quyền. |

Người thực hiện không tự phê duyệt thay đổi/rủi ro trọng yếu do chính mình đề xuất nếu việc đó làm mất kiểm soát độc lập.

## 5. Đầu vào và đầu ra

**Đầu vào:** Danh mục dữ liệu; hợp đồng; mục đích xử lý; nghĩa vụ lưu giữ; hệ thống lưu trữ; người được phép.

**Đầu ra tối thiểu:** Phân loại dữ liệu; quy tắc xử lý; ma trận quyền; lịch lưu giữ; bằng chứng chia sẻ/xóa.

## 6. Trình tự thực hiện

| Bước | Hoạt động | Người chịu trách nhiệm | Hướng dẫn và kiểm soát | Hồ sơ/đầu ra |
|---:|---|---|---|---|
| 1 | Nhận diện và xác định chủ sở hữu | Data Owner | Xác định loại dữ liệu, mục đích, nguồn, người sở hữu, dữ liệu cá nhân/nhạy cảm và khách hàng liên quan. | Danh mục dữ liệu |
| 2 | Phân loại và xác định yêu cầu | Data Owner/ATTT | Áp dụng nhãn/phân loại theo chính sách; xác định mức truy cập, mã hóa, logging và yêu cầu hợp đồng. | Mức phân loại và quy tắc |
| 3 | Phê duyệt mục đích và quyền | Data Owner/khách hàng | Xác minh người dùng có mục đích hợp lệ và quyền được phép; hạn chế bản sao và xuất dữ liệu. | Phê duyệt truy cập/xử lý |
| 4 | Lưu trữ/truyền/chia sẻ an toàn | Người xử lý dữ liệu/IT | Dùng nơi lưu và kênh được duyệt; mã hóa khi phù hợp; xác minh người nhận; tránh gửi nhầm hoặc dùng tài khoản cá nhân. | Log chia sẻ/truyền |
| 5 | Rà soát lưu giữ và sử dụng | Data Owner | Kiểm tra quyền, mục đích, bản sao, thời hạn lưu giữ và yêu cầu khách hàng/pháp luật. | Kết quả rà soát |
| 6 | Trả, lưu trữ dài hạn hoặc hủy | Data Owner/IT | Thực hiện theo lịch và phê duyệt; bảo đảm xóa cả bản sao trong phạm vi kiểm soát; ghi nhận ngoại lệ cần giữ. | Biên bản trả/xóa/lưu giữ |

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
  S1["Nhận diện và xác định chủ sở hữu"]
  S2["Phân loại và xác định yêu cầu"]
  S3["Phê duyệt mục đích và quyền"]
  S4["Lưu trữ/truyền/chia sẻ an toàn"]
  S5["Rà soát lưu giữ và sử dụng"]
  S6["Trả, lưu trữ dài hạn hoặc hủy"]
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

FR-DATA-01 Danh mục dữ liệu; FR-DATA-02 Ma trận phân loại; FR-DATA-03 Phiếu chia sẻ/xuất dữ liệu; FR-DATA-04 Biên bản hủy.

Các biểu mẫu trên là mã đề xuất. Khi ban hành chính thức, đưa từng biểu mẫu vào danh mục tài liệu, xác định chủ sở hữu, phiên bản, nơi lưu, quyền truy cập và thời hạn lưu giữ.

## 9. Bằng chứng bắt buộc lưu

- Yêu cầu/ticket và thông tin đầu vào liên quan.
- Phê duyệt của đúng người có thẩm quyền, bao gồm phê duyệt khách hàng khi cần.
- Nhật ký thực hiện, kết quả kiểm tra và thông báo.
- Biên bản bàn giao/nghiệm thu/đóng việc hoặc quyết định ngoại lệ nếu có.
- Các hành động còn tồn, người phụ trách và hạn hoàn thành.

**Kho lưu chính thức:** QT-ATTT-03 phải được cấu hình theo danh mục tài liệu/hồ sơ của Mstar và phụ lục khách hàng. Không lưu hồ sơ nhạy cảm ở kho công khai hoặc repository mã nguồn nếu chưa được phân loại và phê duyệt.

## 10. KPI và giám sát tuân thủ

Tỷ lệ kho dữ liệu trọng yếu có owner/phân loại; yêu cầu chia sẻ có phê duyệt; bản sao quá hạn; hồ sơ xóa đầy đủ.

Chủ sở hữu quy trình xác định nguồn dữ liệu, chu kỳ đo, người kiểm tra và ngưỡng cảnh báo trước khi áp dụng. Không tự thay đổi công thức hoặc loại trừ dữ liệu mà không có căn cứ và lịch sử phê duyệt.

## 11. Ngoại lệ và xử lý không phù hợp

Không xử lý dữ liệu khách hàng ngoài mục đích và phạm vi được ủy quyền. Khi có yêu cầu xóa nhưng nghĩa vụ pháp lý buộc lưu giữ, ghi rõ cơ sở, hạn, quyền truy cập hạn chế và thông báo bên liên quan theo hợp đồng.

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
