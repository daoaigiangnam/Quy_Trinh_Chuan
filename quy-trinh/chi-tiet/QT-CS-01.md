# QT-CS-01 — KẾT THÚC HỢP ĐỒNG DỊCH VỤ KHÁCH HÀNG

> **Trạng thái:** Dự thảo nâng cấp v0.2; cần rà soát, chạy thử và phê duyệt trước khi áp dụng.  
> **Chủ sở hữu:** Contract Owner / Service Owner.  
> **Liên quan:** QT-IT-08, QT-IT-11, QT-IT-12, QT-ATTT-04, QT-ISMS-02, MA-01, MA-02.

## 1. Kiểm soát tài liệu

| Trường | Nội dung |
|---|---|
| Mã | QT-CS-01 |
| Phiên bản | 0.2 — dự thảo nâng cấp |
| Chủ sở hữu | Contract Owner / Service Owner |
| Người rà soát | IT Lead, ATTT và Legal khi liên quan |
| Người phê duyệt | Người có thẩm quyền theo quản trị tài liệu/hợp đồng |
| Ngày hiệu lực | Điền sau khi phê duyệt |
| Chu kỳ rà soát | Khi có thay đổi hợp đồng và trước/sau kết thúc dịch vụ |

## 2. Mục đích và phạm vi

Kết thúc dịch vụ có kiểm soát, xác định nghĩa vụ còn lại, bàn giao dữ liệu/tài sản và tránh để quyền hoặc công việc tồn tại sau ngày kết thúc.

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

### Bước 1 — Khởi tạo kết thúc
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Contract Owner ghi ngày kết thúc, lý do, phạm vi dịch vụ dừng, điều khoản thông báo, trách nhiệm còn lại và đầu mối hai bên. Xác minh kết thúc toàn bộ hay một phần; không tự ngắt dịch vụ trước thời điểm/điều kiện hợp đồng.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 2 — Lập kế hoạch
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Chỉ định owner, mốc thời gian, hệ thống/dữ liệu/tài sản, quyền truy cập, ticket mở, backup, vendor, license/domain, báo cáo cuối và phương án chuyển tiếp. Mỗi đầu việc có người phụ trách, hạn, phụ thuộc và tiêu chí hoàn tất.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 3 — Đối soát dịch vụ
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Liệt kê ticket/incident/change mở, SLA chưa chốt, vấn đề tồn, rủi ro, cấu hình, sơ đồ, runbook, tài sản, tài khoản, dữ liệu và báo cáo. Đối soát với khách hàng, ghi tranh chấp và người quyết định.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 4 — Bàn giao dữ liệu
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Xác định dữ liệu thuộc khách hàng, định dạng, kênh truyền, người nhận được ủy quyền, thời hạn, kiểm tra tính toàn vẹn và xác nhận nhận. Chỉ chuyển nội dung thuộc phạm vi; bảo vệ secret và thông tin Mstar/vendor không thuộc quyền bàn giao.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 5 — Thu hồi quyền và tài sản
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Lập danh sách tài khoản, VPN, token, API key, vendor, cloud, giám sát và quyền vào cơ sở. Phối hợp QT-IT-11/QT-CS-03; thu hồi đúng thời điểm đã duyệt, không thu hồi sớm gây gián đoạn nhưng cũng không để quyền mở quá hạn.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 6 — Xử lý dữ liệu và backup
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Theo hợp đồng xác định dữ liệu cần trả, lưu và xóa. Kiểm tra legal hold/điều tra trước khi xóa. Ghi phương pháp, người duyệt, ngày, phạm vi, xác nhận khách hàng và bản sao chưa thể xóa ngay.

**Điều kiện đạt:** Có xác nhận và bằng chứng truy nguyên. **Nếu không đạt:** Giữ hồ sơ mở, ghi sai lệch, owner và hạn khắc phục.

### Bước 7 — Nghiệm thu và đóng
**Người thực hiện:** Contract Owner/Service Owner/IT theo phân công.

Xác nhận cuối về dịch vụ, tài sản, dữ liệu, quyền, ticket, tài liệu và các việc thương mại theo thẩm quyền. Ghi biên bản, ngoại lệ, owner/hạn và người chấp nhận. Chỉ đóng khi có bằng chứng hoặc kế hoạch tồn được duyệt.

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