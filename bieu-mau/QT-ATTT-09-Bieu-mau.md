# Bộ biểu mẫu QT-ATTT-09 — Quản lý nhà cung cấp và bên thứ ba

> Dự thảo v0.1 — chưa ban hành. Các thông số khách hàng, SLA, quyền, retention, RTO/RPO và thời hạn thông báo phải theo hợp đồng/phụ lục được phê duyệt.

## Hướng dẫn
- Mỗi hồ sơ cần mã duy nhất, owner, trạng thái, bằng chứng và nơi lưu.
- Ghi “N/A” kèm lý do với trường không áp dụng.
- Không ghi mật khẩu, token, API key, khóa riêng hoặc mã khôi phục dạng rõ.
- Chỉ người có thẩm quyền phê duyệt; lưu hồ sơ theo phân loại và lịch lưu giữ.

## Danh mục
| Mã | Tên biểu mẫu |
|---|---|
| FR-SUP-01 | Hồ sơ nhà cung cấp |
| FR-SUP-02 | Đánh giá rủi ro nhà cung cấp |
| FR-SUP-03 | Checklist điều khoản |
| FR-SUP-04 | Rà soát định kỳ |
| FR-SUP-05 | Checklist kết thúc vendor |

---

### FR-SUP-01 Hồ sơ nhà cung cấp

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-09 — Quản lý nhà cung cấp và bên thứ ba.

**Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ / ngày lập |  |
| Khách hàng / hệ thống / tài sản |  |
| Người lập / owner |  |
| Phân loại thông tin |  |
| Ticket / change / incident liên quan |  |
| Nơi lưu / thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**Trường nghiệp vụ cần điền**

- 1. **Dịch vụ/vendor:**
- 2. **dữ liệu/hệ thống truy cập:**
- 3. **criticality:**
- 4. **quyền:**
- 5. **bằng chứng bảo mật:**
- 6. **sự cố/SLA:**
- 7. **subprocessor:**
- 8. **điều khoản:**
- 9. **rủi ro:**
- 10. **quyết định gia hạn/exit:**

**Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục / hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**Checklist đóng hồ sơ**
- [ ] Phạm vi và quyền được xác minh.
- [ ] Kết quả, log/bằng chứng đã lưu an toàn.
- [ ] Rủi ro/ngoại lệ có owner, hạn và phê duyệt.
- [ ] Ticket/danh mục liên quan đã cập nhật.
- [ ] Không có secret dạng rõ trong hồ sơ.

---

### FR-SUP-02 Đánh giá rủi ro nhà cung cấp

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-09 — Quản lý nhà cung cấp và bên thứ ba.

**Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ / ngày lập |  |
| Khách hàng / hệ thống / tài sản |  |
| Người lập / owner |  |
| Phân loại thông tin |  |
| Ticket / change / incident liên quan |  |
| Nơi lưu / thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**Trường nghiệp vụ cần điền**

- 1. **Dịch vụ/vendor:**
- 2. **dữ liệu/hệ thống truy cập:**
- 3. **criticality:**
- 4. **quyền:**
- 5. **bằng chứng bảo mật:**
- 6. **sự cố/SLA:**
- 7. **subprocessor:**
- 8. **điều khoản:**
- 9. **rủi ro:**
- 10. **quyết định gia hạn/exit:**

**Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục / hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**Checklist đóng hồ sơ**
- [ ] Phạm vi và quyền được xác minh.
- [ ] Kết quả, log/bằng chứng đã lưu an toàn.
- [ ] Rủi ro/ngoại lệ có owner, hạn và phê duyệt.
- [ ] Ticket/danh mục liên quan đã cập nhật.
- [ ] Không có secret dạng rõ trong hồ sơ.

---

### FR-SUP-03 Checklist điều khoản

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-09 — Quản lý nhà cung cấp và bên thứ ba.

**Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ / ngày lập |  |
| Khách hàng / hệ thống / tài sản |  |
| Người lập / owner |  |
| Phân loại thông tin |  |
| Ticket / change / incident liên quan |  |
| Nơi lưu / thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**Trường nghiệp vụ cần điền**

- 1. **Dịch vụ/vendor:**
- 2. **dữ liệu/hệ thống truy cập:**
- 3. **criticality:**
- 4. **quyền:**
- 5. **bằng chứng bảo mật:**
- 6. **sự cố/SLA:**
- 7. **subprocessor:**
- 8. **điều khoản:**
- 9. **rủi ro:**
- 10. **quyết định gia hạn/exit:**

**Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục / hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**Checklist đóng hồ sơ**
- [ ] Phạm vi và quyền được xác minh.
- [ ] Kết quả, log/bằng chứng đã lưu an toàn.
- [ ] Rủi ro/ngoại lệ có owner, hạn và phê duyệt.
- [ ] Ticket/danh mục liên quan đã cập nhật.
- [ ] Không có secret dạng rõ trong hồ sơ.

---

### FR-SUP-04 Rà soát định kỳ

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-09 — Quản lý nhà cung cấp và bên thứ ba.

**Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ / ngày lập |  |
| Khách hàng / hệ thống / tài sản |  |
| Người lập / owner |  |
| Phân loại thông tin |  |
| Ticket / change / incident liên quan |  |
| Nơi lưu / thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**Trường nghiệp vụ cần điền**

- 1. **Dịch vụ/vendor:**
- 2. **dữ liệu/hệ thống truy cập:**
- 3. **criticality:**
- 4. **quyền:**
- 5. **bằng chứng bảo mật:**
- 6. **sự cố/SLA:**
- 7. **subprocessor:**
- 8. **điều khoản:**
- 9. **rủi ro:**
- 10. **quyết định gia hạn/exit:**

**Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục / hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**Checklist đóng hồ sơ**
- [ ] Phạm vi và quyền được xác minh.
- [ ] Kết quả, log/bằng chứng đã lưu an toàn.
- [ ] Rủi ro/ngoại lệ có owner, hạn và phê duyệt.
- [ ] Ticket/danh mục liên quan đã cập nhật.
- [ ] Không có secret dạng rõ trong hồ sơ.

---

### FR-SUP-05 Checklist kết thúc vendor

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-09 — Quản lý nhà cung cấp và bên thứ ba.

**Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ / ngày lập |  |
| Khách hàng / hệ thống / tài sản |  |
| Người lập / owner |  |
| Phân loại thông tin |  |
| Ticket / change / incident liên quan |  |
| Nơi lưu / thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**Trường nghiệp vụ cần điền**

- 1. **Dịch vụ/vendor:**
- 2. **dữ liệu/hệ thống truy cập:**
- 3. **criticality:**
- 4. **quyền:**
- 5. **bằng chứng bảo mật:**
- 6. **sự cố/SLA:**
- 7. **subprocessor:**
- 8. **điều khoản:**
- 9. **rủi ro:**
- 10. **quyết định gia hạn/exit:**

**Nhật ký / dòng dữ liệu**

| Ngày giờ | Hạng mục / hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Việc tiếp theo/hạn |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**Kiểm tra và phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt theo thẩm quyền |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**Checklist đóng hồ sơ**
- [ ] Phạm vi và quyền được xác minh.
- [ ] Kết quả, log/bằng chứng đã lưu an toàn.
- [ ] Rủi ro/ngoại lệ có owner, hạn và phê duyệt.
- [ ] Ticket/danh mục liên quan đã cập nhật.
- [ ] Không có secret dạng rõ trong hồ sơ.


## Kiểm soát phát hành
| Trường | Nội dung |
|---|---|
| Chủ sở hữu quy trình |  |
| Người rà soát / phê duyệt |  |
| Phiên bản / ngày hiệu lực |  |
| Kho lưu / quyền truy cập |  |
| Thời hạn lưu / ngày rà soát |  |
