# REG-04 — Statement of Applicability (SoA) — Bảng tuyên bố áp dụng

> **Dự thảo làm việc, không phải SoA chính thức.** Phải xác định phạm vi ISMS, đánh giá rủi ro, yêu cầu pháp lý/hợp đồng và kiểm soát cần thiết trước khi chốt. Danh mục kiểm soát phải đối chiếu bản tiêu chuẩn ISO/IEC 27001:2022 có bản quyền và các sửa đổi áp dụng; không coi bảng gợi ý này là danh mục đầy đủ/chính thức.

## 1. Mục tiêu và quy tắc
SoA ghi rõ kiểm soát cần thiết, lý do đưa vào, trạng thái triển khai và lý do loại trừ khi có căn cứ. “Không áp dụng” không được chọn chỉ vì chưa triển khai hoặc thiếu ngân sách. Trạng thái “đã triển khai” phải có bằng chứng vận hành, không chỉ có tài liệu.

## 2. Trường SoA
| Trường | Nội dung |
|---|---|
| Control ID/name | Mã/tên theo bản tiêu chuẩn được cấp phép |
| Source | Rủi ro, yêu cầu hợp đồng/pháp lý, yêu cầu kinh doanh hoặc tham chiếu kiểm soát |
| Applicable? | Có/Không |
| Inclusion/exclusion rationale | Lý do đưa vào hoặc loại trừ |
| Implementation status | Chưa bắt đầu/Đang triển khai/Đã triển khai/Không áp dụng có lý do |
| Owner | Người chịu trách nhiệm |
| Related policy/procedure | Mã tài liệu kiểm soát |
| Evidence ID | Bằng chứng vận hành |
| Gap/action | Thiếu hụt, hành động, owner, hạn |
| Approval/review date | Người duyệt và ngày rà soát |

## 3. Khung nhóm kiểm soát cần đánh giá
Đối chiếu với Annex A ISO/IEC 27001:2022; các nhóm dưới đây chỉ là khung tổ chức, không thay thế danh mục kiểm soát chuẩn:
- **Organizational:** chính sách, vai trò, phân tách nhiệm vụ, threat intelligence, dự án, tài sản, dữ liệu, truy cập, nhà cung cấp, incident, continuity, tuân thủ.
- **People:** sàng lọc phù hợp, điều khoản nhân sự, nhận thức, kỷ luật, trách nhiệm khi chấm dứt/đổi vai trò, bảo mật từ xa.
- **Physical:** khu vực, kiểm soát ra vào, thiết bị, phương tiện lưu trữ, bảo vệ khỏi mất điện/tác động môi trường, bàn làm việc sạch.
- **Technological:** danh tính/xác thực, quyền, endpoint, cấu hình, xóa dữ liệu, masking, DLP khi cần, backup, logging, monitoring, clock sync, network, cryptography, secure development, vulnerability, audit test.

## 4. Bảng làm việc
| Control ID | Control name theo tiêu chuẩn | Nguồn yêu cầu/rủi ro | Áp dụng? | Lý do | Trạng thái | Owner | Quy trình/tài liệu | Evidence ID | Gap/action | Hạn | Người duyệt |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Điền theo bản tiêu chuẩn được cấp phép |  |  | Có/Không |  | Chưa/Đang/Đã/Không áp dụng |  |  |  |  |  |  |

## 5. Cổng phê duyệt SoA
- [ ] Phạm vi ISMS và ranh giới đã được duyệt.
- [ ] Rủi ro và yêu cầu hợp đồng/pháp lý đã được xem xét.
- [ ] Tất cả kiểm soát trong danh mục chuẩn đã được đánh giá, không bỏ qua vì chưa triển khai.
- [ ] Lý do áp dụng/loại trừ có căn cứ.
- [ ] Trạng thái triển khai được xác minh bằng bằng chứng.
- [ ] Thiếu hụt có owner, hạn và nguồn lực.
- [ ] SoA được phê duyệt và có ngày rà soát.
