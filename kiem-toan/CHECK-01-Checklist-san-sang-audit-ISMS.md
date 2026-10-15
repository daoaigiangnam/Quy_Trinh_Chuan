# CHECK-01 — Checklist sẵn sàng kiểm tra nội bộ ISMS/IT Outsourcing

> Checklist khởi tạo, không phải tuyên bố tuân thủ/chứng nhận. Đánh giá theo phạm vi ISMS, tiêu chuẩn được cấp phép, yêu cầu pháp lý/hợp đồng và SoA đã phê duyệt.

| ID | Chủ đề | Câu hỏi kiểm tra | Bằng chứng cần xem | Owner | Kết quả | Finding ID / hành động |
|---|---|---|---|---|---|---|
| AUD-001 | Phạm vi | Phạm vi ISMS, địa điểm, dịch vụ, ranh giới và giao diện đã được xác định/duyệt? | Scope statement, sơ đồ | ISMS |  |  |
| AUD-002 | Bối cảnh/lãnh đạo | Vai trò, chính sách, mục tiêu, trách nhiệm và nguồn lực đã rõ? | Policy, RACI, mục tiêu | BGĐ/ISMS |  |  |
| AUD-003 | Rủi ro | Có phương pháp, risk register, kế hoạch xử lý và chấp nhận rủi ro tồn dư? | Risk register, approvals | ISMS/Owner |  |  |
| AUD-004 | SoA | Kiểm soát áp dụng/loại trừ có căn cứ và trạng thái có bằng chứng? | SoA, evidence refs | ISMS |  |  |
| AUD-005 | Tài liệu | Có version, phê duyệt, kiểm soát bản cũ và retention? | Document register | Document Owner |  |  |
| AUD-006 | Nghĩa vụ | Hợp đồng/SLA/pháp lý được chuyển thành kiểm soát vận hành? | Contract checklist, obligations | Sale/Legal/ITL |  |  |
| AUD-007 | Nhân sự | Onboarding, cam kết, đào tạo, thay đổi vai trò và offboarding được thực hiện? | HR checklists, access logs | HR/ITL |  |  |
| AUD-008 | Tài sản/dữ liệu | Tài sản và dữ liệu có owner, phân loại, vị trí, quyền và retention? | Inventory, data register | Asset/Data Owner |  |  |
| AUD-009 | Truy cập | Cấp quyền có phê duyệt, MFA khi cần, quyền tối thiểu, rà soát và thu hồi? | Requests, access review, logs | ITL/System Owner |  |  |
| AUD-010 | Đặc quyền/secrets | Quyền admin, vault, break-glass và rotate secret có kiểm soát/hậu kiểm? | Privileged account register | ITL/SEC |  |  |
| AUD-011 | Nhà cung cấp | Có thẩm định, điều khoản, giám sát và quy trình exit? | Vendor register, contracts | Vendor Owner |  |  |
| AUD-012 | Ticket/SLA | Ticket có timestamp, phân loại, xử lý, escalation, xác nhận và báo cáo? | Bitrix24 sample, SLA report | Service Owner |  |  |
| AUD-013 | Change/config | Thay đổi có risk, approval, test, rollback và hậu kiểm? Baseline có kiểm tra drift? | Change records, baseline | ITL |  |  |
| AUD-014 | Monitoring/log | Log được bảo vệ, đồng bộ thời gian, retention và review theo rủi ro? | Logging matrix, review records | SEC/ITL |  |  |
| AUD-015 | Lỗ hổng/patch | Có inventory, ưu tiên, SLA khắc phục, retest và exception? | Vulnerability register | SEC/ITL |  |  |
| AUD-016 | Endpoint/network | Thiết bị, firewall, VPN, remote access và rule có baseline/review? | Compliance report, firewall review | ITL |  |  |
| AUD-017 | Backup/restore | Job được giám sát; restore test chứng minh tính toàn vẹn và thời gian phục hồi? | Backup report, restore test | Backup Owner |  |  |
| AUD-018 | BCP/DR | Có BIA, RTO/RPO, kế hoạch, danh bạ và diễn tập/khắc phục? | BIA, exercise report | BCP Owner |  |  |
| AUD-019 | Incident | Có triage, containment, escalation, customer notification, evidence, RCA/CAPA? | Incident files | Incident Lead |  |  |
| AUD-020 | Dữ liệu khách hàng | Chia sẻ, trả/xóa dữ liệu và quyền bên thứ ba được phê duyệt/truy nguyên? | Transfer/deletion records | Data Owner |  |  |
| AUD-021 | Audit/CAPA | Audit độc lập, findings có nguyên nhân gốc, owner, hạn và xác minh hiệu lực? | Audit plan, CAPA log | ISMS |  |  |
| AUD-022 | Management review | Lãnh đạo xem xét KPI, risk, incident, audit, khách hàng, nguồn lực và hành động? | Meeting minutes/action log | BGĐ/ISMS |  |  |
| AUD-023 | Phụ lục khách hàng | Có scope, SLA, hệ thống, quyền, đầu mối, retention, incident notification và exit? | Customer appendix | Service Owner |  |  |
| AUD-024 | Bằng chứng | Có thể truy nguyên bằng chứng về người, thời điểm, nguồn, kiểm soát và kỳ lưu? | Evidence register/samples | Control Owners |  |  |

## Kết quả kiểm tra
| Trường | Nội dung |
|---|---|
| Phạm vi/đơn vị/khách hàng |  |
| Tiêu chí và phiên bản tiêu chuẩn |  |
| Ngày kiểm tra |  |
| Người kiểm tra và tính độc lập |  |
| Số mục đạt / không đạt / không áp dụng |  |
| Finding mức nghiêm trọng/cao/trung bình/thấp |  |
| Kết luận và giới hạn đánh giá |  |
| Người phê duyệt báo cáo |  |

## Quy tắc phân loại phát hiện (gợi ý)
- **Nghiêm trọng:** có khả năng gây ảnh hưởng lớn đến tính bảo mật/toàn vẹn/sẵn sàng hoặc vi phạm nghĩa vụ trọng yếu; xử lý khẩn cấp.
- **Cao:** kiểm soát quan trọng không vận hành hoặc thiếu bằng chứng nghiêm trọng.
- **Trung bình:** thiếu sót có phạm vi giới hạn nhưng cần kế hoạch khắc phục.
- **Thấp/quan sát:** cải tiến hoặc lỗi hồ sơ ít ảnh hưởng.
- **Không phù hợp:** phải ghi tiêu chí, bằng chứng khách quan, phạm vi, owner và thời hạn; không kết luận chỉ dựa trên ý kiến.
