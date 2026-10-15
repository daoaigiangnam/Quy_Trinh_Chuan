# KPI-01 — Từ điển KPI vận hành và tuân thủ

> KPI là công cụ giám sát, không thay thế kiểm soát. Mỗi KPI phải được chủ sở hữu dữ liệu và người duyệt xác nhận công thức, nguồn, loại trừ, chu kỳ và mục tiêu theo hợp đồng/rủi ro.

| KPI ID | Chỉ số | Định nghĩa/công thức | Nguồn | Chu kỳ | Owner | Cảnh báo khi |
|---|---|---|---|---|---|---|
| KPI-01 | Tỷ lệ ticket đạt SLA | Ticket đủ điều kiện đạt SLA / tổng ticket đủ điều kiện × 100% | Bitrix24 | Tháng | Service Owner | Dưới mục tiêu hợp đồng |
| KPI-02 | Tỷ lệ ticket quá hạn | Ticket quá hạn chưa đóng / tổng ticket mở đủ điều kiện × 100% | Bitrix24 | Tuần/tháng | ITL | Tăng vượt ngưỡng nội bộ |
| KPI-03 | Tỷ lệ reopen | Ticket bị mở lại / ticket đã đóng trong kỳ × 100% | Bitrix24 | Tháng | Service Owner | Tăng bất thường |
| KPI-04 | Thời gian phản hồi P1 | Thời gian từ mốc bắt đầu SLA đến phản hồi đầu tiên theo định nghĩa hợp đồng | Bitrix24 | Mỗi P1/tháng | Service Desk Lead | Vi phạm mục tiêu |
| KPI-05 | Tỷ lệ hoàn tất rà soát quyền | Rà soát hoàn tất / rà soát đến hạn × 100% | IAM/access register | Tháng/quý | System Owner | Có rà soát quá hạn |
| KPI-06 | Tỷ lệ thu hồi quyền đúng hạn | Quyền thu hồi đúng hạn / quyền phải thu hồi × 100% | IAM/HR checklist | Tháng | ITL/HR | Bất kỳ quyền rủi ro cao bị trễ |
| KPI-07 | Tỷ lệ backup thành công | Job backup thành công / tổng job dự kiến × 100% | Backup console | Ngày/tháng | Backup Owner | Job quan trọng lỗi |
| KPI-08 | Tỷ lệ restore test đạt | Test đạt / test đã thực hiện × 100% | Restore test reports | Theo kế hoạch | Backup Owner | Test không đạt hoặc quá hạn |
| KPI-09 | Tỷ lệ patch đúng hạn | Tài sản đã vá đúng hạn / tài sản phải vá × 100% | Patch/vulnerability register | Tháng | ITL/SEC | Lỗ hổng trọng yếu quá hạn |
| KPI-10 | Thời gian xử lý incident | Thời gian từ phát hiện đến containment/recovery theo định nghĩa từng mức độ | Incident register | Mỗi incident/tháng | Incident Lead | Vượt mục tiêu |
| KPI-11 | CAPA đúng hạn | Hành động đóng đúng hạn / hành động đến hạn × 100% | CAPA register | Tháng | ISMS/Owner | Hành động nghiêm trọng quá hạn |
| KPI-12 | Bằng chứng kiểm soát đầy đủ | Bằng chứng đạt / bằng chứng đến hạn × 100% | Evidence register | Tháng/quý | ISMS/Control Owner | Thiếu bằng chứng kiểm soát trọng yếu |
| KPI-13 | Ngoại lệ quá hạn | Số ngoại lệ quá ngày hết hạn chưa đóng | Exception register | Tuần/tháng | ISMS | Bất kỳ ngoại lệ nghiêm trọng quá hạn |
| KPI-14 | Tỷ lệ tài sản có owner | Tài sản có owner/criticality/record hợp lệ / tổng tài sản trong phạm vi × 100% | CMDB | Tháng/quý | Asset Owner | Thiếu tài sản trọng yếu |
| KPI-15 | Tỷ lệ đào tạo đạt | Nhân sự đạt yêu cầu / nhân sự phải đào tạo × 100% | HR/LMS | Theo kế hoạch | HR/ISMS | Có vai trò trọng yếu chưa đào tạo |
| KPI-16 | Tỷ lệ tuân thủ customer appendix | Trường/kiểm soát bắt buộc đã hoàn tất / tổng trường bắt buộc × 100% | Customer appendix | Tháng/quý | Service Owner | Thiếu quyền/SLA/incident contact |
| KPI-17 | Tỷ lệ change thành công | Change không gây rollback/incident nghiêm trọng / tổng change hoàn tất × 100% | Change register | Tháng | Change Owner | Thay đổi thất bại tăng |
| KPI-18 | Tỷ lệ thông báo sự cố đúng hạn | Thông báo đúng hạn theo nghĩa vụ / sự cố phải thông báo × 100% | Incident/customer notification log | Mỗi incident/tháng | Incident Lead | Bất kỳ vi phạm nghĩa vụ |
| KPI-19 | Tỷ lệ vendor review đúng hạn | Vendor review hoàn tất / review đến hạn × 100% | Vendor register | Quý/năm | Vendor Owner | Vendor trọng yếu quá hạn |
| KPI-20 | Tỷ lệ kiểm soát có bằng chứng hiệu lực | Kiểm soát đã kiểm tra hiệu lực / kiểm soát đến hạn kiểm tra × 100% | Audit/evidence register | Quý/năm | ISMS | Kiểm soát trọng yếu không hiệu lực |

## Quy tắc quản trị KPI
1. Định nghĩa mốc thời gian, mẫu số, loại trừ và xử lý dữ liệu thiếu trước khi đo.
2. Không đổi công thức hồi tố nếu chưa phê duyệt và ghi lịch sử phiên bản.
3. KPI mục tiêu khách hàng phải lấy từ hợp đồng/SLA; không áp dụng một ngưỡng mặc định cho mọi khách hàng.
4. Với chỉ số “0 sự cố” không được hiểu là chứng minh hệ thống an toàn; phải kết hợp chỉ số kiểm soát và bằng chứng.
5. Mỗi chỉ số vượt ngưỡng phải có phân tích nguyên nhân, owner, hạn và kiểm tra hiệu lực.
