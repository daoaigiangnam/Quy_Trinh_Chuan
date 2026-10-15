# MA-01 — Ma trận trách nhiệm RACI chuẩn Mstar

> **Trạng thái:** Dự thảo v0.1 — chưa ban hành. Điều chỉnh chức danh theo cơ cấu thực tế và phụ lục từng khách hàng. RACI không thay thế ma trận phê duyệt tài chính/hợp đồng.

## 1. Quy ước
- **R — Responsible:** trực tiếp thực hiện.
- **A — Accountable:** chịu trách nhiệm cuối cùng; mỗi hoạt động nên có một A duy nhất.
- **C — Consulted:** được tham vấn trước quyết định.
- **I — Informed:** được thông báo.
- Nếu một hoạt động chạm hệ thống/dữ liệu khách hàng, cần phê duyệt của khách hàng theo hợp đồng, quyền được ủy quyền và ma trận khách hàng.

## 2. Vai trò
- **BGĐ:** Ban Giám đốc/người được ủy quyền.
- **ISMS:** Chủ sở hữu ISMS/điều phối ATTT.
- **ITL:** IT Lead/Technical Service Owner.
- **SD:** Service Desk/L1.
- **ENG:** Kỹ thuật viên L2/L3.
- **SEC:** Đầu mối ứng cứu sự cố/bảo mật.
- **SAL:** Sale/Account Manager.
- **HR:** Nhân sự.
- **FIN/LEG:** Tài chính/pháp chế hoặc tư vấn được chỉ định.
- **CUS:** Chủ dịch vụ/đầu mối được khách hàng ủy quyền.
- **SUP:** Nhà cung cấp/bên thứ ba.

## 3. Ma trận RACI

| Hoạt động | BGĐ | ISMS | ITL | SD | ENG | SEC | SAL | HR | FIN/LEG | CUS | SUP |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Phê duyệt chính sách ATTT | A | R | C | I | I | C | I | C | C | I | I |
| Xác định phạm vi ISMS | A | R | C | I | I | C | C | I | C | I | I |
| Đánh giá rủi ro ISMS | A | R | R | C | C | C | I | C | C | C | I |
| Phê duyệt chấp nhận rủi ro cao | A | R | C | I | I | C | I | I | C | C* | I |
| Quản lý tài liệu/quy trình | I | A/R | R | I | C | C | C | C | C | I | I |
| Thẩm định hợp đồng/phạm vi/SLA | A* | C | C | I | I | C | R | I | C | C | I |
| Onboarding khách hàng | I | C | A | R | R | C | C | I | I | C/A* | C |
| Tiếp nhận và phân loại ticket | I | I | A | R | C | C | I | I | I | C | I |
| Xử lý sự cố dịch vụ thông thường | I | I | A | R | R | C | I | I | I | C | C |
| Xử lý sự cố ATTT | I/A* | C | C | R | R | A/R | I | I | C | C/I* | C |
| Cấp quyền trên hệ thống Mstar | I | C | A | R | C | C | I | C | I | I | I |
| Cấp quyền trên hệ thống khách hàng | I | C | R | R | R | C | I | I | I | A* | I |
| Quyền đặc quyền/break-glass | I/A* | C | A | I | R | R/C | I | I | I | A* | I |
| Thay đổi hệ thống Mstar | I | C | A | C | R | C | I | I | I | I | C |
| Thay đổi hệ thống khách hàng | I | C | R | C | R | C | I | I | I | A* | C |
| Backup và kiểm tra backup | I | C | A | I | R | C | I | I | I | C | C |
| Kiểm thử khôi phục | I | C | A | I | R | C | I | I | I | C/A* | C |
| Rà soát quyền định kỳ | I | C | A | R | C | C | I | C | I | A* | C |
| Quản lý tài sản | I | C | A | R | R | C | I | C | I | C | C |
| Quản lý nhà cung cấp | A* | C | R | I | C | C | R | I | C | I | R |
| Nhân sự vào/điều chuyển/nghỉ | I | C | R | I | I | C | I | A/R | I | I | I |
| Thông báo sự cố cho khách hàng | I/A* | C | R | I | C | R | C | I | C | I | I |
| Báo cáo SLA/KPI | I | C | A | R | C | C | C | I | I | C | I |
| Kiểm toán nội bộ | A | R | C | C | C | C | I | C | C | I | I |
| Khắc phục phát hiện audit | I/A* | C | A/R | R | R | R | I | C | C | C | C |
| Exit, thu hồi quyền, trả/xóa dữ liệu | I | C | R | R | R | C | A/R | C | C | A* | C |

`A*` có nghĩa là cấp phê duyệt thay đổi theo thẩm quyền, hợp đồng, loại rủi ro hoặc phạm vi hệ thống; cần xác định rõ trong phụ lục khách hàng. Với sự cố ATTT, không trì hoãn biện pháp cô lập cần thiết chỉ để chờ họp; tuân thủ playbook và thẩm quyền khẩn cấp đã phê duyệt.

## 4. Nguyên tắc phân tách nhiệm vụ
1. Người yêu cầu không tự duyệt quyền của chính mình.
2. Người thực hiện thay đổi rủi ro cao không tự nghiệm thu duy nhất.
3. Người chấp nhận rủi ro tồn dư phải có thẩm quyền tương ứng với mức rủi ro.
4. Quyền khách hàng chỉ được cấp khi có ủy quyền hợp lệ; không dùng tài khoản chung nếu có thể cấp danh tính riêng.
5. Trường hợp thiếu nhân sự không thể phân tách, ghi nhận ngoại lệ, kiểm soát bù trừ và hậu kiểm độc lập.

## 5. Hồ sơ cần lưu
- Phiếu yêu cầu/phê duyệt; ticket/change/incident liên quan.
- Nhật ký thực hiện và bằng chứng kiểm tra.
- Danh sách ngoại lệ và phê duyệt bù trừ.
- Biên bản rà soát RACI ít nhất hằng năm hoặc khi thay đổi cơ cấu/dịch vụ.

## 6. Phê duyệt
| Vai trò | Họ tên | Ý kiến | Ngày |
|---|---|---|---|
| Chủ sở hữu tài liệu |  |  |  |
| Rà soát IT Lead |  |  |  |
| Rà soát ISMS |  |  |  |
| Phê duyệt BGĐ |  |  |  |
