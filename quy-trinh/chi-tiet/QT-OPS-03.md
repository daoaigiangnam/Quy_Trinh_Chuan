# QT-OPS-03 — QUẢN LÝ DOMAIN, SSL VÀ CHỨNG THƯ SỐ

> **Trạng thái:** Dự thảo nâng cấp v0.2; cần rà soát, chạy thử và phê duyệt trước khi áp dụng.  
> **Chủ sở hữu:** Owner quy trình / IT Lead / ISMS Owner theo phân công.  
> **Liên quan:** QT-ISMS-03/04/05/06, REG-01/02/03/04, MA-01 và phụ lục khách hàng khi áp dụng.

## 1. Kiểm soát tài liệu
| Trường | Nội dung |
|---|---|
| Mã | QT-OPS-03 |
| Phiên bản | 0.2 — dự thảo nâng cấp |
| Chủ sở hữu | Owner quy trình được phân công |
| Người rà soát | IT Lead/ISMS Owner và bên liên quan |
| Người phê duyệt | Người có thẩm quyền theo quản trị tài liệu |
| Ngày hiệu lực | Điền sau khi phê duyệt |
| Chu kỳ rà soát | Tối thiểu hằng năm và khi có thay đổi trọng yếu |

## 2. Mục đích và phạm vi
Theo dõi quyền sở hữu, gia hạn, DNS, chứng thư SSL/TLS và chứng thư số để tránh hết hạn, mất quyền kiểm soát hoặc gián đoạn dịch vụ.
Áp dụng theo phạm vi ISMS đã xác định và các dịch vụ Mstar/khách hàng liên quan. Mọi tiêu chí chấm điểm, retention, thẩm quyền và thời hạn phải lấy từ chính sách/hợp đồng được duyệt; không tự đặt yêu cầu pháp lý hoặc cam kết chưa xác minh.

## 3. Nguyên tắc bắt buộc
1. Xác định rõ owner, thẩm quyền và phạm vi trước khi bắt đầu.
2. Mọi quyết định trọng yếu phải có căn cứ, người quyết định, ngày và hành động tiếp theo.
3. Tách biệt người thực hiện với người phê duyệt khi có thể; nếu không thể, ghi kiểm soát bù trừ.
4. Không coi tài liệu đã viết là bằng chứng kiểm soát đã vận hành; cần bằng chứng thực tế.
5. Khi phát hiện sự cố ATTT, bảo toàn bằng chứng và phối hợp QT-ATTT-04.
6. Hồ sơ phải được lưu tại kho chính thức, có phân quyền và truy nguyên.

## 4. Vai trò
| Vai trò | Trách nhiệm |
|---|---|
| Owner quy trình | Duy trì nội dung, biểu mẫu, hiệu lực và cải tiến. |
| Người thực hiện | Thực hiện theo quy trình, lưu hồ sơ và báo sai lệch. |
| Người rà soát | Kiểm tra tính đầy đủ, khả thi, rủi ro và liên kết tài liệu. |
| Người phê duyệt | Quyết định hiệu lực/chấp nhận rủi ro trong thẩm quyền. |
| ISMS Owner/IT Lead | Điều phối, theo dõi tuân thủ và báo cáo lãnh đạo. |
| Khách hàng/Legal/HR/Finance | Tham gia khi nội dung thuộc hợp đồng, pháp lý, nhân sự hoặc chi phí. |

## 5. Đầu vào và điều kiện bắt đầu
Hồ sơ phải có mục tiêu, phạm vi, dữ liệu nguồn, người chịu trách nhiệm, tiêu chí đánh giá, người phê duyệt và nơi lưu. Nếu thiếu căn cứ hoặc có xung đột giữa quy trình với hợp đồng/pháp luật, ghi rõ điểm cần xác minh và chuyển người có thẩm quyền; không tự chọn cách diễn giải có lợi cho tiến độ.

## 6. Trình tự thực hiện chi tiết

### Bước 1 — Lập danh mục
**Người thực hiện:** Owner được phân công; IT Lead/ATTT/đầu mối nghiệp vụ rà soát theo nội dung.

Ghi domain/FQDN, registrar/CA, chủ sở hữu pháp lý, khách hàng, tài khoản quản trị, nhà cung cấp, ngày hết hạn, auto-renew, DNS provider, nameserver, dịch vụ phụ thuộc, certificate issuer/serial/fingerprint, SAN, ngày bắt đầu/hết hạn và owner nội bộ. Secret đăng nhập lưu trong vault, không trong danh mục.

**Điều kiện đạt:** Hồ sơ cập nhật, quyết định và bằng chứng có thể truy nguyên. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi nguyên nhân và giao hành động khắc phục.

### Bước 2 — Xác minh quyền sở hữu và quản trị
**Người thực hiện:** Owner được phân công; IT Lead/ATTT/đầu mối nghiệp vụ rà soát theo nội dung.

Kiểm tra hồ sơ đăng ký, email quản trị, MFA, recovery contact, quyền DNS/registrar và người được phép gia hạn/chuyển đổi. Không tự đổi nameserver, registrant hoặc DNS record khi chưa có phê duyệt khách hàng/owner.

**Điều kiện đạt:** Hồ sơ cập nhật, quyết định và bằng chứng có thể truy nguyên. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi nguyên nhân và giao hành động khắc phục.

### Bước 3 — Giám sát ngày hết hạn
**Người thực hiện:** Owner được phân công; IT Lead/ATTT/đầu mối nghiệp vụ rà soát theo nội dung.

Cấu hình cảnh báo nhiều mốc trước ngày hết hạn theo lịch nội bộ được duyệt, xác minh cảnh báo tới đúng người và có dự phòng. Kiểm tra cả domain, SSL, intermediate chain và chứng thư tích hợp; không dựa duy nhất vào thông báo vendor.

**Điều kiện đạt:** Hồ sơ cập nhật, quyết định và bằng chứng có thể truy nguyên. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi nguyên nhân và giao hành động khắc phục.

### Bước 4 — Gia hạn/cấp mới
**Người thực hiện:** Owner được phân công; IT Lead/ATTT/đầu mối nghiệp vụ rà soát theo nội dung.

Xác nhận chủ sở hữu, chi phí/đơn hàng và người duyệt thương mại; kỹ thuật xác nhận DNS, CSR, SAN, loại chứng thư, thời hạn, thuật toán và hệ thống đích. Không gửi private key qua email/chat. Cập nhật ngày hết hạn và bằng chứng thanh toán/cấp phát sau khi hoàn tất.

**Điều kiện đạt:** Hồ sơ cập nhật, quyết định và bằng chứng có thể truy nguyên. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi nguyên nhân và giao hành động khắc phục.

### Bước 5 — Triển khai chứng thư
**Người thực hiện:** Owner được phân công; IT Lead/ATTT/đầu mối nghiệp vụ rà soát theo nội dung.

Kiểm tra certificate chain, hostname/SAN, thời hạn, key match và môi trường. Lên lịch change nếu có tác động; sao lưu cấu hình an toàn, triển khai, kiểm tra HTTPS/TLS, redirect, ứng dụng phụ thuộc và cảnh báo. Có kế hoạch rollback nếu dịch vụ lỗi.

**Điều kiện đạt:** Hồ sơ cập nhật, quyết định và bằng chứng có thể truy nguyên. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi nguyên nhân và giao hành động khắc phục.

### Bước 6 — Quản lý DNS
**Người thực hiện:** Owner được phân công; IT Lead/ATTT/đầu mối nghiệp vụ rà soát theo nội dung.

Mọi thay đổi record phải có yêu cầu, mục đích, TTL/giá trị cũ-mới, người duyệt, người thực hiện và kiểm tra sau thay đổi. Rà soát record không còn dùng, quyền truy cập và nguy cơ subdomain takeover. Không lưu API token Cloudflare/DNS dạng rõ.

**Điều kiện đạt:** Hồ sơ cập nhật, quyết định và bằng chứng có thể truy nguyên. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi nguyên nhân và giao hành động khắc phục.

### Bước 7 — Xử lý hết hạn/sự cố
**Người thực hiện:** Owner được phân công; IT Lead/ATTT/đầu mối nghiệp vụ rà soát theo nội dung.

Nếu sắp hết hạn mà chưa gia hạn, chuyển cấp theo mức độ dịch vụ và thời gian còn lại; không chờ tới ngày hết hạn. Nếu domain/SSL bị chiếm, sai DNS hoặc chứng thư lỗi, ghi bằng chứng, khôi phục theo thẩm quyền và kích hoạt incident khi có dấu hiệu ATTT.

**Điều kiện đạt:** Hồ sơ cập nhật, quyết định và bằng chứng có thể truy nguyên. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi nguyên nhân và giao hành động khắc phục.

## 7. Ngoại lệ và chuyển cấp
Chuyển cấp khi thiếu thẩm quyền, có rủi ro vượt ngưỡng, nghĩa vụ pháp lý/hợp đồng chưa rõ, bằng chứng thiếu hoặc bị can thiệp, hành động quá hạn hoặc phát hiện kiểm soát không hiệu lực. Ghi nội dung, căn cứ, tác động, người nhận, quyết định cần thiết và hạn phản hồi. Ngoại lệ cần owner, rủi ro, biện pháp bù trừ, ngày hết hạn và người phê duyệt.

## 8. Bằng chứng và lưu hồ sơ
| Hồ sơ | Nội dung |
|---|---|
| Yêu cầu/đầu vào | Mục đích, phạm vi, nguồn và người yêu cầu |
| Đánh giá/rà soát | Tiêu chí, căn cứ, phát hiện và người rà soát |
| Quyết định/phê duyệt | Người quyết định, thời điểm, điều kiện và lý do |
| Nhật ký thực hiện | Hoạt động, kết quả, sai lệch và hành động tiếp theo |
| Báo cáo/khắc phục | Trạng thái, owner, hạn, kiểm tra hiệu lực |

Thời hạn lưu theo danh mục hồ sơ, hợp đồng và pháp luật đã được rà soát. Không xóa hồ sơ đang thuộc điều tra, tranh chấp hoặc legal hold. Không lưu secret dạng rõ.

## 9. KPI và giám sát
| KPI | Định nghĩa |
|---|---|
| Tỷ lệ hồ sơ đủ | Hồ sơ đáp ứng checklist / hồ sơ được lấy mẫu |
| Hành động quá hạn | Số hành động đến hạn chưa hoàn tất |
| Tỷ lệ rà soát đúng hạn | Tài liệu/rủi ro/kiểm soát được rà soát đúng hạn / số đến hạn |
| Tỷ lệ tái diễn | Sai lệch lặp lại cùng nguyên nhân |
| Tỷ lệ khắc phục hiệu lực | Hành động có bằng chứng hiệu lực / hành động được kiểm tra |

Chốt công thức, nguồn dữ liệu, kỳ đo và ngưỡng cảnh báo trước khi áp dụng. Không dùng tỷ lệ tổng hợp che khuất rủi ro nghiêm trọng.

## 10. Lưu đồ
```mermaid
flowchart TD
 A([Nhu cầu/chu kỳ rà soát]) --> B[Ghi nhận đầu vào và phạm vi]
 B --> C{Đủ căn cứ và đúng thẩm quyền?}
 C -- Không --> D[Bổ sung / chuyển cấp]
 D --> C
 C -- Có --> E[Đánh giá và thực hiện theo quy trình]
 E --> F[Rà soát kết quả và bằng chứng]
 F --> G{Đạt tiêu chí?}
 G -- Không --> H[Khắc phục / ngoại lệ có kiểm soát]
 H --> E
 G -- Có --> I[Phê duyệt, lưu hồ sơ, báo cáo]
 I --> J[Theo dõi và cải tiến]
```

## 11. Điều kiện ban hành
- [ ] Xác định owner, thẩm quyền và phạm vi áp dụng.
- [ ] Xác nhận tiêu chí/retention/thời hạn theo nguồn được duyệt.
- [ ] Đối chiếu biểu mẫu, danh mục và nơi lưu bằng chứng.
- [ ] Chạy thử một tình huống thường lệ và một tình huống ngoại lệ.
- [ ] Khắc phục sai lệch, đào tạo người liên quan và lưu bằng chứng.
- [ ] Phê duyệt và công bố phiên bản hiệu lực.

**Lưu ý:** Dự thảo này hỗ trợ vận hành ISMS nhưng không tự chứng minh chứng nhận ISO; phải phù hợp phạm vi ISMS, đánh giá rủi ro, SoA, hợp đồng và pháp luật áp dụng.
