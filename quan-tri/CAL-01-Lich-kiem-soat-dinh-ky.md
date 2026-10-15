# CAL-01 — Lịch kiểm soát định kỳ

> **Dự thảo lịch mẫu.** Điều chỉnh theo rủi ro, năng lực, hợp đồng và SoA. Nếu hợp đồng yêu cầu tần suất chặt hơn thì áp dụng yêu cầu đã ký.

| Tần suất gợi ý | Hoạt động | Owner | Bằng chứng | Điều kiện kích hoạt bổ sung |
|---|---|---|---|---|
| Mỗi ca/ngày làm việc | Kiểm tra cảnh báo P1, tình trạng dịch vụ và backup job quan trọng | IT Operations | Alert/ticket/job report | Alert nghiêm trọng/sự cố |
| Hằng tuần | Rà soát ticket quá hạn, SLA, backlog, lỗi backup, domain/SSL gần hạn | Service Owner | Báo cáo tuần/action tracker | Khách hàng trọng yếu |
| Hằng tháng | Báo cáo SLA/KPI; xem xu hướng incident; rà soát tài khoản không dùng; xác nhận patch/vulnerability backlog | ITL/Service Owner | Monthly service report | Sự cố/biến động lớn |
| Hằng quý | Rà soát quyền đặc quyền; rule firewall; vendor trọng yếu; ngoại lệ sắp hết hạn; test khôi phục mẫu theo kế hoạch | ITL/SEC/Owner | Access review, firewall review, vendor review, restore evidence | Thay đổi kiến trúc/sự cố |
| 6 tháng/lần | Rà soát quyền thông thường; kiểm tra tính đầy đủ inventory; đánh giá nhận thức/đào tạo bổ sung | System Owner/HR | Access review, asset reconciliation, training | Theo hợp đồng/rủi ro |
| Hằng năm | Rà soát chính sách, risk assessment, SoA, BIA/BCP, chương trình audit, mục tiêu ATTT, management review | ISMS/BGĐ | Biên bản, risk register, SoA, audit plan | Thay đổi phạm vi/rủi ro |
| Theo từng sự kiện | Onboarding/offboarding, cấp quyền, change, incident, chuyển dữ liệu, vendor onboarding/exit | Process Owner | Ticket/form/approval/log | Mỗi sự kiện |
| Trước hết hạn | Domain/SSL/license/cert, quyền tạm thời, ngoại lệ, hợp đồng/vendor | Asset/Service Owner | Expiry register/renewal approval | Theo ngưỡng cảnh báo đã đặt |
| Sau change | Kiểm thử chức năng, log/monitoring, bảo mật, backup/rollback readiness | Change Owner + reviewer | Test evidence/post-change review | Mỗi change |
| Sau incident | RCA, evidence preservation, customer update, CAPA, review risk/SoA khi liên quan | Incident Lead/ISMS | Incident file/RCA/CAPA | Mỗi incident phù hợp |
| Theo kế hoạch được duyệt | Restore test, BCP/DR exercise, tabletop incident exercise | BCP/ITL/SEC | Test/exercise report | Khi hệ thống hoặc RTO/RPO thay đổi |

## Theo dõi thực hiện
| Kỳ | Hoạt động | Phạm vi/khách hàng | Kết quả dự kiến | Owner | Hạn | Bằng chứng ID | Trạng thái | Ngoại lệ/Action |
|---|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  | Chưa đến hạn/Đang làm/Đạt/Không đạt/Trễ |  |

## Quy tắc quá hạn
1. Ghi nhận nguyên nhân, mức rủi ro và dịch vụ/khách hàng bị ảnh hưởng.
2. Gán owner và hạn khắc phục mới; phê duyệt nếu cần chấp nhận rủi ro tồn dư.
3. Thông báo khách hàng nếu hợp đồng hoặc mức ảnh hưởng yêu cầu.
4. Không đánh dấu hoàn tất nếu thiếu bằng chứng hoặc chưa xác minh hiệu lực.
