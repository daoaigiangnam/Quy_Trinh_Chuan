# QT-CS-03 — THU HỒI QUYỀN VÀ XÓA DỮ LIỆU SAU HỢP ĐỒNG

> **Trạng thái:** Dự thảo nâng cấp v0.2; cần rà soát, chạy thử và phê duyệt trước khi áp dụng.  
> **Chủ sở hữu:** Contract Owner / Service Owner.  
> **Liên quan:** QT-IT-08, QT-IT-11, QT-IT-12, QT-ATTT-04, QT-ISMS-02, MA-01, MA-02.

## 1. Kiểm soát tài liệu

| Trường | Nội dung |
|---|---|
| Mã | QT-CS-03 |
| Phiên bản | 0.2 — dự thảo nâng cấp |
| Chủ sở hữu | Contract Owner / Service Owner |
| Người rà soát | IT Lead, ATTT và Legal khi liên quan |
| Người phê duyệt | Người có thẩm quyền theo quản trị tài liệu/hợp đồng |
| Ngày hiệu lực | Điền sau khi phê duyệt |
| Chu kỳ rà soát | Khi có thay đổi hợp đồng và trước/sau kết thúc dịch vụ |

## 2. Mục đích và phạm vi

Xác minh toàn bộ quyền được thu hồi và dữ liệu được trả, lưu hoặc xóa đúng hợp đồng, không để tài khoản hoặc bản sao không kiểm soát.

Áp dụng theo hợp đồng/phụ lục và phạm vi ủy quyền. Không tự đặt thời hạn lưu, nghĩa vụ xóa hoặc thời hạn thông báo; phải đối chiếu hợp đồng, yêu cầu pháp lý đã được rà soát và quyết định người có thẩm quyền.

## 3. Nguyên tắc bắt buộc

1. Xác minh phạm vi, chủ sở hữu và người nhận trước khi chuyển dữ liệu/tài sản hoặc thu hồi dịch vụ.
2. Quyền truy cập phải được thu hồi hoặc có ủy quyền mới ghi nhận rõ; không để quyền tồn vô chủ.
3. Kiểm tra legal hold/nghĩa vụ lưu trước khi xóa dữ liệu.
4. Không ghi secret dạng rõ vào biên bản hoặc file bàn giao.
5. Nếu nghi có truy cập trái phép hoặc rò rỉ dữ liệu, kích hoạt QT-ATTT-04 và bảo toàn bằng chứng.
6. Mỗi việc tồn phải có owner, hạn và người chấp nhận rủi ro.

## 4. Vai trò

| Vai trò | Trách nhiệm |
|---|---|
| Contract Owner | Xác nhận hợp đồng, nghĩa vụ, ngày hiệu lực và phạm vi thương mại. |
| Service Owner/IT Lead | Điều phối chuyển giao, kỹ thuật, quyền và chất lượng. |
| Kỹ thuật viên | Thực hiện thao tác được duyệt, ghi log và kết quả. |
| Đầu mối khách hàng/bên nhận | Xác nhận quyền, nhận dữ liệu/tài liệu và nghiệm thu. |
| ATTT/Legal | Rà soát dữ liệu, sự cố, retention và nghĩa vụ pháp lý khi liên quan. |

## 5. Đầu vào và điều kiện bắt đầu

Hồ sơ cần có hợp đồng/phụ lục, ngày hiệu lực, danh mục hệ thống/tài sản/dữ liệu/quyền, đầu mối, người phê duyệt, kế hoạch, tiêu chí nghiệm thu và nơi lưu bằng chứng. Nếu thông tin mâu thuẫn hoặc người nhận chưa được xác minh, dừng việc chuyển/xóa/thu hồi có rủi ro và chuyển cấp.

## 6. Trình tự thực hiện chi tiết

### Bước 1 — Lập danh mục quyền/dữ liệu
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Thu thập tài khoản người dùng/admin, VPN, cloud, API token, service account, vendor, mailbox, shared drive, backup, monitoring, ticketing và thiết bị; lập danh mục dữ liệu production, staging, export, endpoint, file chia sẻ và backup.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 2 — Xác định thời điểm/ngoại lệ
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Đối chiếu ngày kết thúc, hợp đồng, nghĩa vụ lưu, legal hold, tranh chấp và yêu cầu khách hàng. Chốt thời điểm thu hồi từng quyền, dữ liệu trả/xóa/lưu, owner, người duyệt và ngày hết hạn ngoại lệ.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 3 — Thu hồi quyền
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Khóa tài khoản, phiên, token, khóa API, VPN, chứng thư, quyền hỗ trợ từ xa và quyền vendor. Xoay secret dùng chung nếu còn dùng cho dịch vụ khác; tránh gián đoạn khách hàng khác. Kiểm tra bằng log/trạng thái thực tế.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 4 — Trả dữ liệu
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Xuất dữ liệu theo định dạng/kênh đã thỏa thuận; xác minh người nhận, phạm vi và tính toàn vẹn. Ghi danh mục, thời gian, người giao/nhận, hash khi phù hợp và xác nhận. Không chuyển dữ liệu ngoài phạm vi.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 5 — Xóa dữ liệu
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Sau khi xác minh nghĩa vụ lưu và phê duyệt, xóa dữ liệu khỏi hệ thống hoạt động, vùng tạm, bản export, thiết bị và kho chia sẻ theo phương pháp được duyệt. Với backup có chu kỳ, ghi ngày hết hạn, hạn chế truy cập và ngăn khôi phục thông thường.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 6 — Xác nhận vendor
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Yêu cầu vendor xác nhận thu hồi quyền, trả/xóa dữ liệu và bản sao theo hợp đồng. Nếu vendor không xác nhận/không thể xóa, chuyển Contract Owner/Legal và đánh giá rủi ro.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 7 — Kiểm tra độc lập
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Đối chiếu danh mục với hệ thống thực tế, log đăng nhập sau ngày kết thúc, quyền tồn và bản sao. Tài khoản còn hoạt động phải có ủy quyền mới; nếu không, thu hồi và đánh giá sự cố.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 8 — Đóng hồ sơ
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Lập biên bản quyền đã thu hồi, dữ liệu trả/xóa/lưu, backup còn trong chu kỳ, ngoại lệ, xác nhận vendor/khách hàng và bằng chứng. Mọi việc tồn phải có owner/hạn và người chấp nhận.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

## 7. Xử lý ngoại lệ và chuyển cấp

Chuyển cấp khi có tranh chấp về quyền sở hữu dữ liệu, yêu cầu xóa mâu thuẫn nghĩa vụ lưu, không thể thu hồi tài khoản, vendor không xác nhận xóa, dữ liệu chuyển không toàn vẹn hoặc có nguy cơ gián đoạn. Ghi vấn đề, tác động, bằng chứng, người quyết định, phương án bù trừ, owner và hạn. Không tự xác nhận hoàn tất khi còn quyền/dữ liệu chưa được kiểm tra.

## 8. Bằng chứng vận hành

| Hồ sơ | Nội dung tối thiểu |
|---|---|
| Hợp đồng/phạm vi | Ngày kết thúc/chuyển giao, dịch vụ, nghĩa vụ |
| Danh mục quyền/tài sản/dữ liệu | Đối tượng, owner, trạng thái, người nhận |
| Kế hoạch và phê duyệt | Bước, lịch, người duyệt, điều kiện |
| Bằng chứng chuyển/thu hồi/xóa | Thời điểm, người làm, kết quả, log/xác nhận |
| Nghiệm thu/đóng hồ sơ | Người nhận, việc tồn, rủi ro và xác nhận |

Lưu tại kho chính thức, giới hạn quyền truy cập và retention theo danh mục/hợp đồng. Không đưa dữ liệu khách hàng hoặc secret vào repository mã nguồn.

## 9. KPI và giám sát

| KPI | Định nghĩa |
|---|---|
| Tỷ lệ checklist hoàn tất đúng hạn | Checklist hoàn tất đúng hạn / checklist đến hạn |
| Tỷ lệ quyền thu hồi được xác minh | Quyền đã xác minh thu hồi / quyền phải thu hồi |
| Tỷ lệ dữ liệu được đối soát | Dữ liệu trả/xóa/lưu có bằng chứng / dữ liệu thuộc danh mục |
| Ngoại lệ quá hạn | Số ngoại lệ hết hạn chưa đóng |
| Hồ sơ thiếu xác nhận | Hồ sơ chưa có nghiệm thu/xác nhận bắt buộc |

## 10. Lưu đồ

```mermaid
flowchart TD
 A([Khởi tạo kết thúc/chuyển giao]) --> B[Xác nhận hợp đồng và phạm vi]
 B --> C[Lập danh mục quyền, dữ liệu, tài sản, công việc]
 C --> D{Đủ phê duyệt và xác minh người nhận?}
 D -- Không --> E[Chờ xác minh / chuyển cấp]
 E --> D
 D -- Có --> F[Thực hiện bàn giao/thu hồi/xóa theo kế hoạch]
 F --> G[Kiểm tra độc lập và nghiệm thu]
 G --> H{Đạt tiêu chí?}
 H -- Không --> I[Khắc phục, ghi ngoại lệ và owner/hạn]
 I --> F
 H -- Có --> J[Đóng hồ sơ và lưu bằng chứng]
```

## 11. Điều kiện ban hành

- [ ] Xác nhận ngày hiệu lực, phạm vi hợp đồng và người có thẩm quyền.
- [ ] Đối chiếu danh mục quyền, tài sản, dữ liệu và nghĩa vụ lưu/xóa.
- [ ] Kiểm tra biểu mẫu và kho lưu bằng chứng.
- [ ] Chạy thử kịch bản chuyển giao/kết thúc, bao gồm ngoại lệ.
- [ ] Khắc phục sai lệch, đào tạo người tham gia và lưu bằng chứng.
- [ ] Phê duyệt và công bố phiên bản hiệu lực.

**Lưu ý:** Dự thảo cần được rà soát theo hợp đồng, pháp luật áp dụng và phạm vi ISMS; không tự chứng minh chứng nhận ISO.