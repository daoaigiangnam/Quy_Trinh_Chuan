# MA-02 — Ma trận phân quyền RBAC chuẩn Mstar

> **Trạng thái:** Dự thảo v0.1. Đây là ma trận vai trò mẫu cho Mstar; quyền trên tenant/hệ thống khách hàng phải được khách hàng phê duyệt riêng. Không đồng nghĩa mọi kỹ thuật viên được truy cập mọi khách hàng.

## 1. Mô hình quyền
- **RBAC:** cấp quyền theo vai trò công việc, không theo sự thuận tiện cá nhân.
- **Least privilege:** chỉ cấp quyền tối thiểu cần thiết, đúng phạm vi và thời hạn.
- **Need-to-know:** chỉ xem dữ liệu cần để xử lý công việc.
- **MFA:** bắt buộc cho truy cập từ xa, tài khoản quản trị và hệ thống hỗ trợ MFA; ngoại lệ phải có kiểm soát bù trừ và thời hạn.
- **Named account:** ưu tiên tài khoản định danh riêng; tài khoản dùng chung chỉ khi bất khả kháng, có vault, nhật ký và người chịu trách nhiệm.
- **Time-bound access:** quyền tạm thời phải có ngày hết hạn và được thu hồi tự động hoặc theo checklist.
- **Segregation:** người yêu cầu không tự phê duyệt quyền của mình.

## 2. Mức quyền
| Mã | Quyền | Mô tả |
|---|---|---|
| V | View | Xem dữ liệu được phép |
| C | Create | Tạo hồ sơ/ticket |
| E | Edit | Sửa trong phạm vi được giao |
| X | Execute | Thực hiện thao tác kỹ thuật |
| AP | Approve | Phê duyệt theo thẩm quyền |
| AD | Admin | Quản trị cấu hình/quyền |
| RV | Review | Rà soát độc lập |
| — | No access | Không được truy cập |

## 3. Ma trận quyền trên công cụ Mstar
| Vai trò | Ticket/Bitrix | CMDB/tài sản | Kho tài liệu | Vault/Secrets | Monitoring/Logs | Thay đổi production | Báo cáo khách hàng | Quản trị quyền |
|---|---|---|---|---|---|---|---|---|
| Ban Giám đốc | V | V | V theo nhu cầu | — mặc định | V báo cáo | AP theo thẩm quyền | V | AP chính sách |
| ISMS Owner | V | V | E/RV | V metadata, secret chỉ khi được ủy quyền | V/RV | RV | V | RV |
| IT Lead/Service Owner | V/E/AP | V/E | V/E | V theo phê duyệt | V/E | AP/X theo phạm vi | E/AP | AP theo phạm vi |
| Service Desk L1 | C/E ticket | V giới hạn | V runbook | — mặc định | V dashboard | — hoặc X tác vụ chuẩn đã duyệt | C | — |
| Engineer L2 | V/E ticket | V/E theo phạm vi | V/E | Truy cập qua vault theo ticket | V/X | X theo change đã duyệt | C | — |
| Senior/Lead L3 | V/E | V/E | V/E | Truy cập đặc quyền theo phê duyệt | V/X/RV | X; không tự duyệt change của mình | C/RV | R theo ủy quyền |
| Security/Incident Lead | V incident | V khi cần | V runbook | X khi cần ứng cứu và được ủy quyền | V/RV/X | X khẩn cấp theo playbook | R | RV/khóa quyền khẩn cấp theo ủy quyền |
| Sale/Account Manager | V thông tin hợp đồng cần thiết | — | V tài liệu đã phát hành | — | — | — | C | — |
| HR | — | V thiết bị được giao | V chính sách/đào tạo | — | — | — | — | Yêu cầu offboarding, không tự cấp quyền kỹ thuật |
| Auditor nội bộ | V bằng chứng theo phạm vi | V theo mẫu | V bản kiểm soát | —; chỉ metadata khi cần | V bản xuất đã duyệt | — | V theo phạm vi | RV |
| Khách hàng Owner | V/E phạm vi khách hàng | V tài sản khách hàng | V tài liệu khách hàng được phép | Không tự động có quyền vault Mstar | V báo cáo khách hàng | AP theo hợp đồng | V/AP | AP quyền trong tenant khách hàng |
| Nhà cung cấp | — hoặc ticket giới hạn | — | Chỉ tài liệu cần thiết | Truy cập tạm thời theo phê duyệt | Theo phạm vi | Chỉ change được giao | — | — |

**Lưu ý:** Ma trận trên là baseline tham khảo. Trước khi triển khai phải cấu hình theo công cụ thực tế, từng nhóm khách hàng, hợp đồng và phân loại dữ liệu.

## 4. Ma trận phê duyệt cấp quyền
| Loại quyền | Người yêu cầu | Người duyệt | Người thực hiện | Kiểm tra sau cấp |
|---|---|---|---|---|
| Tài khoản công cụ nội bộ tiêu chuẩn | Quản lý/HR/nhân sự theo luồng | Owner hệ thống/IT Lead | IT được phân công | Owner hoặc quản lý |
| Quyền quản trị nội bộ | IT Lead/Owner | Owner hệ thống + cấp có thẩm quyền | Admin được chỉ định | Người rà soát độc lập |
| Quyền tenant khách hàng | Mstar/đầu mối khách hàng | Khách hàng có thẩm quyền và IT Lead theo hợp đồng | Kỹ thuật viên được chỉ định | Khách hàng Owner/Service Owner |
| Quyền đặc quyền/tạm thời | Ticket có lý do và thời hạn | IT Lead/Security + khách hàng nếu thuộc hệ thống khách hàng | Kỹ thuật viên được chỉ định | Hậu kiểm log |
| Break-glass | Incident khẩn cấp | Theo playbook/ủy quyền khẩn cấp | Người được ủy quyền | Hậu kiểm bắt buộc |
| Quyền nhà cung cấp | Owner dịch vụ | IT Lead + khách hàng nếu liên quan khách hàng | Admin được chỉ định | Owner xác nhận thu hồi |

## 5. Chu kỳ rà soát baseline
- Tài khoản đặc quyền: tối thiểu hằng quý và sau sự cố/thay đổi vai trò.
- Quyền thông thường: tối thiểu 6 tháng/lần hoặc theo yêu cầu hợp đồng/rủi ro.
- Nhà cung cấp/tài khoản tạm thời: rà soát theo từng lần cấp và trước ngày hết hạn.
- Nhân sự nghỉ việc/điều chuyển: thu hồi/điều chỉnh theo thời điểm hiệu lực được HR và quản lý xác nhận.
- Khách hàng có thể yêu cầu chu kỳ chặt hơn; phụ lục khách hàng là nguồn quyết định.

## 6. Bằng chứng bắt buộc
- Yêu cầu cấp/sửa/thu hồi quyền và phê duyệt.
- Danh tính, vai trò, hệ thống, phạm vi, ngày hiệu lực/hết hạn.
- Log thực hiện và kết quả kiểm tra.
- Biên bản rà soát quyền, phát hiện quyền thừa và bằng chứng khắc phục.
- Báo cáo tài khoản không dùng, tài khoản chung, MFA và ngoại lệ.

## 7. Checklist rà soát quyền
- [ ] Có owner và mục đích nghiệp vụ.
- [ ] Quyền phù hợp nhiệm vụ, không vượt phạm vi.
- [ ] Có phê duyệt trước khi cấp, trừ luồng khẩn cấp được quy định.
- [ ] MFA và log được bật khi áp dụng.
- [ ] Tài khoản có thời hạn khi cần; tài khoản không dùng đã xử lý.
- [ ] Quyền nhà cung cấp/tạm thời được thu hồi đúng hạn.
- [ ] Bằng chứng được lưu và ticket được đóng.
