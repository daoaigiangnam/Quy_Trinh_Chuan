# Bộ biểu mẫu QT-IT-07 — Phối hợp Sale và IT

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
| FR-SI-01 | Phiếu khảo sát nhu cầu | Theo sự kiện/điều kiện của quy trình QT-IT-07 |
| FR-SI-02 | Checklist khảo sát kỹ thuật | Theo sự kiện/điều kiện của quy trình QT-IT-07 |
| FR-SI-03 | Phiếu thẩm định khả thi | Theo sự kiện/điều kiện của quy trình QT-IT-07 |
| FR-SI-04 | Biên bản bàn giao Sale–IT | Theo sự kiện/điều kiện của quy trình QT-IT-07 |

---

### FR-SI-01 — Phiếu khảo sát nhu cầu

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-07 — Phối hợp Sale và IT.

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
| 11 | người yêu cầu/đầu mối |  |
| 12 | mô tả nhu cầu/vấn đề/hạng mục |  |
| 13 | mức ưu tiên/tác động |  |
| 14 | phạm vi và điều kiện hợp đồng |  |
| 15 | thời điểm bắt đầu/hạn/SLA |  |
| 16 | người thực hiện/người nhận |  |
| 17 | kết quả và tiêu chí nghiệm thu |  |
| 18 | việc tồn/đầu mối tiếp theo |  |

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

### FR-SI-02 — Checklist khảo sát kỹ thuật

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-07 — Phối hợp Sale và IT.

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
| 11 | người yêu cầu/đầu mối |  |
| 12 | mô tả nhu cầu/vấn đề/hạng mục |  |
| 13 | mức ưu tiên/tác động |  |
| 14 | phạm vi và điều kiện hợp đồng |  |
| 15 | thời điểm bắt đầu/hạn/SLA |  |
| 16 | người thực hiện/người nhận |  |
| 17 | kết quả và tiêu chí nghiệm thu |  |
| 18 | việc tồn/đầu mối tiếp theo |  |

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

### FR-SI-03 — Phiếu thẩm định khả thi

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-07 — Phối hợp Sale và IT.

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
| 11 | người yêu cầu/đầu mối |  |
| 12 | mô tả nhu cầu/vấn đề/hạng mục |  |
| 13 | mức ưu tiên/tác động |  |
| 14 | phạm vi và điều kiện hợp đồng |  |
| 15 | thời điểm bắt đầu/hạn/SLA |  |
| 16 | người thực hiện/người nhận |  |
| 17 | kết quả và tiêu chí nghiệm thu |  |
| 18 | việc tồn/đầu mối tiếp theo |  |

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

### FR-SI-04 — Biên bản bàn giao Sale–IT

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho quy trình QT-IT-07 — Phối hợp Sale và IT.

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
| 11 | người yêu cầu/đầu mối |  |
| 12 | mô tả nhu cầu/vấn đề/hạng mục |  |
| 13 | mức ưu tiên/tác động |  |
| 14 | phạm vi và điều kiện hợp đồng |  |
| 15 | thời điểm bắt đầu/hạn/SLA |  |
| 16 | người thực hiện/người nhận |  |
| 17 | kết quả và tiêu chí nghiệm thu |  |
| 18 | việc tồn/đầu mối tiếp theo |  |

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
