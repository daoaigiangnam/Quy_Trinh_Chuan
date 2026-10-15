# REG-01 — Danh mục bằng chứng vận hành

> **Mục tiêu:** Định nghĩa bằng chứng tối thiểu để chứng minh quy trình được thực hiện. Không phải mọi khách hàng đều cần mọi bằng chứng; chọn theo phạm vi dịch vụ, rủi ro, hợp đồng và SoA.

## 1. Quy tắc quản lý bằng chứng
Mỗi bằng chứng cần có: **Evidence ID, quy trình/kiểm soát, khách hàng hoặc phạm vi, kỳ/thời điểm, người tạo, người rà soát, nguồn, vị trí lưu, phân loại, retention, trạng thái và liên kết ticket/change/incident**. Lưu bản gốc hoặc nguồn có thể truy nguyên; hạn chế ảnh chụp màn hình không có ngữ cảnh. Không lưu mật khẩu, token, khóa riêng hoặc dữ liệu khách hàng vượt nhu cầu.

## 2. Danh mục bằng chứng tối thiểu

| ID | Quy trình/kiểm soát | Bằng chứng cần lưu | Owner | Tần suất/trigger | Người rà soát | Nơi lưu tham chiếu |
|---|---|---|---|---|---|---|
| EV-001 | Chính sách ATTT | Chính sách phiên bản hiện hành, phê duyệt, lịch sử thay đổi | ISMS | Khi ban hành/thay đổi; rà soát năm | BGĐ/ISMS | Kho ISMS |
| EV-002 | Phạm vi ISMS | Phạm vi, sơ đồ ranh giới, giao diện/phụ thuộc | ISMS | Năm/lần hoặc đổi phạm vi | BGĐ | Kho ISMS |
| EV-003 | Đánh giá rủi ro | Risk register, phương pháp, phê duyệt xử lý | ISMS/Owner | Năm/lần và khi thay đổi trọng yếu | BGĐ/Owner | Kho ISMS hạn chế |
| EV-004 | SoA | SoA có lý do áp dụng/không áp dụng, trạng thái triển khai | ISMS | Khi thay đổi rủi ro/phạm vi/kiểm soát | BGĐ | Kho ISMS |
| EV-005 | Năng lực/đào tạo | Kế hoạch, tham dự, kết quả, đào tạo bù | HR/ISMS | Theo kế hoạch; khi onboarding | Quản lý | HR/ISMS |
| EV-006 | Nghĩa vụ hợp đồng/pháp lý | Sổ nghĩa vụ, đánh giá hợp đồng, chuyển yêu cầu thành kiểm soát | Sale/Legal/ITL | Trước ký/gia hạn và khi đổi | BGĐ/ITL | Hợp đồng hạn chế |
| EV-007 | Tài sản | CMDB/inventory, owner, phân loại, kiểm kê | ITL | Cập nhật khi thay đổi; kiểm kê theo rủi ro | Owner | CMDB |
| EV-008 | Phân loại dữ liệu | Danh mục dữ liệu, owner, nơi lưu, retention | Data/System Owner | Khi tạo/thay đổi; rà soát định kỳ | ISMS/Owner | Kho hạn chế |
| EV-009 | Cấp quyền | Phiếu yêu cầu, phê duyệt, log cấp, xác minh | ITL/System Owner | Mỗi lần cấp/đổi/thu hồi | Owner độc lập | Ticket/IAM |
| EV-010 | Rà soát quyền | Danh sách quyền, quyết định giữ/thu hồi, xác nhận hoàn tất | System Owner | Theo chu kỳ rủi ro/hợp đồng | ITL/ISMS | IAM |
| EV-011 | Quyền đặc quyền | Inventory admin, MFA, vault metadata, log và hậu kiểm | ITL/SEC | Mỗi lần dùng; rà soát quý | Security/Owner | Vault/SIEM |
| EV-012 | Nhà cung cấp | Thẩm định, hợp đồng, quyền truy cập, đánh giá định kỳ | Owner/Sale | Trước sử dụng và khi gia hạn/thay đổi | ITL/ISMS | Vendor register |
| EV-013 | Ticket/SLA | Ticket, timestamp, ưu tiên, phản hồi, giải quyết, xác nhận | Service Desk | Mỗi ticket; báo cáo kỳ | Service Owner | Bitrix24 |
| EV-014 | Thay đổi | RFC, risk, approval, test, rollback, hậu kiểm | Change Owner | Mỗi change | Người duyệt độc lập | Bitrix24/Change log |
| EV-015 | Cấu hình | Baseline, drift, ngoại lệ, kết quả rà soát | System Owner | Theo thay đổi/chu kỳ | ITL | CMDB/Config repo |
| EV-016 | Monitoring | Cấu hình cảnh báo, alert, xử lý, downtime | IT Operations | Liên tục; review theo ca/kỳ | ITL | Monitoring/SIEM |
| EV-017 | Lỗ hổng/patch | Scan, mức độ, kế hoạch, change, retest, ngoại lệ | Security/ITL | Theo lịch scan/patch | IT Lead | Vulnerability register |
| EV-018 | Endpoint | Báo cáo EDR, encryption, patch, compliance, exception | IT Operations | Theo dashboard/chu kỳ | ITL/SEC | Endpoint console |
| EV-019 | Firewall/VPN | Request, approval, rule diff, log, review/expiry | Network Owner | Mỗi rule; rà soát định kỳ | ITL/SEC | Change repository |
| EV-020 | Backup | Policy/job result, lỗi, cảnh báo, khắc phục | Backup Owner | Mỗi job/kỳ | ITL | Backup console |
| EV-021 | Restore test | Kịch bản, log, thời gian, integrity/function test, gap | Backup Owner | Theo rủi ro/hợp đồng; tối thiểu theo kế hoạch được duyệt | ITL/Customer Owner nếu cần | DR evidence |
| EV-022 | Incident | Timeline, severity, decisions, evidence, notification, RCA | Incident Lead | Mỗi sự cố | ITL/ISMS | Incident repository |
| EV-023 | Bằng chứng điều tra | Hash, người thu, thời gian, nguồn, chain of custody | Incident Lead | Mỗi vụ cần bảo toàn | Security/Legal khi cần | Kho hạn chế |
| EV-024 | BCP/DR | BIA, kế hoạch, diễn tập, kết quả, corrective action | BCP Owner | Theo kế hoạch và khi đổi trọng yếu | BGĐ/Service Owner | BCP/DR repository |
| EV-025 | Domain/SSL | Inventory, expiry alert, gia hạn, xác minh DNS/TLS | Service Owner | Theo lịch kiểm tra/cảnh báo | ITL | CMDB |
| EV-026 | Nhân sự vào/điều chuyển/nghỉ | Checklist HR, cấp/đổi/thu hồi quyền, tài sản, bàn giao | HR/ITL | Mỗi sự kiện | HR/Manager | HR hạn chế |
| EV-027 | Offboarding vendor | Thu hồi quyền, token, dữ liệu, xác nhận xóa/trả | Vendor Owner | Khi kết thúc | ITL/Customer Owner | Vendor register |
| EV-028 | Dữ liệu khách hàng | Phê duyệt chia sẻ, người nhận, transfer log, xóa/trả | Data Owner | Mỗi lần chia sẻ/exit | Customer Owner | Kho khách hàng hạn chế |
| EV-029 | Kiểm toán nội bộ | Kế hoạch, mẫu, bằng chứng, phát hiện, báo cáo | Auditor/ISMS | Theo chương trình | BGĐ | Audit repository |
| EV-030 | CAPA | Nguyên nhân gốc, hành động, owner, hạn, xác minh hiệu lực | Process Owner | Mỗi phát hiện | ISMS/Owner độc lập | CAPA register |
| EV-031 | KPI/SLA | Định nghĩa, nguồn dữ liệu, tính toán, báo cáo, phê duyệt | Service Owner | Theo kỳ báo cáo | ITL/Customer Owner | Reporting |
| EV-032 | Xem xét lãnh đạo | Đầu vào, biên bản, quyết định, nguồn lực và action | ISMS | Theo lịch quản trị | BGĐ | Kho ISMS |
| EV-033 | Ngoại lệ | Risk assessment, bù trừ, approver, expiry, closure | Control Owner | Mỗi ngoại lệ; trước hết hạn | ISMS/Owner | Exception register |
| EV-034 | Quản lý tài liệu | Danh mục, version, approval, distribution, retirement | Document Controller | Mỗi thay đổi; review định kỳ | ISMS | Document repository |
| EV-035 | Bàn giao dịch vụ | Inventory, sơ đồ, access, SLA, risk/gap, acceptance | Service Owner | Mỗi onboarding/exit | ITL/Customer Owner | Customer folder |

## 3. Metadata bắt buộc cho từng bản ghi bằng chứng
| Trường | Yêu cầu |
|---|---|
| Evidence ID | Mã duy nhất, không tái sử dụng |
| Control/Procedure ID | Mã quy trình/kiểm soát liên quan |
| Scope/customer | Phạm vi hoặc khách hàng, tránh trộn dữ liệu khách hàng |
| Period/timestamp | Kỳ và múi giờ rõ ràng |
| Source | Hệ thống nguồn, ticket ID, report ID hoặc log query |
| Owner/reviewer | Người tạo và người rà soát |
| Integrity | Hash/checksum khi phù hợp; quyền sửa hạn chế |
| Classification | Phân loại thông tin |
| Location/access | Kho lưu chính thức và nhóm được truy cập |
| Retention/disposal | Thời hạn, căn cứ, cách hủy và legal hold nếu có |
| Status | Đã thu thập / Đang xác minh / Đạt / Thiếu / Khắc phục |

## 4. Điều kiện bằng chứng đạt
- Có thể truy nguyên tới người thực hiện, thời điểm, hệ thống nguồn và yêu cầu kiểm soát.
- Có nội dung đủ để tái kiểm tra; không chỉ là tick “đã làm”.
- Được bảo vệ khỏi sửa/xóa trái phép; có phân quyền và lịch lưu giữ.
- Nếu thiếu, mở finding/action có owner, mức độ, hạn và phê duyệt rủi ro tồn dư.
- Mẫu bằng chứng, tần suất và thời hạn lưu cuối cùng phải theo rủi ro, hợp đồng, nghĩa vụ pháp lý và SoA đã duyệt.
