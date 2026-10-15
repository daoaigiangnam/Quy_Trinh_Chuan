# Bộ biểu mẫu QT-IT-15 — Giám sát và bảo trì hệ thống

> **Trạng thái:** Dự thảo v0.1 — chưa ban hành. Áp dụng cho quy trình lõi Mstar; SLA, khách hàng, quyền, lưu giữ, RTO/RPO và thông báo phải theo hợp đồng/phụ lục từng khách hàng.

## Hướng dẫn chung

- Dùng biểu mẫu theo điều kiện kích hoạt; chủ sở hữu quy trình xác định mẫu bắt buộc trước khi ban hành.
- Mỗi hồ sơ phải có mã truy nguyên và liên kết ticket/change/incident/tài sản liên quan.
- Người thực hiện không tự phê duyệt rủi ro trọng yếu do mình tạo ra.
- Không ghi mật khẩu, token, API key, khóa riêng hoặc mã khôi phục dạng rõ.
- Lưu trong kho chính thức, theo phân loại, quyền truy cập và lịch lưu giữ đã được phê duyệt.

## Danh mục biểu mẫu

| Mã | Tên biểu mẫu | Khi sử dụng |
|---|---|---|
| FR-MON-01 | Ma trận giám sát/cảnh báo | Theo sự kiện/điều kiện của quy trình QT-IT-15 |
| FR-MON-02 | Kế hoạch bảo trì | Theo sự kiện/điều kiện của quy trình QT-IT-15 |
| FR-MON-03 | Báo cáo sức khỏe | Theo sự kiện/điều kiện của quy trình QT-IT-15 |
| FR-MON-04 | Phiếu xử lý cảnh báo | Theo sự kiện/điều kiện của quy trình QT-IT-15 |

---

### FR-MON-01 — Ma trận giám sát/cảnh báo

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-15 — Giám sát và bảo trì hệ thống.

**Cách điền:** Ghi mã hồ sơ duy nhất; điền đầy đủ trường áp dụng; ghi “N/A” kèm lý do với trường không áp dụng; liên kết ticket/log/bằng chứng trong kho được duyệt; không lưu secret dạng rõ; xin phê duyệt theo ma trận thẩm quyền.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ |  |
| Khách hàng/đơn vị |  |
| Hệ thống/dịch vụ/tài sản |  |
| Ngày lập/kỳ áp dụng |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/change/incident liên quan |  |
| Nơi lưu chính thức |  |
| Thời hạn lưu/ngày rà soát |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**

| STT | Trường cần ghi nhận | Giá trị / mô tả |
|---:|---|---|
| 1 | Mã hồ sơ |  |
| 2 |  ngày lập |  |
| 3 |  khách hàng/đơn vị |  |
| 4 |  hệ thống/dịch vụ/tài sản |  |
| 5 |  người lập |  |
| 6 |  owner |  |
| 7 |  ticket/change/incident liên quan |  |
| 8 |  phân loại thông tin |  |
| 9 |  nơi lưu hồ sơ |  |
| 10 |  trạng thái |  |
| 11 | mã tài sản/CI/FQDN/thiết bị |  |
| 12 | owner/người giữ/vendor |  |
| 13 | phiên bản/trạng thái/vị trí |  |
| 14 | cấu hình/giá trị chuẩn/hạn dùng |  |
| 15 | mức quan trọng và rủi ro |  |
| 16 | lần kiểm tra/kết quả |  |
| 17 | hành động/owner/hạn |  |
| 18 | bằng chứng |  |

**C. Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả/giá trị | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist trước khi đóng**

- [ ] Thông tin và phạm vi đã được xác minh.
- [ ] Quyền/phê duyệt cần thiết đã có.
- [ ] Kết quả và bằng chứng có thể truy nguyên.
- [ ] Rủi ro/ngoại lệ/việc tồn có owner và hạn.
- [ ] Hồ sơ lưu đúng nơi, đúng phân loại và quyền truy cập.
- [ ] Ticket/danh mục liên quan đã được cập nhật.


---

### FR-MON-02 — Kế hoạch bảo trì

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-15 — Giám sát và bảo trì hệ thống.

**Cách điền:** Ghi mã hồ sơ duy nhất; điền đầy đủ trường áp dụng; ghi “N/A” kèm lý do với trường không áp dụng; liên kết ticket/log/bằng chứng trong kho được duyệt; không lưu secret dạng rõ; xin phê duyệt theo ma trận thẩm quyền.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ |  |
| Khách hàng/đơn vị |  |
| Hệ thống/dịch vụ/tài sản |  |
| Ngày lập/kỳ áp dụng |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/change/incident liên quan |  |
| Nơi lưu chính thức |  |
| Thời hạn lưu/ngày rà soát |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**

| STT | Trường cần ghi nhận | Giá trị / mô tả |
|---:|---|---|
| 1 | Mã hồ sơ |  |
| 2 |  ngày lập |  |
| 3 |  khách hàng/đơn vị |  |
| 4 |  hệ thống/dịch vụ/tài sản |  |
| 5 |  người lập |  |
| 6 |  owner |  |
| 7 |  ticket/change/incident liên quan |  |
| 8 |  phân loại thông tin |  |
| 9 |  nơi lưu hồ sơ |  |
| 10 |  trạng thái |  |
| 11 | mã tài sản/CI/FQDN/thiết bị |  |
| 12 | owner/người giữ/vendor |  |
| 13 | phiên bản/trạng thái/vị trí |  |
| 14 | cấu hình/giá trị chuẩn/hạn dùng |  |
| 15 | mức quan trọng và rủi ro |  |
| 16 | lần kiểm tra/kết quả |  |
| 17 | hành động/owner/hạn |  |
| 18 | bằng chứng |  |

**C. Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả/giá trị | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist trước khi đóng**

- [ ] Thông tin và phạm vi đã được xác minh.
- [ ] Quyền/phê duyệt cần thiết đã có.
- [ ] Kết quả và bằng chứng có thể truy nguyên.
- [ ] Rủi ro/ngoại lệ/việc tồn có owner và hạn.
- [ ] Hồ sơ lưu đúng nơi, đúng phân loại và quyền truy cập.
- [ ] Ticket/danh mục liên quan đã được cập nhật.


---

### FR-MON-03 — Báo cáo sức khỏe

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-15 — Giám sát và bảo trì hệ thống.

**Cách điền:** Ghi mã hồ sơ duy nhất; điền đầy đủ trường áp dụng; ghi “N/A” kèm lý do với trường không áp dụng; liên kết ticket/log/bằng chứng trong kho được duyệt; không lưu secret dạng rõ; xin phê duyệt theo ma trận thẩm quyền.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ |  |
| Khách hàng/đơn vị |  |
| Hệ thống/dịch vụ/tài sản |  |
| Ngày lập/kỳ áp dụng |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/change/incident liên quan |  |
| Nơi lưu chính thức |  |
| Thời hạn lưu/ngày rà soát |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**

| STT | Trường cần ghi nhận | Giá trị / mô tả |
|---:|---|---|
| 1 | Mã hồ sơ |  |
| 2 |  ngày lập |  |
| 3 |  khách hàng/đơn vị |  |
| 4 |  hệ thống/dịch vụ/tài sản |  |
| 5 |  người lập |  |
| 6 |  owner |  |
| 7 |  ticket/change/incident liên quan |  |
| 8 |  phân loại thông tin |  |
| 9 |  nơi lưu hồ sơ |  |
| 10 |  trạng thái |  |
| 11 | mã tài sản/CI/FQDN/thiết bị |  |
| 12 | owner/người giữ/vendor |  |
| 13 | phiên bản/trạng thái/vị trí |  |
| 14 | cấu hình/giá trị chuẩn/hạn dùng |  |
| 15 | mức quan trọng và rủi ro |  |
| 16 | lần kiểm tra/kết quả |  |
| 17 | hành động/owner/hạn |  |
| 18 | bằng chứng |  |

**C. Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả/giá trị | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist trước khi đóng**

- [ ] Thông tin và phạm vi đã được xác minh.
- [ ] Quyền/phê duyệt cần thiết đã có.
- [ ] Kết quả và bằng chứng có thể truy nguyên.
- [ ] Rủi ro/ngoại lệ/việc tồn có owner và hạn.
- [ ] Hồ sơ lưu đúng nơi, đúng phân loại và quyền truy cập.
- [ ] Ticket/danh mục liên quan đã được cập nhật.


---

### FR-MON-04 — Phiếu xử lý cảnh báo

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-15 — Giám sát và bảo trì hệ thống.

**Cách điền:** Ghi mã hồ sơ duy nhất; điền đầy đủ trường áp dụng; ghi “N/A” kèm lý do với trường không áp dụng; liên kết ticket/log/bằng chứng trong kho được duyệt; không lưu secret dạng rõ; xin phê duyệt theo ma trận thẩm quyền.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ |  |
| Khách hàng/đơn vị |  |
| Hệ thống/dịch vụ/tài sản |  |
| Ngày lập/kỳ áp dụng |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/change/incident liên quan |  |
| Nơi lưu chính thức |  |
| Thời hạn lưu/ngày rà soát |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**

| STT | Trường cần ghi nhận | Giá trị / mô tả |
|---:|---|---|
| 1 | Mã hồ sơ |  |
| 2 |  ngày lập |  |
| 3 |  khách hàng/đơn vị |  |
| 4 |  hệ thống/dịch vụ/tài sản |  |
| 5 |  người lập |  |
| 6 |  owner |  |
| 7 |  ticket/change/incident liên quan |  |
| 8 |  phân loại thông tin |  |
| 9 |  nơi lưu hồ sơ |  |
| 10 |  trạng thái |  |
| 11 | mã tài sản/CI/FQDN/thiết bị |  |
| 12 | owner/người giữ/vendor |  |
| 13 | phiên bản/trạng thái/vị trí |  |
| 14 | cấu hình/giá trị chuẩn/hạn dùng |  |
| 15 | mức quan trọng và rủi ro |  |
| 16 | lần kiểm tra/kết quả |  |
| 17 | hành động/owner/hạn |  |
| 18 | bằng chứng |  |

**C. Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả/giá trị | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist trước khi đóng**

- [ ] Thông tin và phạm vi đã được xác minh.
- [ ] Quyền/phê duyệt cần thiết đã có.
- [ ] Kết quả và bằng chứng có thể truy nguyên.
- [ ] Rủi ro/ngoại lệ/việc tồn có owner và hạn.
- [ ] Hồ sơ lưu đúng nơi, đúng phân loại và quyền truy cập.
- [ ] Ticket/danh mục liên quan đã được cập nhật.



## Kiểm soát phát hành

| Trường | Nội dung |
|---|---|
| Chủ sở hữu quy trình |  |
| Người rà soát |  |
| Người phê duyệt |  |
| Phiên bản/ngày hiệu lực |  |
| Kho lưu hồ sơ chính thức |  |
| Quyền truy cập |  |
| Thời hạn lưu |  |
| Ngày rà soát tiếp theo |  |
