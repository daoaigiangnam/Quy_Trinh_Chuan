# Bộ biểu mẫu QT-BCP-02 — Khôi phục sau thảm họa

> Dự thảo v0.1 — chưa ban hành. Các thông số khách hàng, SLA, quyền, retention, RTO/RPO và thời hạn thông báo phải theo hợp đồng/phụ lục được phê duyệt.

## Hướng dẫn
- Mỗi hồ sơ cần mã duy nhất, owner, trạng thái, bằng chứng và nơi lưu.
- Ghi “N/A” kèm lý do với trường không áp dụng.
- Không ghi mật khẩu, token, API key, khóa riêng hoặc mã khôi phục dạng rõ.
- Chỉ người có thẩm quyền phê duyệt; lưu hồ sơ theo phân loại và lịch lưu giữ.

## Danh mục
| Mã | Tên biểu mẫu |
|---|---|
| FR-DR-01 | Phiếu kích hoạt DR |
| FR-DR-02 | Timeline điều phối |
| FR-DR-03 | Checklist khôi phục dịch vụ |
| FR-DR-04 | Xác nhận phục hồi |
| FR-DR-05 | Báo cáo hậu kiểm DR |

---

### FR-DR-01 Phiếu kích hoạt DR

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-BCP-02 — Khôi phục sau thảm họa.

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
- 1. **Tiêu chí kích hoạt:**
- 2. **hệ thống/phạm vi:**
- 3. **RTO/RPO mục tiêu và thực tế:**
- 4. **timeline:**
- 5. **thứ tự khôi phục:**
- 6. **kiểm thử:**
- 7. **người quyết định:**
- 8. **thông báo:**
- 9. **gap/action:**

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

### FR-DR-02 Timeline điều phối

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-BCP-02 — Khôi phục sau thảm họa.

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
- 1. **Tiêu chí kích hoạt:**
- 2. **hệ thống/phạm vi:**
- 3. **RTO/RPO mục tiêu và thực tế:**
- 4. **timeline:**
- 5. **thứ tự khôi phục:**
- 6. **kiểm thử:**
- 7. **người quyết định:**
- 8. **thông báo:**
- 9. **gap/action:**

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

### FR-DR-03 Checklist khôi phục dịch vụ

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-BCP-02 — Khôi phục sau thảm họa.

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
- 1. **Tiêu chí kích hoạt:**
- 2. **hệ thống/phạm vi:**
- 3. **RTO/RPO mục tiêu và thực tế:**
- 4. **timeline:**
- 5. **thứ tự khôi phục:**
- 6. **kiểm thử:**
- 7. **người quyết định:**
- 8. **thông báo:**
- 9. **gap/action:**

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

### FR-DR-04 Xác nhận phục hồi

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-BCP-02 — Khôi phục sau thảm họa.

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
- 1. **Tiêu chí kích hoạt:**
- 2. **hệ thống/phạm vi:**
- 3. **RTO/RPO mục tiêu và thực tế:**
- 4. **timeline:**
- 5. **thứ tự khôi phục:**
- 6. **kiểm thử:**
- 7. **người quyết định:**
- 8. **thông báo:**
- 9. **gap/action:**

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

### FR-DR-05 Báo cáo hậu kiểm DR

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-BCP-02 — Khôi phục sau thảm họa.

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
- 1. **Tiêu chí kích hoạt:**
- 2. **hệ thống/phạm vi:**
- 3. **RTO/RPO mục tiêu và thực tế:**
- 4. **timeline:**
- 5. **thứ tự khôi phục:**
- 6. **kiểm thử:**
- 7. **người quyết định:**
- 8. **thông báo:**
- 9. **gap/action:**

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
