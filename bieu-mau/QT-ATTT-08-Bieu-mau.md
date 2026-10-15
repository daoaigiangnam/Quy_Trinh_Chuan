# Bộ biểu mẫu QT-ATTT-08 — Quản lý mạng, Firewall và truy cập từ xa

> Dự thảo v0.1 — chưa ban hành. Các thông số khách hàng, SLA, quyền, retention, RTO/RPO và thời hạn thông báo phải theo hợp đồng/phụ lục được phê duyệt.

## Hướng dẫn
- Mỗi hồ sơ cần mã duy nhất, owner, trạng thái, bằng chứng và nơi lưu.
- Ghi “N/A” kèm lý do với trường không áp dụng.
- Không ghi mật khẩu, token, API key, khóa riêng hoặc mã khôi phục dạng rõ.
- Chỉ người có thẩm quyền phê duyệt; lưu hồ sơ theo phân loại và lịch lưu giữ.

## Danh mục
| Mã | Tên biểu mẫu |
|---|---|
| FR-NET-01 | Yêu cầu rule firewall |
| FR-NET-02 | Ma trận luồng mạng |
| FR-NET-03 | Cấp VPN/remote support |
| FR-NET-04 | Rà soát rule firewall |

---

### FR-NET-01 Yêu cầu rule firewall

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-08 — Quản lý mạng, Firewall và truy cập từ xa.

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

- 1. **Source/destination:**
- 2. **port/protocol:**
- 3. **mục đích:**
- 4. **owner:**
- 5. **hệ thống khách hàng:**
- 6. **MFA:**
- 7. **thời hạn:**
- 8. **phê duyệt:**
- 9. **change ID:**
- 10. **log/xác minh:**

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

### FR-NET-02 Ma trận luồng mạng

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-08 — Quản lý mạng, Firewall và truy cập từ xa.

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

- 1. **Source/destination:**
- 2. **port/protocol:**
- 3. **mục đích:**
- 4. **owner:**
- 5. **hệ thống khách hàng:**
- 6. **MFA:**
- 7. **thời hạn:**
- 8. **phê duyệt:**
- 9. **change ID:**
- 10. **log/xác minh:**

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

### FR-NET-03 Cấp VPN/remote support

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-08 — Quản lý mạng, Firewall và truy cập từ xa.

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

- 1. **Source/destination:**
- 2. **port/protocol:**
- 3. **mục đích:**
- 4. **owner:**
- 5. **hệ thống khách hàng:**
- 6. **MFA:**
- 7. **thời hạn:**
- 8. **phê duyệt:**
- 9. **change ID:**
- 10. **log/xác minh:**

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

### FR-NET-04 Rà soát rule firewall

**Mục đích:** Ghi nhận quyết định, công việc và bằng chứng cho QT-ATTT-08 — Quản lý mạng, Firewall và truy cập từ xa.

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

- 1. **Source/destination:**
- 2. **port/protocol:**
- 3. **mục đích:**
- 4. **owner:**
- 5. **hệ thống khách hàng:**
- 6. **MFA:**
- 7. **thời hạn:**
- 8. **phê duyệt:**
- 9. **change ID:**
- 10. **log/xác minh:**

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
