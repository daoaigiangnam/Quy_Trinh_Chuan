# FR-CUS-01 — Phụ lục chuẩn dịch vụ và an toàn thông tin khách hàng

> **Dự thảo dùng lặp lại cho từng khách hàng.** Đây là phụ lục vận hành, không tự thay thế hợp đồng/NDA/DPA hoặc tư vấn pháp lý. Chỉ kích hoạt sau khi được Mstar và khách hàng có thẩm quyền xác nhận.

## A. Thông tin quản lý
| Trường | Nội dung |
|---|---|
| Mã phụ lục / phiên bản |  |
| Khách hàng / pháp nhân |  |
| Hợp đồng / ngày hiệu lực |  |
| Service Owner Mstar |  |
| Customer Owner / người duyệt |  |
| Ngày bắt đầu / review tiếp theo |  |
| Trạng thái | Nháp / Rà soát / Đã duyệt / Hết hiệu lực |

## B. Phạm vi dịch vụ
| Dịch vụ/hạng mục | Trong phạm vi | Ngoài phạm vi | Giờ hỗ trợ | Site/tenant | Owner |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

## C. SLA và quy tắc ticket
| Mức độ | Tiêu chí tác động/khẩn cấp | Thời gian phản hồi | Mục tiêu khắc phục/khôi phục | Chu kỳ cập nhật | Giờ hỗ trợ/loại trừ |
|---|---|---|---|---|---|
| P1 |  |  |  |  |  |
| P2 |  |  |  |  |  |
| P3 |  |  |  |  |  |
| P4 |  |  |  |  |  |

Định nghĩa điểm bắt đầu/dừng SLA, ngày nghỉ, chờ khách hàng/vendor, thay đổi phạm vi và phương pháp tính phải ghi rõ; không suy diễn từ mẫu chuẩn.

## D. Danh mục hệ thống/tài sản
| System/Asset ID | Tên | Owner khách hàng | Criticality | Vị trí/tenant | Phụ thuộc | Monitoring/backup | Hồ sơ nguồn |
|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |  |

## E. Ma trận quyền theo khách hàng
| Nhân sự/role Mstar | Hệ thống | Quyền cần thiết | Mục đích/ticket | Phê duyệt khách hàng | MFA/kênh | Ngày hết hạn | Cách thu hồi |
|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |  |

Không điền mật khẩu/token/secret vào phụ lục. Chỉ tham chiếu kho bí mật được phê duyệt.

## F. Dữ liệu, bảo mật và quyền riêng tư
| Chủ đề | Quyết định được duyệt |
|---|---|
| Phân loại dữ liệu khách hàng |  |
| Dữ liệu cá nhân/nhạy cảm có xử lý? |  |
| Vị trí lưu/xử lý và khu vực địa lý |  |
| Mục đích, phạm vi và quyền truy cập |  |
| Mã hóa khi truyền/lưu |  |
| Chia sẻ với bên thứ ba/subprocessor |  |
| Retention, legal hold, trả/xóa dữ liệu |  |
| Nghĩa vụ thông báo và đầu mối pháp lý |  |
| Hạn chế chụp màn hình/export/log |  |

## G. Sự cố và thông báo
| Mức độ | Đầu mối Mstar | Đầu mối khách hàng | Kênh khẩn cấp | Thời hạn thông báo theo hợp đồng | Nội dung cập nhật |
|---|---|---|---|---|---|
| Sự cố dịch vụ |  |  |  |  |  |
| Nghi ngờ sự cố ATTT |  |  |  |  |  |
| Rò rỉ/mất dữ liệu |  |  |  |  |  |

Thời hạn thông báo phải lấy từ hợp đồng và yêu cầu pháp lý đã được xác minh; không tự đặt một SLA chung cho mọi khách hàng.

## H. Backup, khôi phục và liên tục kinh doanh
| Hệ thống | Owner | RPO mục tiêu | RTO mục tiêu | Lịch backup | Retention | Vị trí bản sao | Chu kỳ restore test | Người xác nhận |
|---|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |  |  |

## I. Nhà cung cấp và phụ thuộc
| Vendor/service | Dữ liệu/quyền truy cập | Criticality | Hợp đồng/điều khoản ATTT | Đầu mối | Kế hoạch exit |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

## J. Ngoại lệ, rủi ro và giả định
| ID | Mô tả | Tác động | Biện pháp bù trừ | Owner | Hạn | Người chấp nhận | Ngày rà soát |
|---|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |  |

## K. Bàn giao/exit
- [ ] Ticket, cấu hình, inventory, runbook và rủi ro tồn được bàn giao.
- [ ] Quyền Mstar/vendor được rà soát và thu hồi.
- [ ] Dữ liệu trả/xóa/giữ có quyết định và bằng chứng.
- [ ] License, domain, SSL, hợp đồng và tài sản được đối soát.
- [ ] Khách hàng xác nhận hoàn tất hoặc chấp nhận danh sách tồn.

## L. Phê duyệt
| Bên | Họ tên/chức danh | Quyết định | Ngày |
|---|---|---|---|
| Mstar Service Owner |  |  |  |
| Mstar IT Lead/ISMS theo phạm vi |  |  |  |
| Khách hàng Owner |  |  |  |
| Người có thẩm quyền hợp đồng |  |  |  |
