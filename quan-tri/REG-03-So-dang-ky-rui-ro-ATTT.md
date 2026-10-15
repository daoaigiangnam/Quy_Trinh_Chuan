# REG-03 — Sổ đăng ký rủi ro an toàn thông tin

> Dự thảo v0.1. Chấm điểm và ngưỡng chấp nhận phải được phê duyệt trong phương pháp đánh giá rủi ro. Không dùng mẫu này thay cho đánh giá thực tế.

## 1. Thang đánh giá gợi ý
**Khả năng (L):** 1 Hiếm; 2 Ít khả năng; 3 Có thể; 4 Có khả năng cao; 5 Gần như chắc chắn.  
**Tác động (I):** 1 Không đáng kể; 2 Thấp; 3 Trung bình; 4 Cao; 5 Nghiêm trọng.  
**Điểm rủi ro = L × I**. Ma trận và ngưỡng dưới đây chỉ là điểm khởi tạo, cần phê duyệt.

| Điểm | Mức gợi ý | Hướng xử lý gợi ý |
|---:|---|---|
| 1–4 | Thấp | Theo dõi hoặc xử lý trong kế hoạch thông thường |
| 5–9 | Trung bình | Có kế hoạch, owner và hạn |
| 10–16 | Cao | Ưu tiên xử lý; cần phê duyệt cấp quản lý |
| 17–25 | Nghiêm trọng | Hành động khẩn cấp và quyết định cấp lãnh đạo |

## 2. Sổ đăng ký rủi ro
| Risk ID | Phạm vi/tài sản | Kịch bản rủi ro | Mối đe dọa/lỗ hổng | CIA/tác động khách hàng | Kiểm soát hiện có | L | I | Điểm | Mức | Owner | Xử lý | Hạn | Rủi ro tồn dư | Người chấp nhận | Trạng thái |
|---|---|---|---|---|---|---:|---:|---:|---|---|---|---|---|---|---|
| R-001 |  |  |  |  |  |  |  |  |  |  | Tránh/Giảm/Chia sẻ/Chấp nhận |  |  |  | Mở |

## 3. Mô tả bắt buộc cho mỗi rủi ro
1. Tài sản, quy trình, khách hàng hoặc mục tiêu bị ảnh hưởng.
2. Sự kiện có thể xảy ra, nguyên nhân, điểm yếu và hậu quả.
3. Kiểm soát hiện có và bằng chứng chứng minh kiểm soát đang vận hành.
4. Điểm rủi ro trước xử lý, lựa chọn xử lý và kế hoạch hành động.
5. Điểm rủi ro tồn dư sau xử lý, người chịu trách nhiệm và người có thẩm quyền chấp nhận.
6. Ngày đánh giá lại, trigger tái đánh giá và trạng thái.

## 4. Kế hoạch xử lý rủi ro
| Risk ID | Hành động | Kiểm soát/biện pháp | Owner | Nguồn lực | Hạn | Phụ thuộc | Bằng chứng hoàn tất | Kiểm tra hiệu lực | Trạng thái |
|---|---|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |  |  |  |

## 5. Khi phải đánh giá lại
- Thay đổi phạm vi dịch vụ, khách hàng, hạ tầng, kiến trúc, nhà cung cấp hoặc dữ liệu.
- Sự cố ATTT, phát hiện audit, lỗ hổng nghiêm trọng hoặc thay đổi pháp lý/hợp đồng.
- Thay đổi mức độ rủi ro, kiểm soát, mục tiêu RTO/RPO hoặc cách truy cập.
- Đến kỳ rà soát đã được phê duyệt.

## 6. Chấp nhận rủi ro tồn dư
Không chấp nhận chỉ bằng lời nói. Hồ sơ phải nêu lý do, tác động, kiểm soát bù trừ, hạn hiệu lực, trigger đánh giá lại, người chấp nhận đúng thẩm quyền và bằng chứng thông báo khách hàng nếu cần.

## 7. Phê duyệt
| Vai trò | Họ tên | Quyết định/ý kiến | Ngày |
|---|---|---|---|
| Risk Owner |  |  |  |
| ISMS/IT Lead rà soát |  |  |  |
| Người có thẩm quyền chấp nhận |  |  |  |
