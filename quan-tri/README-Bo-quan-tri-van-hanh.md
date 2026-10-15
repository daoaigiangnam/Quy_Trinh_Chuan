# Bộ quản trị vận hành, phân quyền và bằng chứng chuẩn Mstar

**Mục tiêu:** Bổ sung các thành phần quản trị để bộ quy trình IT Outsourcing có thể vận hành nhất quán giữa các khách hàng doanh nghiệp và tạo bằng chứng kiểm tra theo hướng ISO/IEC 27001:2022.

> **Trạng thái toàn bộ tài liệu:** Dự thảo v0.1, chưa ban hành. Đây là bộ khung quản trị, không phải tuyên bố Mstar đã được chứng nhận ISO. Phải xác nhận phạm vi ISMS, đánh giá rủi ro, SoA, nghĩa vụ hợp đồng/pháp lý và bằng chứng thực tế trước khi kết luận tuân thủ.

## 1. Bộ tài liệu mới bổ sung

| Mã | Tài liệu | Dùng để |
|---|---|---|
| MA-01 | [Ma trận trách nhiệm RACI](./MA-01-Ma-tran-trach-nhiem-RACI.md) | Ai thực hiện, chịu trách nhiệm cuối, tham vấn, được thông báo |
| MA-02 | [Ma trận phân quyền RBAC](../an-toan-thong-tin/MA-02-Ma-tran-phan-quyen-RBAC.md) | Quyền theo vai trò, phê duyệt cấp quyền, MFA, rà soát/thu hồi |
| REG-01 | [Danh mục bằng chứng vận hành](../van-hanh/REG-01-Danh-muc-bang-chung-van-hanh.md) | Bằng chứng nào cần có, owner, tần suất, nơi lưu, tiêu chí đạt |
| REG-02 | [Danh mục tài liệu, hồ sơ và lưu giữ](./REG-02-Danh-muc-tai-lieu-ho-so-va-luu-giu.md) | Version, phát hành, thu hồi bản cũ, retention và hủy |
| REG-03 | [Sổ đăng ký rủi ro ATTT](./REG-03-So-dang-ky-rui-ro-ATTT.md) | Kịch bản, đánh giá, xử lý và chấp nhận rủi ro tồn dư |
| REG-04 | [SoA — Bảng tuyên bố áp dụng](./REG-04-SoA-bang-tuyen-bo-ap-dung.md) | Kiểm soát áp dụng/loại trừ, lý do, trạng thái, bằng chứng, gap |
| FR-CUS-01 | [Phụ lục chuẩn theo khách hàng](../khach-hang/FR-CUS-01-Phu-luc-chuan-dich-vu-khach-hang.md) | Scope, SLA, systems, access, data, incident, backup/DR, exit |
| CAL-01 | [Lịch kiểm soát định kỳ](./CAL-01-Lich-kiem-soat-dinh-ky.md) | Hoạt động theo ngày/tuần/tháng/quý/năm và theo sự kiện |
| CHECK-01 | [Checklist sẵn sàng audit](../kiem-toan/CHECK-01-Checklist-san-sang-audit-ISMS.md) | Kiểm tra tài liệu, thực thi, bằng chứng, phát hiện và CAPA |
| KPI-01 | [Từ điển KPI vận hành và tuân thủ](../bao-cao/KPI-01-KPI-van-hanh-va-tuan-thu.md) | Theo dõi hiệu lực vận hành và nghĩa vụ SLA/ATTT |

## 2. Bộ quy trình và biểu mẫu liên quan

- [Danh mục quy trình chuẩn](../README.md)
- [Thư viện 41 bộ biểu mẫu](../bieu-mau/README.md)
- [QT-IT-11 — Quy trình quản lý tài khoản và quyền truy cập](../quy-trinh/chi-tiet/QT-IT-11.md)
- [QT-ATTT-04 — Quy trình ứng cứu sự cố ATTT](../quy-trinh/chi-tiet/QT-ATTT-04.md)
- [QT-OPS-01 — Quy trình sao lưu dữ liệu](../quy-trinh/chi-tiet/QT-OPS-01.md)
- [QT-BCP-02 — Quy trình khôi phục sau thảm họa](../quy-trinh/chi-tiet/QT-BCP-02.md)

## 3. Thành phần còn phải hoàn tất trước khi ban hành
1. Chốt phạm vi ISMS, bối cảnh, bên liên quan và giao diện với khách hàng/nhà cung cấp.
2. Phê duyệt phương pháp chấm điểm rủi ro, ngưỡng chấp nhận, risk register thực tế và kế hoạch xử lý.
3. Hoàn tất SoA từ bản ISO/IEC 27001:2022 được cấp phép và yêu cầu liên quan; mọi loại trừ cần lý do.
4. Xác nhận RACI/RBAC theo nhân sự và công cụ thực tế; không cấp quyền rộng chỉ vì vai trò.
5. Chốt retention theo hợp đồng/pháp lý; cấu hình kho lưu, quyền, logging, backup và hủy dữ liệu.
6. Điền phụ lục riêng cho từng khách hàng: SLA, hệ thống, quyền, đầu mối, dữ liệu, thông báo sự cố, RTO/RPO và exit.
7. Chạy thử các quy trình và thu thập bằng chứng thật; mở CAPA cho thiếu hụt.
8. Rà soát độc lập, phê duyệt chính thức, đào tạo nhân sự và đặt lịch review.

## 4. Nguyên tắc quan trọng
- Tài liệu được ban hành không tự chứng minh kiểm soát đã vận hành.
- Không dùng mẫu chung để ghi đè nghĩa vụ riêng trong hợp đồng khách hàng.
- Không lưu mật khẩu, token, API key, khóa riêng hoặc mã khôi phục dạng rõ.
- Bằng chứng phải truy nguyên được, có giới hạn truy cập, retention và cách hủy.
- Mapping ISO là định hướng cho tới khi đối chiếu tiêu chuẩn có bản quyền, phạm vi và SoA được phê duyệt.
