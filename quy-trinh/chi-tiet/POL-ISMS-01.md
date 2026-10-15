# POL-ISMS-01 — CHÍNH SÁCH AN TOÀN THÔNG TIN TỔNG THỂ

> **Trạng thái:** Dự thảo nâng cấp v0.2; chỉ có hiệu lực sau khi Ban Giám đốc/người được ủy quyền phê duyệt.  
> **Chủ sở hữu:** ISMS Owner / IT Lead.  
> **Phạm vi:** Hoạt động Mstar và dịch vụ IT Outsourcing trong phạm vi được xác định; phạm vi khách hàng cụ thể được quy định tại hợp đồng/phụ lục.

## 1. Cam kết của lãnh đạo

Mstar cam kết bảo vệ tính bí mật, toàn vẹn và sẵn sàng của thông tin thuộc phạm vi quản lý; đáp ứng nghĩa vụ pháp lý, hợp đồng và yêu cầu khách hàng đã được xác minh; quản lý rủi ro theo mức độ; và cải tiến hiệu lực các kiểm soát an toàn thông tin.

Lãnh đạo có trách nhiệm:
- Phê duyệt phạm vi ISMS, mục tiêu, chính sách, nguồn lực và mức chấp nhận rủi ro.
- Chỉ định người chịu trách nhiệm, quyền quyết định và cơ chế báo cáo.
- Yêu cầu các đơn vị tuân thủ chính sách và báo cáo sai lệch/sự cố.
- Xem xét kết quả rủi ro, sự cố, audit, KPI, CAPA và thay đổi bối cảnh.
- Không xem việc ban hành tài liệu là bằng chứng đủ để kết luận kiểm soát đã vận hành.

## 2. Mục đích

Thiết lập nguyên tắc bắt buộc cho việc quản lý thông tin, tài sản, danh tính, quyền truy cập, vận hành hệ thống, nhà cung cấp, sự cố, backup/khôi phục, hồ sơ và tuân thủ. Chính sách này là tài liệu nền; quy trình chuyên biệt, phụ lục khách hàng và hướng dẫn kỹ thuật cụ thể hóa cách thực hiện.

## 3. Phạm vi áp dụng

Áp dụng cho:
- Nhân viên, quản lý, cộng tác viên, nhà thầu và bên thứ ba được cấp quyền truy cập thông tin/hệ thống thuộc phạm vi.
- Thiết bị, mạng, ứng dụng, cloud tenant, máy chủ, dữ liệu, tài khoản, log, bản sao lưu và hồ sơ vận hành.
- Dịch vụ khách hàng mà Mstar quản lý hoặc được ủy quyền hỗ trợ theo hợp đồng.

Không tự động mở rộng quyền quản lý của Mstar sang hệ thống khách hàng ngoài phạm vi hợp đồng/ủy quyền. Mỗi khách hàng phải có phụ lục xác định hệ thống, SLA, đầu mối, quyền, dữ liệu, thông báo, backup/DR, lưu giữ và kết thúc dịch vụ.

## 4. Nguyên tắc an toàn thông tin

1. **Quyền tối thiểu:** Chỉ cấp quyền cần thiết cho nhiệm vụ, đúng phạm vi và thời hạn.
2. **Định danh cá nhân:** Dùng tài khoản riêng khi khả thi; không chia sẻ tài khoản/mật khẩu.
3. **Phân loại dữ liệu:** Dữ liệu phải có owner, mục đích, phân loại, nơi lưu và quy tắc chia sẻ/lưu/xóa.
4. **Bảo vệ theo vòng đời:** Kiểm soát từ tạo/thu thập đến sử dụng, chia sẻ, lưu giữ, bàn giao và tiêu hủy.
5. **Thay đổi có kiểm soát:** Thay đổi hệ thống cần đánh giá tác động, phê duyệt, kiểm thử và rollback phù hợp.
6. **Ghi nhận và giám sát:** Hành động trọng yếu phải có log/hồ sơ đủ để truy nguyên; log phải được bảo vệ.
7. **Ứng cứu kịp thời:** Sự kiện nghi ngờ phải được báo cáo; không chờ chứng minh đầy đủ mới kích hoạt đánh giá sự cố.
8. **Khôi phục có kiểm chứng:** Backup thành công không đồng nghĩa restore thành công; phải kiểm thử phục hồi theo mức rủi ro.
9. **Quản lý bên thứ ba:** Quyền, dữ liệu, trách nhiệm, thông báo và kết thúc quan hệ phải được kiểm soát theo hợp đồng.
10. **Cải tiến liên tục:** Sai lệch, sự cố, audit và KPI phải dẫn đến hành động có owner/hạn và kiểm tra hiệu lực.

## 5. Vai trò và trách nhiệm

| Vai trò | Trách nhiệm |
|---|---|
| Ban Giám đốc/người được ủy quyền | Phê duyệt chính sách, phạm vi, mục tiêu, nguồn lực và chấp nhận rủi ro thuộc thẩm quyền. |
| ISMS Owner | Điều phối hệ thống quản lý ATTT, rủi ro, SoA, audit, CAPA và xem xét lãnh đạo. |
| IT Lead/Service Owner | Triển khai kiểm soát kỹ thuật/vận hành, quản lý dịch vụ và báo cáo hiệu lực. |
| Owner tài sản/dữ liệu | Phân loại, xác định nhu cầu truy cập, phê duyệt trong thẩm quyền và rà soát quyền. |
| HR | Quản lý sự kiện nhân sự, cam kết, đào tạo và thông báo cho IT theo kênh chính thức. |
| Sale/Contract Owner/Legal | Rà soát phạm vi, cam kết thương mại, hợp đồng, nghĩa vụ thông báo và yêu cầu pháp lý. |
| Nhân viên/nhà thầu | Tuân thủ chính sách, bảo vệ thông tin, dùng quyền đúng mục đích và báo sự cố/sai lệch. |
| Nhà cung cấp | Tuân thủ yêu cầu bảo mật/hợp đồng và phối hợp theo phạm vi được duyệt. |

Vai trò cụ thể và quyền phê duyệt được xác định trong MA-01 (RACI), MA-02 (RBAC) và ma trận thẩm quyền. Khi không thể tách nhiệm vụ, phải có kiểm soát bù trừ và rà soát độc lập.

## 6. Các chính sách kiểm soát tối thiểu

### 6.1 Tài sản và cấu hình
Mọi tài sản trọng yếu phải có mã, owner, trạng thái và vòng đời được theo dõi. Cấu hình chuẩn phải được phê duyệt, bảo vệ và rà soát. Tài sản mất/hỏng hoặc sai lệch phải có hồ sơ xử lý.

### 6.2 Danh tính và quyền truy cập
Cấp/đổi/thu hồi quyền theo QT-IT-11; quyền đặc quyền theo QT-ATTT-01. Phải có yêu cầu hợp lệ, phê duyệt, MFA khi hỗ trợ, quyền tối thiểu, rà soát định kỳ và bằng chứng thu hồi. Tài khoản khẩn cấp cần kiểm soát riêng và hậu kiểm.

### 6.3 Mật khẩu và bí mật kỹ thuật
Secret phải lưu trong vault/kho được duyệt, không đưa vào mã nguồn, ticket, email/chat thường hoặc tài liệu công khai. Secret bị lộ phải được đánh giá và xoay vòng/thu hồi; xóa nội dung hiển thị không đủ để xử lý.

### 6.4 Phân loại và xử lý dữ liệu
Dữ liệu có owner, mục đích và phân loại. Chia sẻ theo nguyên tắc tối thiểu, dùng kênh được duyệt, xác minh người nhận và tuân thủ hợp đồng. Dữ liệu khách hàng không được dùng cho mục đích khác hoặc đưa vào công cụ bên ngoài nếu chưa được phép.

### 6.5 Vận hành, thay đổi và giám sát
Ticket/Work Item, change, cấu hình, cảnh báo, backup và bảo trì phải có owner, tiêu chí và bằng chứng. Thay đổi sản xuất theo QT-IT-13; giám sát theo QT-IT-15; SLA theo QT-IT-16 và phụ lục khách hàng.

### 6.6 Nhật ký, bằng chứng và lưu hồ sơ
Hệ thống trọng yếu phải ghi log phù hợp; quyền truy cập log bị hạn chế. Hồ sơ được lưu ở kho chính thức, có kiểm soát phiên bản/quyền và retention theo danh mục, hợp đồng, pháp luật đã rà soát. Không xóa hồ sơ đang thuộc điều tra, tranh chấp hoặc legal hold.

### 6.7 Lỗ hổng và thiết bị đầu cuối
Lỗ hổng được xác minh, đánh giá rủi ro, ưu tiên và khắc phục theo kế hoạch đã duyệt. Endpoint phải đáp ứng baseline, cập nhật, bảo vệ malware, mã hóa và kiểm soát quyền phù hợp.

### 6.8 Mạng, nhà cung cấp và dịch vụ khách hàng
Rule firewall/VPN phải có mục đích, phạm vi tối thiểu, phê duyệt, thời hạn và rà soát. Vendor phải được đánh giá theo rủi ro, hợp đồng và quyền truy cập. Dịch vụ khách hàng phải có phụ lục phạm vi/SLA/đầu mối/quyền/dữ liệu/incident/backup/exit.

### 6.9 Sự cố và liên tục hoạt động
Sự kiện nghi ngờ phải được ghi nhận và chuyển QT-ATTT-04. BCP/DR cần xác định dịch vụ trọng yếu, đầu mối, RTO/RPO được phê duyệt và phương án đã diễn tập. Không công bố thời hạn thông báo hoặc mục tiêu khôi phục chung khi chưa xác minh.

### 6.10 Nhân sự và nhận thức
Onboarding, điều chuyển, offboarding, bàn giao kiến thức và đào tạo phải được kiểm soát theo QT-HR-01 đến QT-HR-05. Quyền và tài sản phải được cấp/thu hồi đúng thời điểm; thông tin nhân sự được bảo vệ theo nguyên tắc cần biết.

## 7. Quản lý rủi ro, ngoại lệ và không phù hợp

Rủi ro được quản lý theo QT-ISMS-01 và sổ đăng ký rủi ro; kiểm soát áp dụng/loại trừ được ghi trong SoA đã được rà soát. Ngoại lệ theo QT-ISMS-04 phải có lý do, đánh giá rủi ro, biện pháp bù trừ, người phê duyệt, owner và ngày hết hạn.

Vi phạm, kiểm soát không hiệu lực hoặc hành động quá hạn phải được ghi nhận, phân tích nguyên nhân và xử lý theo CAPA. Không tự chấp nhận rủi ro vượt thẩm quyền; rủi ro tồn dư phải được trình đúng cấp.

## 8. Đào tạo, truyền thông và tuân thủ

Chính sách được công bố qua kho tài liệu chính thức. Nhân sự và bên liên quan được đào tạo theo vai trò, xác nhận đã đọc/hiểu khi yêu cầu và được hướng dẫn cách báo sự cố. Vi phạm được xử lý theo quy định nội bộ và hợp đồng; mọi xử lý phải phù hợp thẩm quyền và pháp luật.

## 9. Theo dõi, đánh giá và xem xét lãnh đạo

ISMS Owner/IT Lead theo dõi rủi ro, KPI, sự cố, audit, CAPA, nhà cung cấp và phản hồi khách hàng. Chương trình kiểm tra nội bộ và xem xét lãnh đạo phải ghi đầu vào, quyết định, owner, hạn và bằng chứng theo QT-ISMS-05/06.

Chính sách được rà soát tối thiểu hằng năm và khi thay đổi đáng kể về tổ chức, công nghệ, dịch vụ, hợp đồng, rủi ro hoặc yêu cầu pháp lý. Phiên bản mới phải được phê duyệt, truyền thông và thu hồi bản cũ khỏi nơi sử dụng.

## 10. Tài liệu liên quan

- QT-ISMS-01 đến QT-ISMS-06: rủi ro, tài liệu, nghĩa vụ, ngoại lệ, audit, xem xét lãnh đạo.
- QT-ATTT-01 đến QT-ATTT-10: kiểm soát kỹ thuật và vận hành ATTT.
- QT-IT-07 đến QT-IT-16: phối hợp và vận hành dịch vụ IT.
- QT-OPS-01 đến QT-OPS-03; QT-BCP-01/02; QT-HR-01 đến QT-HR-05; QT-CS-01 đến QT-CS-03.
- MA-01, MA-02, REG-01 đến REG-04, CAL-01, CHECK-01, KPI-01 và phụ lục khách hàng.

## 11. Phê duyệt

| Vai trò | Họ tên/chức danh | Ngày | Xác nhận |
|---|---|---|---|
| Người soạn | Điền khi trình ký | | |
| Người rà soát | Điền khi trình ký | | |
| Người phê duyệt | Ban Giám đốc/người được ủy quyền | | |

**Tuyên bố:** Chính sách này là dự thảo quản trị. Việc ban hành không tự chứng minh Mstar đã được chứng nhận ISO/IEC 27001. Cần xác định phạm vi ISMS, đánh giá rủi ro, SoA, yêu cầu hợp đồng/pháp lý, kiểm soát thực tế và bằng chứng vận hành trước khi kết luận tuân thủ.
