# Bộ quy trình chuẩn Mstar

Bộ quy trình chuẩn của Mstar, áp dụng cho hoạt động cung cấp dịch vụ IT Outsourcing cho khách hàng doanh nghiệp. Bộ tài liệu được xây dựng theo định hướng ISO/IEC 27001:2022 và ISO/IEC 27002:2022 về hệ thống quản lý an toàn thông tin.

> **Trạng thái:** Danh mục và checklist đang trong giai đoạn rà soát. Các quy trình chỉ được áp dụng chính thức sau khi được người có thẩm quyền phê duyệt và công bố.

## 1. Mục tiêu

- Chuẩn hóa cách Mstar tiếp nhận, vận hành, hỗ trợ và kết thúc dịch vụ IT Outsourcing.
- Bảo vệ tính bí mật, toàn vẹn và sẵn sàng của thông tin Mstar và thông tin khách hàng.
- Bảo đảm trách nhiệm, quyền truy cập, thay đổi hệ thống, sao lưu, xử lý sự cố và bàn giao đều có kiểm soát.
- Tạo bằng chứng vận hành để kiểm tra nội bộ, đánh giá tuân thủ và cải tiến liên tục.
- Sử dụng quy trình lõi chung, đồng thời cho phép cấu hình phụ lục riêng theo hợp đồng và từng khách hàng.

## 2. Nguyên tắc thiết kế

1. **Quy trình lõi dùng chung:** quy định phương pháp và trách nhiệm tiêu chuẩn của Mstar.
2. **Phụ lục theo khách hàng:** xác định phạm vi hệ thống, SLA, đầu mối, quyền truy cập, RTO/RPO, thời hạn lưu dữ liệu, yêu cầu thông báo sự cố và điều kiện kết thúc hợp đồng.
3. **Có bằng chứng:** mỗi quy trình phải xác định hồ sơ, log, ticket, phê duyệt hoặc biên bản cần lưu.
4. **Quyền tối thiểu:** chỉ cấp quyền cần thiết, đúng mục đích, có phê duyệt và thời hạn phù hợp.
5. **Không lưu bí mật ở dạng rõ:** không ghi mật khẩu, token, khóa API, mã khôi phục hoặc thông tin xác thực nhạy cảm trong README, checklist hay ticket thông thường.
6. **Mapping ISO là sơ bộ:** việc xác định kiểm soát áp dụng chính thức phải dựa trên phạm vi ISMS, đánh giá rủi ro và Statement of Applicability (SoA). Bộ tài liệu này tự thân không chứng minh Mstar đã được chứng nhận ISO.

## 3. Checklist danh mục quy trình

Checklist chi tiết được tổ chức theo các nhóm sau. Trước khi soạn tài liệu đầy đủ, cần xác nhận mục đích, trường hợp áp dụng, phạm vi, đầu ra/bằng chứng, mức ưu tiên và quyết định giữ/gộp/tách từng quy trình.

### A. Quản trị hệ thống quản lý an toàn thông tin (ISMS)

| Mã | Quy trình | Mục đích sử dụng |
|---|---|---|
| POL-ISMS-01 | Chính sách an toàn thông tin tổng thể | Xác lập nguyên tắc, cam kết của lãnh đạo và trách nhiệm bảo vệ thông tin. |
| QT-ISMS-01 | Đánh giá và xử lý rủi ro | Nhận diện, đánh giá, xử lý và theo dõi rủi ro an toàn thông tin. |
| QT-ISMS-02 | Quản lý tài liệu và hồ sơ | Kiểm soát phiên bản, phê duyệt, lưu giữ, truy cập và hủy tài liệu/hồ sơ. |
| QT-ISMS-03 | Quản lý nghĩa vụ pháp lý, quy định và hợp đồng | Theo dõi cam kết pháp lý, bảo mật, quyền riêng tư và nghĩa vụ hợp đồng. |
| QT-ISMS-04 | Quản lý ngoại lệ an toàn thông tin | Kiểm soát ngoại lệ bằng đánh giá rủi ro, phê duyệt, biện pháp bù trừ và thời hạn. |
| QT-ISMS-05 | Kiểm tra tuân thủ và kiểm toán nội bộ | Xác minh việc thực hiện kiểm soát, ghi nhận phát hiện và theo dõi khắc phục. |
| QT-ISMS-06 | Xem xét của lãnh đạo và cải tiến | Đánh giá hiệu lực ISMS, KPI, rủi ro và quyết định cải tiến. |

### B. Vận hành dịch vụ IT Outsourcing

| Mã | Quy trình | Mục đích sử dụng |
|---|---|---|
| QT-IT-07 | Phối hợp Sale và IT | Thẩm định kỹ thuật, nguồn lực, rủi ro và bàn giao trước khi cam kết dịch vụ. |
| QT-IT-08 | Hỗ trợ khách hàng | Tiếp nhận, phân loại, xử lý, cập nhật và đóng yêu cầu theo SLA. |
| QT-IT-09 | Quản lý công việc Phòng IT | Phân công, theo dõi và báo cáo ticket cùng các công việc ngoài ticket. |
| QT-IT-10 | Quản lý tài sản CNTT | Quản lý vòng đời tài sản và phân biệt tài sản Mstar với tài sản khách hàng. |
| QT-IT-12 | Tiếp nhận và bàn giao dịch vụ khách hàng | Thu thập hồ sơ hệ thống, đầu mối, quyền hợp lệ, SLA và rủi ro tồn đọng. |
| QT-IT-13 | Quản lý thay đổi hệ thống | Đánh giá tác động, phê duyệt, kiểm thử, triển khai và quay lui khi cần. |
| QT-IT-14 | Quản lý cấu hình hệ thống | Duy trì cấu hình chuẩn, lịch sử thay đổi và kiểm soát sai lệch. |
| QT-IT-15 | Giám sát và bảo trì hệ thống | Theo dõi cảnh báo, hiệu năng, dung lượng, dịch vụ và lịch bảo trì. |
| QT-IT-16 | Quản lý SLA và chất lượng dịch vụ | Đo lường SLA, ticket quá hạn, chất lượng hỗ trợ và hành động cải tiến. |

### C. An toàn thông tin và bảo vệ dữ liệu

| Mã | Quy trình | Mục đích sử dụng |
|---|---|---|
| QT-IT-11 | Quản lý tài khoản và quyền truy cập | Cấp, thay đổi, rà soát và thu hồi quyền theo nguyên tắc quyền tối thiểu. |
| QT-ATTT-01 | Quản lý tài khoản đặc quyền | Kiểm soát quyền quản trị hệ thống, nền tảng cloud, mạng và cơ sở dữ liệu. |
| QT-ATTT-02 | Quản lý mật khẩu và bí mật kỹ thuật | Quản lý an toàn mật khẩu, API key, token, SSH key và chứng thư. |
| QT-ATTT-03 | Phân loại và xử lý dữ liệu | Xác định cách lưu trữ, truyền, chia sẻ, giữ lại và hủy dữ liệu theo mức nhạy cảm. |
| QT-ATTT-04 | Quản lý và ứng cứu sự cố ATTT | Phát hiện, phân loại, cô lập, thông báo, xử lý và rút kinh nghiệm từ sự cố. |
| QT-ATTT-05 | Quản lý nhật ký và bằng chứng | Bảo đảm khả năng truy nguyên và bảo toàn log/bằng chứng phục vụ điều tra. |
| QT-ATTT-06 | Quản lý lỗ hổng và bản vá | Xếp hạng, khắc phục và xác minh lỗ hổng theo mức rủi ro. |
| QT-ATTT-07 | Bảo vệ thiết bị đầu cuối | Kiểm soát EDR/AV, mã hóa, cập nhật, USB và quyền quản trị thiết bị. |
| QT-ATTT-08 | Quản lý mạng, Firewall và truy cập từ xa | Kiểm soát phân vùng mạng, luật firewall, VPN, MFA và truy cập từ xa. |
| QT-ATTT-09 | Quản lý nhà cung cấp và bên thứ ba | Đánh giá rủi ro, điều khoản bảo mật, quyền truy cập và chấm dứt dịch vụ. |
| QT-ATTT-10 | Kiểm soát dữ liệu khách hàng | Tách biệt dữ liệu, hạn chế truy cập, kiểm soát xuất/chia sẻ và giảm nguy cơ thất thoát. |

### D. Sao lưu, khôi phục và liên tục kinh doanh

| Mã | Quy trình | Mục đích sử dụng |
|---|---|---|
| QT-OPS-01 | Sao lưu dữ liệu | Xác định phạm vi, lịch, nơi lưu, mã hóa, thời hạn giữ và giám sát backup. |
| QT-OPS-02 | Kiểm thử khôi phục dữ liệu | Chứng minh bản sao lưu có thể khôi phục theo mục tiêu đã thống nhất. |
| QT-BCP-01 | Duy trì hoạt động kinh doanh | Xác định dịch vụ trọng yếu, RTO/RPO và phương án duy trì hoạt động. |
| QT-BCP-02 | Khôi phục sau thảm họa | Điều phối khôi phục hạ tầng/dịch vụ và xác nhận hoạt động bình thường trở lại. |
| QT-OPS-03 | Quản lý domain, SSL và chứng thư số | Theo dõi hạn dùng, cảnh báo, gia hạn và kiểm tra sau gia hạn. |

### E. Nhân sự và bảo toàn thông tin

| Mã | Quy trình | Mục đích sử dụng |
|---|---|---|
| QT-HR-01 | Tiếp nhận nhân sự mới | Hoàn tất cam kết, đào tạo, thiết bị và cấp quyền theo vai trò. |
| QT-HR-02 | Điều chuyển nhân sự | Thu hồi quyền không còn cần và cấp quyền mới theo nhiệm vụ. |
| QT-HR-03 | Nhân viên nghỉ việc | Thu hồi quyền, thiết bị, bí mật kỹ thuật và bảo đảm bàn giao tri thức. |
| QT-HR-04 | Bàn giao kiến thức và tài liệu kỹ thuật | Giảm phụ thuộc cá nhân và giúp người thay thế tiếp quản an toàn. |
| QT-HR-05 | Đào tạo và nhận thức an toàn thông tin | Nâng cao nhận thức và lưu bằng chứng đào tạo/đánh giá. |

### F. Kết thúc hợp đồng và cải tiến dịch vụ

| Mã | Quy trình | Mục đích sử dụng |
|---|---|---|
| QT-CS-01 | Kết thúc hợp đồng dịch vụ khách hàng | Điều phối kết thúc dịch vụ, xác nhận việc mở và nghĩa vụ còn lại. |
| QT-CS-02 | Bàn giao hệ thống cho khách hàng/nhà cung cấp mới | Chuyển giao hồ sơ, cấu hình, dữ liệu và quyền hợp lệ có kiểm soát. |
| QT-CS-03 | Thu hồi quyền và xóa dữ liệu sau hợp đồng | Thu hồi truy cập, trả/xóa dữ liệu và xử lý bản sao theo hợp đồng/nghĩa vụ lưu giữ. |
| QT-QL-01 | Quản lý KPI và cải tiến dịch vụ | Đo chất lượng, phân tích xu hướng và theo dõi hành động cải tiến. |

## 4. Tiêu chí bắt buộc khi viết chi tiết một quy trình

Mỗi quy trình hoàn chỉnh cần được rà soát tối thiểu theo checklist sau:

- [ ] Mã tài liệu, phiên bản, ngày hiệu lực, người soạn, người kiểm tra và người phê duyệt.
- [ ] Mục đích và kết quả mong muốn rõ ràng.
- [ ] Phạm vi áp dụng, đối tượng, hệ thống và điều kiện loại trừ.
- [ ] Căn cứ, chính sách và quy trình liên quan.
- [ ] Vai trò và trách nhiệm; phân biệt người yêu cầu, người thực hiện, người kiểm tra và người phê duyệt.
- [ ] Đầu vào và điều kiện bắt đầu.
- [ ] Các bước thực hiện, đầu ra và điều kiện chuyển bước.
- [ ] Nhánh xử lý thiếu thông tin, từ chối, thất bại, khẩn cấp và ngoại lệ.
- [ ] Kiểm soát an toàn thông tin phù hợp: quyền tối thiểu, MFA, phân tách khách hàng và bảo vệ bí mật.
- [ ] SLA/thời hạn tham chiếu đúng hợp đồng và phụ lục khách hàng.
- [ ] Hồ sơ/bằng chứng cần tạo, nơi lưu, quyền truy cập và thời hạn lưu giữ.
- [ ] KPI/tiêu chí hiệu lực và cách kiểm tra.
- [ ] Biểu mẫu đi kèm và hướng dẫn sử dụng.
- [ ] Lưu đồ thống nhất với các bước trong nội dung.
- [ ] Phụ lục cấu hình riêng cho khách hàng.
- [ ] Thử nghiệm quy trình, xử lý góp ý, phê duyệt và truyền thông trước khi áp dụng.

## 5. Thông tin phải xác nhận riêng theo khách hàng

Không mặc định mọi khách hàng có cùng SLA hoặc cùng yêu cầu bảo mật. Khi tiếp nhận mỗi khách hàng, cần xác nhận tối thiểu:

- Hợp đồng, phạm vi dịch vụ và thời hạn.
- Danh sách hệ thống, tài sản, tenant, site và dịch vụ được quản lý.
- SLA, lịch hỗ trợ, mức ưu tiên và cách tính thời gian.
- Đầu mối yêu cầu, người phê duyệt thay đổi và liên lạc khẩn cấp.
- Tài khoản/quyền được phép, MFA, VPN và thời hạn truy cập.
- Phân loại dữ liệu, nơi lưu, quy tắc xuất/chia sẻ và thời hạn lưu giữ.
- Phạm vi backup, RPO/RTO và lịch kiểm thử restore.
- Kênh, thời hạn và người nhận thông báo sự cố.
- Nhà cung cấp/bên thứ ba được phép tham gia.
- Điều kiện bàn giao, thu hồi quyền, trả/xóa dữ liệu khi kết thúc hợp đồng.

## 6. Trạng thái và mức ưu tiên

- **Chưa rà soát:** chưa thống nhất nội dung.
- **Đồng ý:** có thể đưa vào kế hoạch soạn chi tiết.
- **Cần sửa:** phải cập nhật mục đích, phạm vi hoặc nội dung.
- **Gộp với quy trình khác:** tránh trùng lặp và giảm gánh nặng vận hành.
- **Chưa áp dụng:** chỉ dùng khi có căn cứ phạm vi/rủi ro và được người có thẩm quyền chấp thuận.

Ưu tiên đề xuất:
- **P1:** cần có trước hoặc trong giai đoạn đầu vận hành.
- **P2:** cần triển khai để hoàn thiện kiểm soát.
- **P3:** triển khai tùy phạm vi dịch vụ và kết quả đánh giá rủi ro.

## 7. Lộ trình thực hiện

1. Rà soát danh mục và mục đích sử dụng từng quy trình.
2. Xác định phạm vi ISMS, bối cảnh, bên liên quan và phương pháp đánh giá rủi ro.
3. Lập sổ đăng ký rủi ro và Statement of Applicability (SoA).
4. Soạn chính sách và các quy trình ưu tiên P1.
5. Hoàn thiện biểu mẫu, lưu đồ, nơi lưu hồ sơ và phân quyền.
6. Thử nghiệm trên quy trình nội bộ hoặc một khách hàng phù hợp.
7. Đánh giá bằng chứng, khắc phục điểm yếu và phê duyệt áp dụng.
8. Mở rộng triển khai, đào tạo, kiểm toán và cải tiến định kỳ.

## 8. Tài liệu tham khảo

- [ISO/IEC 27001 — Information security management systems](https://www.iso.org/standard/27001)
- [ISO/IEC 27002 — Information security controls](https://www.iso.org/standard/75652.html)

**Lưu ý:** Các tham chiếu ISO trong danh mục chỉ mang tính định hướng ban đầu, không phải tuyên bố mapping chính thức. Cần xác nhận theo tiêu chuẩn được cấp phép, phạm vi ISMS, đánh giá rủi ro và SoA của Mstar.

## 9. Bộ quy trình chi tiết và lưu đồ

Đã tạo các tài liệu Markdown theo từng nhóm. Mỗi quy trình có mục đích, phạm vi, vai trò, các bước thực hiện, lưu đồ Mermaid, biểu mẫu/hồ sơ, KPI, ngoại lệ và các trường cần cấu hình riêng theo khách hàng.

| Nhóm | Nội dung | Liên kết |
|---|---|---|
| A | Quản trị ISMS — chính sách, rủi ro, tài liệu, nghĩa vụ, ngoại lệ, kiểm toán, xem xét lãnh đạo | [Mở nhóm A](quy-trinh/01-Quan-tri-ISMS/README.md) |
| B | Vận hành IT Outsourcing — Sale–IT, hỗ trợ, công việc IT, tài sản, onboarding khách hàng, change, cấu hình, giám sát, SLA | [Mở nhóm B](quy-trinh/02-Van-hanh-IT/README.md) |
| C | An toàn thông tin — IAM, đặc quyền, bí mật kỹ thuật, dữ liệu, incident, log, lỗ hổng, endpoint, network, vendor | [Mở nhóm C](quy-trinh/03-An-toan-thong-tin/README.md) |
| D | Sao lưu/khôi phục/BCP-DR — backup, restore test, BCP, DR, domain/SSL/chứng thư | [Mở nhóm D](quy-trinh/04-Backup-BCP-DR/README.md) |
| E | Nhân sự — onboarding, điều chuyển, nghỉ việc, bàn giao tri thức, đào tạo ATTT | [Mở nhóm E](quy-trinh/05-Nhan-su/README.md) |
| F | Kết thúc hợp đồng và cải tiến — exit, bàn giao nhà cung cấp, thu hồi/xóa dữ liệu, KPI | [Mở nhóm F](quy-trinh/06-Ket-thuc-hop-dong/README.md) |

**Tổng số:** 41 quy trình trong 6 tài liệu nhóm. Lưu đồ được viết bằng Mermaid để GitHub hiển thị trực tiếp.

### Trạng thái kiểm soát tài liệu

Các nội dung hiện là **dự thảo v0.1**, chưa phải quy trình đã ban hành. Trước khi áp dụng cần:
1. Rà soát theo thực tế vận hành Mstar và hợp đồng khách hàng.
2. Xác nhận chủ sở hữu, người kiểm tra, người phê duyệt và nơi lưu hồ sơ.
3. Hoàn tất đánh giá rủi ro và SoA; kiểm tra mapping ISO với bản tiêu chuẩn được cấp phép.
4. Thử nghiệm, sửa lỗi lưu đồ/biểu mẫu, đào tạo và ban hành theo thẩm quyền.
5. Không coi việc có tài liệu là bằng chứng Mstar đã được chứng nhận ISO.

## 10. Tài liệu quy trình theo mã

Để thuận tiện phân công, rà soát và quản lý phiên bản, từng quy trình đã có một file Markdown riêng trong thư mục `quy-trinh/chi-tiet/`.

- [Mở danh mục 41 quy trình chi tiết](quy-trinh/chi-tiet/README.md)
- [Mở thư mục quy trình chi tiết](quy-trinh/chi-tiet/)

Mỗi file riêng chứa nội dung quy trình và lưu đồ Mermaid tương ứng. Các tài liệu nhóm vẫn được duy trì để đọc theo chủ đề.

## 11. Thư viện biểu mẫu đi kèm

Đã bổ sung bộ biểu mẫu cho từng quy trình, gồm các trường cần điền, bảng ghi nhận, phần rà soát/phê duyệt và checklist đóng hồ sơ.

- [Mở thư viện biểu mẫu chuẩn Mstar](bieu-mau/README.md)
- [Mở thư mục biểu mẫu](bieu-mau/)

Các biểu mẫu đang là dự thảo v0.1; cần rà soát, thử nghiệm và phê duyệt trước khi ban hành. SLA, quyền, thời hạn thông báo, lưu giữ và RTO/RPO phải được cấu hình theo hợp đồng từng khách hàng.
