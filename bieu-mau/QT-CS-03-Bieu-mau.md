# Bộ biểu mẫu QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng

> Dự thảo v0.1 — chưa ban hành. Các thông số khách hàng, SLA, quyền, retention, RTO/RPO và thời hạn thông báo phải theo hợp đồng/phụ lục được phê duyệt.

## Hướng dẫn
- Mỗi hồ sơ cần mã duy nhất, owner, trạng thái, bằng chứng và nơi lưu.
- Ghi “N/A” kèm lý do với trường không áp dụng.
- Không ghi mật khẩu, token, API key, khóa riêng hoặc mã khôi phục dạng rõ.
- Chỉ người có thẩm quyền phê duyệt; lưu hồ sơ theo phân loại và lịch lưu giữ.

## Danh mục
| Mã | Tên biểu mẫu |
|---|---|
| FR-DEL-01 | Danh mục quyền thu hồi |
| FR-DEL-02 | Quyết định trả/xóa/giữ dữ liệu |
| FR-DEL-03 | Biên bản xóa dữ liệu |
| FR-DEL-04 | Xác nhận xử lý dữ liệu vendor |
| FR-DEL-05 | Biên bản lưu giữ ngoại lệ |

---

### FR-DEL-01 Danh mục quyền thu hồi

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng.

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
- 1. **Hợp đồng/ngày kết thúc:**
- 2. **hệ thống:**
- 3. **ticket tồn:**
- 4. **tài sản/quyền:**
- 5. **dataset/bản sao:**
- 6. **quyết định trả/xóa/giữ:**
- 7. **bên nhận:**
- 8. **bằng chứng:**
- 9. **phê duyệt:**
- 10. **xác nhận khách hàng:**

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

### FR-DEL-02 Quyết định trả/xóa/giữ dữ liệu

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng.

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
- 1. **Hợp đồng/ngày kết thúc:**
- 2. **hệ thống:**
- 3. **ticket tồn:**
- 4. **tài sản/quyền:**
- 5. **dataset/bản sao:**
- 6. **quyết định trả/xóa/giữ:**
- 7. **bên nhận:**
- 8. **bằng chứng:**
- 9. **phê duyệt:**
- 10. **xác nhận khách hàng:**

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

### FR-DEL-03 Biên bản xóa dữ liệu

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng.

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
- 1. **Hợp đồng/ngày kết thúc:**
- 2. **hệ thống:**
- 3. **ticket tồn:**
- 4. **tài sản/quyền:**
- 5. **dataset/bản sao:**
- 6. **quyết định trả/xóa/giữ:**
- 7. **bên nhận:**
- 8. **bằng chứng:**
- 9. **phê duyệt:**
- 10. **xác nhận khách hàng:**

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

### FR-DEL-04 Xác nhận xử lý dữ liệu vendor

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng.

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
- 1. **Hợp đồng/ngày kết thúc:**
- 2. **hệ thống:**
- 3. **ticket tồn:**
- 4. **tài sản/quyền:**
- 5. **dataset/bản sao:**
- 6. **quyết định trả/xóa/giữ:**
- 7. **bên nhận:**
- 8. **bằng chứng:**
- 9. **phê duyệt:**
- 10. **xác nhận khách hàng:**

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

### FR-DEL-05 Biên bản lưu giữ ngoại lệ

**Mục đích:** Ghi nhận kiểm soát và bằng chứng cho QT-CS-03 — Thu hồi quyền và xóa dữ liệu sau hợp đồng.

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
- 1. **Hợp đồng/ngày kết thúc:**
- 2. **hệ thống:**
- 3. **ticket tồn:**
- 4. **tài sản/quyền:**
- 5. **dataset/bản sao:**
- 6. **quyết định trả/xóa/giữ:**
- 7. **bên nhận:**
- 8. **bằng chứng:**
- 9. **phê duyệt:**
- 10. **xác nhận khách hàng:**

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
