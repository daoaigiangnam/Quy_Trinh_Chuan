# Checklist rà soát bộ quy trình chuẩn Mstar

> Mục đích: thống nhất danh mục, mục đích sử dụng và tiêu chí rà soát trước khi soạn chi tiết từng quy trình. Đây là danh mục đề xuất; trạng thái phê duyệt được ghi nhận trong file Excel checklist.

## Cách sử dụng

- Rà soát từng quy trình trong file Excel checklist.
- Chọn trạng thái: Chưa rà soát / Đồng ý / Cần sửa / Gộp với quy trình khác / Chưa áp dụng.
- Ghi rõ yêu cầu chỉnh sửa, quyết định phạm vi và người phụ trách.
- Xác nhận SLA, quyền truy cập, thời gian lưu giữ, thông báo sự cố và yêu cầu riêng theo hợp đồng trong phụ lục từng khách hàng.
- Mapping ISO trong checklist chỉ là định hướng sơ bộ; cần xác nhận theo phạm vi ISMS, đánh giá rủi ro và Statement of Applicability (SoA).

## Các nhóm quy trình

### A. Quản trị ISMS
- **POL-ISMS-01 — Chính sách an toàn thông tin tổng thể:** Đặt nguyên tắc bảo mật, toàn vẹn, sẵn sàng và trách nhiệm bảo vệ thông tin.
- **QT-ISMS-01 — Đánh giá và xử lý rủi ro:** Xác định tài sản, mối đe dọa, điểm yếu, mức rủi ro và phương án xử lý.
- **QT-ISMS-02 — Quản lý tài liệu và hồ sơ:** Kiểm soát phiên bản, phê duyệt, truy cập, lưu giữ và hủy tài liệu/hồ sơ.
- **QT-ISMS-03 — Quản lý nghĩa vụ pháp lý, quy định và hợp đồng:** Theo dõi các cam kết bảo mật, quyền riêng tư và nghĩa vụ dịch vụ.
- **QT-ISMS-04 — Quản lý ngoại lệ an toàn thông tin:** Đánh giá và phê duyệt ngoại lệ có thời hạn, rủi ro tồn dư và kiểm soát bù trừ.
- **QT-ISMS-05 — Kiểm tra tuân thủ và kiểm toán nội bộ:** Xác minh việc thực thi và ghi nhận điểm không phù hợp.
- **QT-ISMS-06 — Xem xét của lãnh đạo và cải tiến:** Đánh giá KPI, rủi ro, sự cố, kiểm toán và quyết định cải tiến.

### B. Vận hành IT Outsourcing
- **QT-IT-07 — Phối hợp Sale và IT:** Xác nhận tính khả thi, nguồn lực, phạm vi và phê duyệt trước khi cam kết.
- **QT-IT-08 — Hỗ trợ khách hàng:** Tiếp nhận, phân loại, xử lý, cập nhật và đóng yêu cầu/sự cố theo SLA.
- **QT-IT-09 — Quản lý công việc Phòng IT:** Phân công, theo dõi tiến độ, ticket và công việc định kỳ/ngoài ticket.
- **QT-IT-10 — Quản lý tài sản CNTT:** Quản lý vòng đời tài sản và phân biệt tài sản Mstar với tài sản khách hàng.
- **QT-IT-12 — Tiếp nhận và bàn giao dịch vụ khách hàng:** Thu thập thông tin hệ thống, quyền hợp lệ, SLA, đầu mối và rủi ro ban đầu.
- **QT-IT-13 — Quản lý thay đổi hệ thống:** Đánh giá tác động, phê duyệt, kiểm thử, triển khai và quay lui.
- **QT-IT-14 — Quản lý cấu hình hệ thống:** Duy trì baseline, lịch sử thay đổi và xử lý sai lệch cấu hình.
- **QT-IT-15 — Giám sát và bảo trì hệ thống:** Theo dõi cảnh báo, hiệu năng, dung lượng và lịch bảo trì.
- **QT-IT-16 — Quản lý SLA và chất lượng dịch vụ:** Theo dõi cam kết, ticket quá hạn, nguyên nhân và hành động khắc phục.

### C. An toàn thông tin
- **QT-ATTT-01 — Quản lý tài khoản đặc quyền:** Kiểm soát và rà soát các tài khoản quản trị trọng yếu.
- **QT-ATTT-02 — Quản lý mật khẩu và bí mật kỹ thuật:** Bảo vệ mật khẩu, token, khóa API, SSH key và chứng thư.
- **QT-ATTT-03 — Phân loại và xử lý dữ liệu:** Quy định cách lưu, truyền, chia sẻ, giữ lại và hủy dữ liệu.
- **QT-ATTT-04 — Quản lý và ứng cứu sự cố ATTT:** Phát hiện, phân loại, cô lập, bảo toàn bằng chứng, thông báo và khôi phục.
- **QT-ATTT-05 — Quản lý nhật ký và bằng chứng:** Kiểm soát nguồn log, quyền xem, lưu giữ, đồng bộ thời gian và bảo toàn bằng chứng.
- **QT-ATTT-06 — Quản lý lỗ hổng và bản vá:** Đánh giá mức độ nghiêm trọng, ưu tiên xử lý và xác minh sau vá.
- **QT-ATTT-07 — Bảo vệ thiết bị đầu cuối:** Quản lý EDR/AV, mã hóa, cập nhật, USB và quyền quản trị cục bộ.
- **QT-ATTT-08 — Quản lý mạng, Firewall và truy cập từ xa:** Kiểm soát VPN, luật firewall, MFA, phân vùng và rà soát quyền.
- **QT-ATTT-09 — Quản lý nhà cung cấp và bên thứ ba:** Đánh giá rủi ro, điều khoản bảo mật, quyền truy cập và kết thúc dịch vụ.
- **QT-ATTT-10 — Kiểm soát dữ liệu khách hàng:** Tách biệt dữ liệu, giới hạn quyền và kiểm soát sao chép/chuyển dữ liệu.

### D. Sao lưu và liên tục kinh doanh
- **QT-OPS-01 — Sao lưu dữ liệu:** Xác định phạm vi, lịch, mã hóa, lưu giữ, giám sát và xử lý lỗi backup.
- **QT-OPS-02 — Kiểm thử khôi phục dữ liệu:** Chứng minh backup khôi phục được và đáp ứng mục tiêu đã thống nhất.
- **QT-BCP-01 — Duy trì hoạt động kinh doanh:** Xác định dịch vụ trọng yếu, RTO/RPO, phương án dự phòng và liên lạc.
- **QT-BCP-02 — Khôi phục sau thảm họa:** Kích hoạt DR, khôi phục dịch vụ, xác minh và hậu kiểm.
- **QT-OPS-03 — Quản lý domain, SSL và chứng thư số:** Theo dõi ngày hết hạn, gia hạn và kiểm tra sau gia hạn.

### E. Nhân sự và bảo toàn thông tin
- **QT-HR-01 — Tiếp nhận nhân sự mới:** Cam kết bảo mật, đào tạo, cấp thiết bị và quyền theo vai trò.
- **QT-HR-02 — Điều chuyển nhân sự:** Thu hồi quyền không còn cần và cấp quyền mới theo nhiệm vụ.
- **QT-HR-03 — Nhân viên nghỉ việc:** Thu hồi quyền/tài sản, bàn giao, xử lý khóa và xác nhận hoàn tất.
- **QT-HR-04 — Bàn giao kiến thức và tài liệu kỹ thuật:** Cập nhật tài liệu, cấu hình, công việc tồn đọng và xác nhận tiếp nhận.
- **QT-HR-05 — Đào tạo và nhận thức ATTT:** Đào tạo theo vai trò, đánh giá hiểu biết và lưu bằng chứng.

### F. Kết thúc hợp đồng và cải tiến
- **QT-CS-01 — Kết thúc hợp đồng dịch vụ khách hàng:** Lập kế hoạch exit, xác định trách nhiệm và bàn giao có kiểm soát.
- **QT-CS-02 — Bàn giao hệ thống cho khách hàng/nhà cung cấp mới:** Bàn giao tài liệu, cấu hình, dữ liệu và quyền hợp lệ.
- **QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng:** Thu hồi tài khoản và xử lý bản sao dữ liệu theo hợp đồng/nghĩa vụ lưu giữ.
- **QT-QL-01 — Quản lý KPI và cải tiến dịch vụ:** Theo dõi chất lượng, phân tích nguyên nhân và quản lý hành động cải tiến.

## Tiêu chí bắt buộc cho mỗi quy trình chi tiết

1. Mã, phiên bản, người soạn/kiểm tra/phê duyệt và lịch sử sửa đổi.
2. Mục đích, phạm vi, điều kiện áp dụng và trường hợp loại trừ.
3. Vai trò và trách nhiệm; xác định người thực hiện, kiểm tra, phê duyệt và được thông báo.
4. Đầu vào, từng bước thao tác, điểm quyết định, nhánh ngoại lệ và đầu ra.
5. Yêu cầu ATTT phù hợp: quyền tối thiểu, MFA, tách biệt khách hàng, bảo vệ bí mật.
6. SLA/thời hạn tham chiếu hợp đồng cụ thể; không mặc định một SLA cho mọi khách hàng.
7. Biểu mẫu, hồ sơ, bằng chứng, nơi lưu, quyền truy cập, thời hạn lưu và cách hủy.
8. KPI/kiểm soát, tần suất kiểm tra và hành động khi không đạt.
9. Lưu đồ nhất quán với nội dung quy trình.
10. Phụ lục riêng khách hàng, thử nghiệm/pilot, phê duyệt và truyền thông trước khi áp dụng.

## Nguyên tắc bảo mật

Không ghi mật khẩu, khóa API, mã khôi phục hoặc dữ liệu nhạy cảm thật vào checklist hay tài liệu mẫu. Các quy trình lõi Mstar dùng chung; SLA, danh mục hệ thống, đầu mối, quyền truy cập, thời gian lưu giữ và điều khoản thông báo được cấu hình trong phụ lục khách hàng.
