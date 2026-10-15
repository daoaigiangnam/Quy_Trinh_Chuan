# Bộ biểu mẫu QT-OPS-03 — Quản lý domain, SSL và chứng thư số

> Dự thảo v0.1 — chưa ban hành. Các thông số khách hàng, SLA, quyền, retention, RTO/RPO và thời hạn thông báo phải theo hợp đồng/phụ lục được phê duyệt.

## Hướng dẫn
- Mỗi hồ sơ cần mã duy nhất, owner, trạng thái, bằng chứng và nơi lưu.
- Ghi “N/A” kèm lý do với trường không áp dụng.
- Không ghi mật khẩu, token, API key, khóa riêng hoặc mã khôi phục dạng rõ.
- Chỉ người có thẩm quyền phê duyệt; lưu hồ sơ theo phân loại và lịch lưu giữ.

## Danh mục
| Mã | Tên biểu mẫu |
|---|---|
| FR-EXP-01 | Inventory domain/SSL |
| FR-EXP-02 | Yêu cầu gia hạn/thay thế |
| FR-EXP-03 | Lịch cảnh báo |
| FR-EXP-04 | Checklist DNS/TLS |

---

### FR-EXP-01 Inventory domain/SSL

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-OPS-03 — Quản lý domain, SSL và chứng thư số.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ/ngày lập |  |
| Khách hàng/đơn vị/hệ thống |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/incident/contract liên quan |  |
| Nơi lưu/thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**
- 1. **Domain/FQDN:**
- 2. **registrar/CA/vendor:**
- 3. **owner:**
- 4. **DNS/hostname:**
- 5. **serial:**
- 6. **ngày hết hạn:**
- 7. **cảnh báo:**
- 8. **phê duyệt gia hạn:**
- 9. **kiểm tra chain/TLS sau thay đổi:**

**C. Nhật ký/bảng ghi nhận**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Owner/hạn tiếp theo |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Rà soát/phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist**
- [ ] Phạm vi và thẩm quyền đã được xác minh.
- [ ] Kết quả được kiểm tra và có bằng chứng.
- [ ] Ngoại lệ/việc tồn có owner, hạn và phê duyệt.
- [ ] Hồ sơ lưu đúng nơi và đúng quyền.
- [ ] Không lưu secret dạng rõ.

---

### FR-EXP-02 Yêu cầu gia hạn/thay thế

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-OPS-03 — Quản lý domain, SSL và chứng thư số.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ/ngày lập |  |
| Khách hàng/đơn vị/hệ thống |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/incident/contract liên quan |  |
| Nơi lưu/thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**
- 1. **Domain/FQDN:**
- 2. **registrar/CA/vendor:**
- 3. **owner:**
- 4. **DNS/hostname:**
- 5. **serial:**
- 6. **ngày hết hạn:**
- 7. **cảnh báo:**
- 8. **phê duyệt gia hạn:**
- 9. **kiểm tra chain/TLS sau thay đổi:**

**C. Nhật ký/bảng ghi nhận**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Owner/hạn tiếp theo |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Rà soát/phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist**
- [ ] Phạm vi và thẩm quyền đã được xác minh.
- [ ] Kết quả được kiểm tra và có bằng chứng.
- [ ] Ngoại lệ/việc tồn có owner, hạn và phê duyệt.
- [ ] Hồ sơ lưu đúng nơi và đúng quyền.
- [ ] Không lưu secret dạng rõ.

---

### FR-EXP-03 Lịch cảnh báo

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-OPS-03 — Quản lý domain, SSL và chứng thư số.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ/ngày lập |  |
| Khách hàng/đơn vị/hệ thống |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/incident/contract liên quan |  |
| Nơi lưu/thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**
- 1. **Domain/FQDN:**
- 2. **registrar/CA/vendor:**
- 3. **owner:**
- 4. **DNS/hostname:**
- 5. **serial:**
- 6. **ngày hết hạn:**
- 7. **cảnh báo:**
- 8. **phê duyệt gia hạn:**
- 9. **kiểm tra chain/TLS sau thay đổi:**

**C. Nhật ký/bảng ghi nhận**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Owner/hạn tiếp theo |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Rà soát/phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist**
- [ ] Phạm vi và thẩm quyền đã được xác minh.
- [ ] Kết quả được kiểm tra và có bằng chứng.
- [ ] Ngoại lệ/việc tồn có owner, hạn và phê duyệt.
- [ ] Hồ sơ lưu đúng nơi và đúng quyền.
- [ ] Không lưu secret dạng rõ.

---

### FR-EXP-04 Checklist DNS/TLS

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-OPS-03 — Quản lý domain, SSL và chứng thư số.

**A. Thông tin hồ sơ**

| Trường | Nội dung |
|---|---|
| Mã hồ sơ/ngày lập |  |
| Khách hàng/đơn vị/hệ thống |  |
| Người lập/owner |  |
| Phân loại thông tin |  |
| Ticket/incident/contract liên quan |  |
| Nơi lưu/thời hạn lưu |  |
| Trạng thái | Nháp / Chờ duyệt / Đã duyệt / Đóng |

**B. Trường nghiệp vụ**
- 1. **Domain/FQDN:**
- 2. **registrar/CA/vendor:**
- 3. **owner:**
- 4. **DNS/hostname:**
- 5. **serial:**
- 6. **ngày hết hạn:**
- 7. **cảnh báo:**
- 8. **phê duyệt gia hạn:**
- 9. **kiểm tra chain/TLS sau thay đổi:**

**C. Nhật ký/bảng ghi nhận**

| Ngày giờ | Hạng mục/hành động | Người thực hiện | Kết quả | Bằng chứng/ticket | Owner/hạn tiếp theo |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
|  |  |  |  |  |  |

**D. Rà soát/phê duyệt**

| Vai trò | Họ tên/chức danh | Ý kiến/điều kiện | Kết quả | Ngày |
|---|---|---|---|---|
| Người lập |  |  |  |  |
| Người kiểm tra/owner |  |  |  |  |
| Người phê duyệt |  |  |  |  |
| Đầu mối khách hàng (nếu cần) |  |  |  |  |

**E. Checklist**
- [ ] Phạm vi và thẩm quyền đã được xác minh.
- [ ] Kết quả được kiểm tra và có bằng chứng.
- [ ] Ngoại lệ/việc tồn có owner, hạn và phê duyệt.
- [ ] Hồ sơ lưu đúng nơi và đúng quyền.
- [ ] Không lưu secret dạng rõ.


## Kiểm soát phát hành
| Trường | Nội dung |
|---|---|
| Chủ sở hữu quy trình |  |
| Người rà soát/phê duyệt |  |
| Phiên bản/ngày hiệu lực |  |
| Kho lưu/quyền truy cập |  |
| Thời hạn lưu/ngày rà soát |  |
