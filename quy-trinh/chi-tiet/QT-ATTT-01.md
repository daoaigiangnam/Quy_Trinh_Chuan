# QT-ATTT-01 — QUẢN LÝ TÀI KHOẢN ĐẶC QUYỀN

> **Trạng thái:** Dự thảo nâng cấp v0.2; cần rà soát, diễn tập và phê duyệt trước khi áp dụng.  
> **Chủ sở hữu:** IT Lead / đầu mối ATTT hoặc BCP được chỉ định.  
> **Liên quan:** QT-ATTT-04, QT-IT-08, QT-IT-11, QT-IT-13, QT-IT-15, QT-ISMS-03/04, REG-01, MA-01, MA-02.

## 1. Kiểm soát tài liệu
| Trường | Nội dung |
|---|---|
| Mã | QT-ATTT-01 |
| Phiên bản | 0.2 — dự thảo nâng cấp |
| Chủ sở hữu | IT Lead / BCP Lead |
| Người rà soát | Owner hệ thống, ATTT, Service Owner và khách hàng khi liên quan |
| Người phê duyệt | Người có thẩm quyền theo cơ chế quản trị |
| Ngày hiệu lực | Điền sau khi phê duyệt |
| Rà soát | Tối thiểu hằng năm, sau diễn tập hoặc sự cố nghiêm trọng |

## 2. Mục đích và phạm vi
Kiểm soát tài khoản có quyền quản trị hệ thống, thay đổi bảo mật, truy cập dữ liệu trọng yếu hoặc ảnh hưởng nhiều người dùng.
Áp dụng cho dịch vụ thuộc Mstar và dịch vụ khách hàng trong phạm vi hợp đồng/ủy quyền. Phụ lục từng khách hàng phải xác định hệ thống, đầu mối, RTO/RPO, thứ tự ưu tiên, kênh thông báo và trách nhiệm quyết định. Không cam kết RTO/RPO chưa được phân tích, phê duyệt và kiểm thử.

## 3. Nguyên tắc bắt buộc
1. An toàn con người và hạn chế thiệt hại được ưu tiên.
2. Chỉ người có thẩm quyền mới kích hoạt kế hoạch hoặc chấp nhận rủi ro trọng yếu.
3. Bảo toàn bằng chứng trước hành động có thể phá hủy khi khả thi; nếu phải hành động ngay, ghi lý do/thời điểm.
4. Bản sao lưu phải được xác minh; không mặc định backup thành công đồng nghĩa restore thành công.
5. RTO/RPO là mục tiêu được duyệt, không phải cam kết chung cho mọi hệ thống.
6. Mọi hành động khẩn cấp phải có nhật ký, người chịu trách nhiệm và hậu kiểm.
7. Khi có dấu hiệu ATTT, phối hợp QT-ATTT-04; không đưa hệ thống chưa an toàn trở lại mạng sản xuất.

## 4. Vai trò
| Vai trò | Trách nhiệm |
|---|---|
| Incident/BCP/DR Lead | Điều phối, duy trì nhật ký, cập nhật tình hình và đề xuất quyết định. |
| Owner hệ thống/dịch vụ | Xác định mức độ trọng yếu, tiêu chí phục hồi và nghiệm thu. |
| Nhóm kỹ thuật | Thực hiện phương án, ghi thao tác, kiểm thử và báo sai lệch. |
| Đầu mối ATTT | Đánh giá an toàn, bảo toàn bằng chứng và kiểm tra trước khi tái kết nối. |
| Ban lãnh đạo/người có thẩm quyền | Kích hoạt, ưu tiên nguồn lực và chấp nhận rủi ro trong thẩm quyền. |
| Đầu mối khách hàng/vendor | Phối hợp, xác nhận quyết định và hỗ trợ theo hợp đồng. |

## 5. Điều kiện kích hoạt/đầu vào
Hồ sơ phải có dấu hiệu sự cố, hệ thống/dịch vụ bị ảnh hưởng, thời điểm, tác động, người báo, mức độ ban đầu, phụ thuộc và phương án liên lạc. Kích hoạt khi gián đoạn vượt ngưỡng đã duyệt, có nguy cơ không đạt RTO/RPO hoặc sự cố ảnh hưởng nhiều dịch vụ/khách hàng. Nếu chưa đủ dữ liệu, ghi giả định và đánh giá lại theo mốc do Incident Lead quyết định.

## 6. Trình tự thực hiện chi tiết

### Bước 1 — Lập danh mục
**Người thực hiện:** Owner hệ thống/đầu mối ATTT/BCP được phân công; người có thẩm quyền phê duyệt các quyết định trọng yếu.

Liệt kê tài khoản admin/root/domain admin/cloud admin/firewall/database/backup và các quyền tương đương; ghi hệ thống, owner, mục đích, người được phép dùng, loại tài khoản, MFA, kho secret, logging và ngày rà soát. Tài khoản không rõ owner phải được điều tra và hạn chế; không xóa ngay khi chưa xác định phụ thuộc.

**Điều kiện đạt:** Có quyết định, kết quả kiểm tra và bằng chứng truy nguyên. **Nếu không đạt:** Ghi sai lệch, giữ trạng thái chưa hoàn tất và chuyển cấp.

### Bước 2 — Phê duyệt nhu cầu
**Người thực hiện:** Owner hệ thống/đầu mối ATTT/BCP được phân công; người có thẩm quyền phê duyệt các quyết định trọng yếu.

Yêu cầu phải có lý do công việc, hệ thống, quyền cụ thể, thời hạn, người dùng và người phê duyệt. Đánh giá có thể dùng quyền thường hoặc elevation theo phiên thay vì cấp quyền admin thường trực. Phê duyệt theo ma trận; người nhận quyền không tự phê duyệt.

**Điều kiện đạt:** Có quyết định, kết quả kiểm tra và bằng chứng truy nguyên. **Nếu không đạt:** Ghi sai lệch, giữ trạng thái chưa hoàn tất và chuyển cấp.

### Bước 3 — Cấp và bảo vệ
**Người thực hiện:** Owner hệ thống/đầu mối ATTT/BCP được phân công; người có thẩm quyền phê duyệt các quyết định trọng yếu.

Dùng tài khoản định danh riêng hoặc giải pháp PAM khi có; bật MFA, logging và cảnh báo. Tách tài khoản thường với tài khoản admin; hạn chế truy cập từ Internet; không dùng chung tài khoản nếu nền tảng cho phép định danh cá nhân. Secret chỉ lưu trong vault được duyệt.

**Điều kiện đạt:** Có quyết định, kết quả kiểm tra và bằng chứng truy nguyên. **Nếu không đạt:** Ghi sai lệch, giữ trạng thái chưa hoàn tất và chuyển cấp.

### Bước 4 — Sử dụng quyền đặc quyền
**Người thực hiện:** Owner hệ thống/đầu mối ATTT/BCP được phân công; người có thẩm quyền phê duyệt các quyết định trọng yếu.

Chỉ dùng cho tác vụ đã được ủy quyền; ghi ticket/change ID, mục đích, hệ thống, thời điểm và kết quả. Với thao tác sản xuất, dữ liệu nhạy cảm hoặc rủi ro cao, cần phê duyệt change/khách hàng tương ứng. Không dùng quyền admin để duyệt email/web thông thường.

**Điều kiện đạt:** Có quyết định, kết quả kiểm tra và bằng chứng truy nguyên. **Nếu không đạt:** Ghi sai lệch, giữ trạng thái chưa hoàn tất và chuyển cấp.

### Bước 5 — Giám sát và cảnh báo
**Người thực hiện:** Owner hệ thống/đầu mối ATTT/BCP được phân công; người có thẩm quyền phê duyệt các quyết định trọng yếu.

Thu thập log đăng nhập, nâng quyền, thay đổi nhóm, tạo tài khoản, thay đổi policy, tắt logging và thao tác nhạy cảm. Rà soát cảnh báo bất thường; mọi lần dùng break-glass phải có hậu kiểm. Nếu nghi bị chiếm, thu hồi phiên/secret và kích hoạt QT-ATTT-04.

**Điều kiện đạt:** Có quyết định, kết quả kiểm tra và bằng chứng truy nguyên. **Nếu không đạt:** Ghi sai lệch, giữ trạng thái chưa hoàn tất và chuyển cấp.

### Bước 6 — Rà soát và thu hồi
**Người thực hiện:** Owner hệ thống/đầu mối ATTT/BCP được phân công; người có thẩm quyền phê duyệt các quyết định trọng yếu.

Định kỳ xác nhận nhu cầu, owner, phạm vi, lần dùng, thời hạn và tài khoản không hoạt động. Thu hồi khi hết nhiệm vụ, nghỉ việc, hết hợp đồng, quyền không còn cần hoặc không được tái xác nhận. Với tài khoản dịch vụ, xác định phụ thuộc trước khi khóa và có kế hoạch chuyển owner.

**Điều kiện đạt:** Có quyết định, kết quả kiểm tra và bằng chứng truy nguyên. **Nếu không đạt:** Ghi sai lệch, giữ trạng thái chưa hoàn tất và chuyển cấp.

### Bước 7 — Kiểm tra độc lập
**Người thực hiện:** Owner hệ thống/đầu mối ATTT/BCP được phân công; người có thẩm quyền phê duyệt các quyết định trọng yếu.

Người rà soát không phải người duy nhất đã cấp quyền phải kiểm tra mẫu log, danh mục, phê duyệt và thu hồi. Sai lệch có owner/hạn/CAPA; không đóng chỉ vì danh mục đã sửa nếu chưa kiểm tra quyền thực tế.

**Điều kiện đạt:** Có quyết định, kết quả kiểm tra và bằng chứng truy nguyên. **Nếu không đạt:** Ghi sai lệch, giữ trạng thái chưa hoàn tất và chuyển cấp.

## 7. Chuyển cấp và ngoại lệ
Chuyển cấp ngay khi hệ thống trọng yếu ngừng hoạt động, backup không đọc được, nghi bản sao lưu bị nhiễm, dữ liệu không nhất quán, mục tiêu phục hồi có nguy cơ không đạt, thiếu quyền/nguồn lực hoặc có nghĩa vụ thông báo khẩn. Ghi thời điểm, tác động, lựa chọn, người quyết định, việc đã làm và mốc cập nhật tiếp theo.

Mọi ngoại lệ về mục tiêu phục hồi, bảo mật, lưu dữ liệu hoặc thời gian gián đoạn phải có đánh giá rủi ro, biện pháp bù trừ, owner, hạn và người chấp nhận. Không dùng ngoại lệ để che giấu việc kế hoạch chưa được kiểm thử.

## 8. Bằng chứng vận hành
| Hồ sơ | Nội dung tối thiểu |
|---|---|
| Đánh giá tác động | Dịch vụ, phụ thuộc, mức độ, RTO/RPO mục tiêu |
| Quyết định kích hoạt | Người quyết định, thời gian, lý do, phạm vi |
| Nhật ký ứng cứu | Mốc thời gian, hành động, kết quả, người làm |
| Bằng chứng backup/restore | Nguồn, điểm khôi phục, kiểm tra tính toàn vẹn |
| Kiểm thử/nghiệm thu | Tiêu chí, kết quả, người xác nhận |
| Thông báo | Người nhận, kênh, thời điểm, nội dung |
| Hậu kiểm/CAPA | Sai lệch, nguyên nhân, owner, hạn, kiểm tra hiệu lực |

Lưu trong kho chính thức, phân quyền theo nhu cầu công việc và thời hạn theo danh mục hồ sơ/hợp đồng. Không đưa bản backup hoặc dữ liệu khách hàng vào repository mã nguồn.

## 9. KPI và giám sát
| KPI | Định nghĩa |
|---|---|
| RTO thực tế so với mục tiêu | Thời gian khôi phục thực tế so với RTO được duyệt |
| RPO thực tế so với mục tiêu | Mức mất dữ liệu thực tế so với RPO được duyệt |
| Tỷ lệ diễn tập đạt | Kịch bản đạt tiêu chí / kịch bản được thực hiện |
| Tỷ lệ backup phục hồi thành công | Bài test restore đạt / bài test restore thực hiện |
| Hành động sau diễn tập/sự cố quá hạn | Số hành động chưa hoàn thành đến hạn |

Cần xác định cách đo, hệ thống nguồn và tiêu chí đạt trước khi báo cáo. Nếu không có RTO/RPO được duyệt thì không được báo cáo là đạt mục tiêu.

## 10. Lưu đồ
```mermaid
flowchart TD
 A([Gián đoạn/sự cố]) --> B[Đánh giá tác động và ghi nhận]
 B --> C{Đạt ngưỡng kích hoạt BCP/DR?}
 C -- Không --> D[Xử lý theo quy trình sự cố thông thường, đánh giá lại]
 D --> B
 C -- Có --> E[Người có thẩm quyền quyết định kích hoạt]
 E --> F[Bảo toàn bằng chứng và chuẩn bị môi trường]
 F --> G[Chọn backup/điểm khôi phục đã xác minh]
 G --> H[Khôi phục theo thứ tự ưu tiên]
 H --> I[Kiểm thử dữ liệu, chức năng và bảo mật]
 I --> J{Đạt tiêu chí và được nghiệm thu?}
 J -- Không --> K[Tiếp tục khắc phục / chọn phương án khác]
 K --> H
 J -- Có --> L[Đưa vào hoạt động, giám sát tăng cường]
 L --> M[Hậu kiểm, CAPA và cập nhật kế hoạch]
```

## 11. Điều kiện ban hành
- [ ] Xác định dịch vụ trọng yếu, owner và người có quyền kích hoạt.
- [ ] Phê duyệt BIA, RTO/RPO, thứ tự phục hồi và phụ thuộc.
- [ ] Xác minh danh bạ khẩn cấp, vendor và kênh liên lạc dự phòng.
- [ ] Chạy thử/diễn tập, kiểm tra backup và phục hồi.
- [ ] Ghi nhận vấn đề, khắc phục và kiểm tra lại.
- [ ] Đào tạo người tham gia, phê duyệt và công bố phiên bản hiệu lực.

**Lưu ý:** Quy trình là dự thảo quản trị liên tục/khôi phục; không tự chứng minh chứng nhận ISO hoặc năng lực đạt RTO/RPO nếu chưa được kiểm thử.
