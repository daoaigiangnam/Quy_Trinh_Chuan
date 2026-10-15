# REG-02 — Danh mục tài liệu, hồ sơ và lịch lưu giữ

> **Trạng thái:** Dự thảo. Thời hạn lưu dưới đây phải được Legal/ISMS/khách hàng xác nhận theo nghĩa vụ pháp lý, hợp đồng và nhu cầu vận hành; không coi các khoảng thời gian gợi ý là yêu cầu pháp luật.

## 1. Quy tắc kiểm soát tài liệu
1. Mỗi tài liệu có mã, tên, owner, phiên bản, trạng thái, người duyệt, ngày hiệu lực, nơi lưu và nhóm được truy cập.
2. Chỉ bản đã phê duyệt ở kho chính thức mới là bản kiểm soát; bản tải xuống/in ra phải được đánh dấu “bản tham khảo” nếu không kiểm soát được cập nhật.
3. Mọi thay đổi cần lý do, nội dung thay đổi, người rà soát/duyệt và lịch sử phiên bản.
4. Khi thay thế, thu hồi bản cũ khỏi nơi phát hành; giữ lịch sử theo lịch lưu giữ.
5. Không lưu secret dạng rõ trong SOP, mẫu, screenshot hoặc log.

## 2. Danh mục tài liệu khởi tạo
| Mã | Nhóm | Ví dụ | Owner | Người duyệt | Phân loại | Review gợi ý |
|---|---|---|---|---|---|---|
| POL-ISMS | Chính sách | Chính sách ATTT, phân loại dữ liệu | ISMS | BGĐ | Nội bộ | Hằng năm/khi thay đổi |
| QT-ISMS | Quy trình ISMS | Risk, SoA, audit, tài liệu, CAPA | ISMS | BGĐ/ủy quyền | Hằng năm |
| QT-IT | Vận hành IT | Ticket, change, asset, SLA, onboarding | ITL | Owner có thẩm quyền | Hằng năm/khi thay đổi |
| QT-ATTT | Kiểm soát ATTT | IAM, incident, log, vulnerability, network | ISMS/ITL | BGĐ/ủy quyền | Hằng năm/khi thay đổi |
| QT-OPS/BCP | Backup/BCP/DR | Backup, restore, BIA, DR | ITL/BCP Owner | BGĐ/Customer Owner theo phạm vi | Theo kế hoạch |
| FR | Biểu mẫu | Phiếu quyền, incident, change, backup | Process Owner | Owner tài liệu | Cùng quy trình |
| REG | Sổ đăng ký | Risk, evidence, asset, vendor, exception | Owner theo sổ | ISMS/ITL | Theo kỳ |
| CUS-APP | Phụ lục khách hàng | SLA, scope, contacts, systems, retention | Service Owner | Mstar và khách hàng theo hợp đồng | Khi thay đổi/gia hạn |
| RUN | Runbook | Thao tác vận hành, khôi phục, ứng cứu | System Owner | ITL/SEC | Sau test/sự cố/thay đổi |

## 3. Lịch lưu giữ — khung để phê duyệt
| Loại hồ sơ | Thời hạn khởi tạo đề xuất | Căn cứ phải xác nhận | Quyền truy cập | Hủy/đóng |
|---|---|---|---|---|
| Hợp đồng, phụ lục, SLA | Theo hợp đồng và nghĩa vụ pháp lý; có thể qua kỳ hợp đồng | Legal/Finance/contract | Hạn chế | Legal hold trước khi hủy |
| Ticket/SLA/báo cáo dịch vụ | Theo hợp đồng và nhu cầu tranh chấp; đề xuất 12–36 tháng để thảo luận | Customer contract | Service team/Owner | Xóa theo lịch được duyệt |
| Quyền truy cập/phê duyệt | Theo rủi ro và audit; đề xuất tối thiểu 12 tháng sau thu hồi để thảo luận | ISMS/contract | IAM Owner/ISMS | Hủy an toàn |
| Log bảo mật | Theo khả năng, rủi ro, hợp đồng và luật; đặt thời hạn online/archive riêng | Security/Legal | Rất hạn chế | Có quy trình purge |
| Incident/RCA/evidence | Theo mức độ, nghĩa vụ và legal hold | Legal/ISMS/customer contract | Incident team hạn chế | Chỉ hủy sau phê duyệt |
| Backup | Theo ma trận backup, RPO/RTO và hợp đồng | System Owner/customer | Backup Owner | Expiry/purge có xác minh |
| Hồ sơ nhân sự/đào tạo | Theo chính sách HR và luật áp dụng | HR/Legal | HR hạn chế | Hủy bảo mật |
| Audit/CAPA/SoA/risk | Theo nhu cầu chứng minh và chương trình ISMS; đề xuất nhiều chu kỳ audit | ISMS/Legal | ISMS/BGĐ | Phê duyệt trước hủy |
| Asset/license/vendor | Vòng đời tài sản/hợp đồng và kỳ đối soát | Asset/Vendor Owner | Owner | Lưu dấu vết thanh lý/exit |
| Hồ sơ xóa/trả dữ liệu | Theo hợp đồng và nghĩa vụ chứng minh | Customer Owner/Legal | Hạn chế | Giữ bằng chứng xóa theo lịch |

**Không tự động áp dụng các con số gợi ý:** chủ sở hữu phải điền thời hạn chính thức, căn cứ, ngày bắt đầu tính, điều kiện legal hold, người phê duyệt và cách hủy.

## 4. Phiếu yêu cầu thay đổi tài liệu
| Trường | Nội dung |
|---|---|
| Document ID / tên |  |
| Phiên bản hiện tại / dự kiến |  |
| Lý do thay đổi |  |
| Nội dung/đoạn bị ảnh hưởng |  |
| Tác động tới quy trình/khách hàng/SoA |  |
| Người soạn / ngày |  |
| Người rà soát / ý kiến |  |
| Người phê duyệt / ngày hiệu lực |  |
| Nơi phát hành / bản cũ thu hồi |  |

## 5. Checklist phát hành
- [ ] Mã/tên/owner/phiên bản đúng.
- [ ] Nội dung được rà soát kỹ thuật và bảo mật.
- [ ] Có phê duyệt đúng thẩm quyền.
- [ ] Đã xác định người nhận, phân loại và quyền.
- [ ] Đã cập nhật liên kết quy trình, mẫu và SoA nếu liên quan.
- [ ] Bản cũ được đánh dấu/thu hồi.
- [ ] Ngày review và thời hạn lưu được ghi nhận.
