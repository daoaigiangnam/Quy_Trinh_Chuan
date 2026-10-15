# QT-ATTT-02 — QUẢN LÝ MẬT KHẨU VÀ BÍ MẬT KỸ THUẬT

> **Trạng thái:** Dự thảo nâng cấp v0.2; cần rà soát, chạy thử và phê duyệt trước khi áp dụng.  
> **Chủ sở hữu:** Đầu mối ATTT / IT Lead theo phân công.  
> **Liên quan:** QT-IT-08, QT-IT-11, QT-IT-13, QT-ATTT-04, QT-ISMS-03/04, REG-01, MA-01, MA-02.

## 1. Kiểm soát tài liệu
| Trường | Nội dung |
|---|---|
| Mã | QT-ATTT-02 |
| Phiên bản | 0.2 — dự thảo nâng cấp |
| Chủ sở hữu | Đầu mối ATTT / IT Lead |
| Người rà soát | Chủ hệ thống và các bên liên quan |
| Người phê duyệt | Người có thẩm quyền theo quản trị tài liệu |
| Ngày hiệu lực | Điền sau khi phê duyệt |
| Rà soát | Tối thiểu hằng năm và sau sự cố/thay đổi trọng yếu |

## 2. Mục đích và phạm vi
Quản lý mật khẩu, token, API key, certificate private key, recovery code và secret của dịch vụ trong toàn bộ vòng đời.
Áp dụng cho hệ thống, dữ liệu và hoạt động thuộc Mstar hoặc thuộc khách hàng mà Mstar được ủy quyền. Phụ lục khách hàng xác định phạm vi, công cụ, người phê duyệt, SLA, nơi lưu và thời hạn lưu. Không thực hiện kiểm tra/truy xuất dữ liệu ngoài phạm vi được duyệt.

## 3. Nguyên tắc bắt buộc
1. Chỉ thực hiện trong phạm vi quyền và mục đích được ủy quyền.
2. Áp dụng quyền tối thiểu, phân tách nhiệm vụ và lưu lịch sử thao tác.
3. Không lưu secret dạng rõ hoặc đưa dữ liệu nhạy cảm vào repository/tài liệu dùng chung.
4. Khi nghi ngờ sự cố ATTT, kích hoạt QT-ATTT-04; bảo toàn bằng chứng trước hành động có thể làm mất dấu vết.
5. Ngoại lệ phải có đánh giá rủi ro, biện pháp bù trừ, owner, thời hạn và người phê duyệt.
6. Không tự đặt thời hạn xử lý/retention chung khi chưa có chính sách, hợp đồng hoặc ma trận đã duyệt.

## 4. Vai trò
| Vai trò | Trách nhiệm |
|---|---|
| Người yêu cầu/tiếp nhận | Ghi nhận yêu cầu, xác minh phạm vi và thông tin đầu vào. |
| Người thực hiện | Thực hiện theo hướng dẫn, ghi nhật ký và báo sai lệch. |
| Owner hệ thống/dữ liệu | Xác nhận phạm vi, rủi ro, quyền và tiêu chí đạt. |
| Đầu mối ATTT | Đánh giá rủi ro, điều phối ứng phó và kiểm tra bằng chứng. |
| IT Lead | Phê duyệt trong thẩm quyền, điều phối nguồn lực và chuyển cấp. |
| Đầu mối khách hàng/Legal | Xác nhận nghĩa vụ hợp đồng/pháp lý và phê duyệt khi cần. |

## 5. Đầu vào và điều kiện bắt đầu
Hồ sơ phải xác định đối tượng, mục đích, phạm vi, người yêu cầu, owner, quyền cần dùng, người phê duyệt, công cụ, tiêu chí hoàn thành và nơi lưu bằng chứng. Nếu thiếu thông tin trọng yếu, chuyển Chờ xác nhận; không thực hiện hành động có thể ảnh hưởng dữ liệu/hệ thống khi chưa rõ thẩm quyền.

## 6. Trình tự thực hiện chi tiết

### Bước 1 — Xác định secret và owner
**Người thực hiện:** Người được phân công; owner hệ thống/ATTT rà soát theo mức độ.

Lập danh mục loại secret, hệ thống sử dụng, owner, mục đích, quyền truy cập, nơi lưu, cách xoay vòng và thời hạn. Ưu tiên secret có quyền quản trị, truy cập dữ liệu khách hàng, cloud/API, backup và tài khoản dịch vụ. Không ghi giá trị secret vào danh mục; chỉ lưu định danh hoặc tham chiếu tới kho bí mật.

**Điều kiện đạt:** Kết quả được xác minh và hồ sơ truy nguyên được. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi sai lệch, owner khắc phục và hạn xử lý.

### Bước 2 — Lựa chọn nơi lưu
**Người thực hiện:** Người được phân công; owner hệ thống/ATTT rà soát theo mức độ.

Chỉ lưu secret trong password manager/vault/secret store được phê duyệt có kiểm soát truy cập, mã hóa, audit log và khả năng thu hồi. Không lưu trong source code, Git, file cấu hình chia sẻ, ticket, email, chat, bảng tính hoặc tài liệu hướng dẫn. Nếu phát hiện secret trong nơi không phù hợp, coi là có khả năng lộ và xử lý theo bước ứng phó.

**Điều kiện đạt:** Kết quả được xác minh và hồ sơ truy nguyên được. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi sai lệch, owner khắc phục và hạn xử lý.

### Bước 3 — Cấp quyền truy cập secret
**Người thực hiện:** Người được phân công; owner hệ thống/ATTT rà soát theo mức độ.

Yêu cầu phải nêu người/nhóm, secret cần dùng, mục đích, thời hạn và người duyệt. Cấp quyền tối thiểu, ưu tiên cấp qua cơ chế tự động/định danh; bật MFA và ghi log khi hỗ trợ. Không gửi secret dạng rõ cho người không cần biết; không chia sẻ tài khoản cá nhân.

**Điều kiện đạt:** Kết quả được xác minh và hồ sơ truy nguyên được. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi sai lệch, owner khắc phục và hạn xử lý.

### Bước 4 — Tạo và cấu hình secret
**Người thực hiện:** Người được phân công; owner hệ thống/ATTT rà soát theo mức độ.

Dùng độ dài/thuật toán/chính sách phù hợp nền tảng và tiêu chuẩn nội bộ được duyệt. Không tái sử dụng secret giữa môi trường hoặc khách hàng. Cấu hình ngày hết hạn, owner, cảnh báo và phương thức thu hồi. Certificate phải theo dõi ngày hết hạn và chuỗi tin cậy.

**Điều kiện đạt:** Kết quả được xác minh và hồ sơ truy nguyên được. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi sai lệch, owner khắc phục và hạn xử lý.

### Bước 5 — Xoay vòng và thu hồi
**Người thực hiện:** Người được phân công; owner hệ thống/ATTT rà soát theo mức độ.

Xoay vòng theo lịch đã duyệt, sau thay đổi owner, nghi ngờ lộ, nhân sự rời đi, vendor chấm dứt hoặc sau sự cố. Thực hiện theo thứ tự để tránh downtime: tạo secret mới, cập nhật dịch vụ, xác minh hoạt động, thu hồi secret cũ, kiểm tra log. Ghi kết quả và hệ thống phụ thuộc.

**Điều kiện đạt:** Kết quả được xác minh và hồ sơ truy nguyên được. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi sai lệch, owner khắc phục và hạn xử lý.

### Bước 6 — Xử lý secret bị lộ
**Người thực hiện:** Người được phân công; owner hệ thống/ATTT rà soát theo mức độ.

Không chỉ xóa nội dung khỏi chat/Git. Ghi nhận nơi lộ, thời gian, phạm vi, loại secret và hệ thống liên quan; hạn chế truy cập; thu hồi/rotate ngay theo mức rủi ro; kiểm tra log sử dụng bất thường; xóa bản sao không cần thiết khi có thể và kích hoạt QT-ATTT-04. Bảo toàn bằng chứng trước khi xóa nếu cần điều tra.

**Điều kiện đạt:** Kết quả được xác minh và hồ sơ truy nguyên được. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi sai lệch, owner khắc phục và hạn xử lý.

### Bước 7 — Rà soát và kiểm tra
**Người thực hiện:** Người được phân công; owner hệ thống/ATTT rà soát theo mức độ.

Định kỳ đối chiếu secret đang hoạt động với owner, quyền, ngày xoay vòng và nơi lưu. Phát hiện secret không owner, quá hạn, quyền rộng hoặc secret nhúng trong mã. Giao hành động khắc phục có owner/hạn; không báo đạt nếu chưa xác minh được việc thu hồi.

**Điều kiện đạt:** Kết quả được xác minh và hồ sơ truy nguyên được. **Nếu không đạt:** Giữ trạng thái chưa hoàn tất, ghi sai lệch, owner khắc phục và hạn xử lý.

## 7. Xử lý ngoại lệ và chuyển cấp
Chuyển cấp khi phát hiện truy cập trái phép, secret bị lộ, dữ liệu có nguy cơ lộ/mất, log bị can thiệp, lỗ hổng có thể đã bị khai thác, không thể kiểm soát quyền, thiếu phê duyệt bắt buộc hoặc có rủi ro ảnh hưởng nhiều hệ thống/khách hàng. Ghi mã hồ sơ, thời điểm, phạm vi, bằng chứng, việc đã làm, tác động, người nhận và quyết định cần thiết.

## 8. Bằng chứng tối thiểu
| Bằng chứng | Nội dung |
|---|---|
| Yêu cầu/phạm vi | Người yêu cầu, đối tượng, mục đích và thẩm quyền |
| Cấu hình/kiểm tra ban đầu | Nguồn, thời điểm, trạng thái và phương pháp |
| Phê duyệt | Người duyệt, thời gian, phạm vi, điều kiện |
| Nhật ký thực hiện | Người làm, thao tác, kết quả, sai lệch |
| Kiểm tra sau xử lý | Tiêu chí, kết quả, bằng chứng và người xác nhận |
| Ngoại lệ/CAPA | Rủi ro, biện pháp bù trừ, owner, hạn, kiểm tra hiệu lực |

Lưu trong kho chính thức, hạn chế quyền theo nguyên tắc cần biết và thời hạn theo danh mục hồ sơ/hợp đồng. Bằng chứng sự cố phải giữ chain of custody khi áp dụng.

## 9. KPI và giám sát
| KPI | Định nghĩa |
|---|---|
| Tỷ lệ hồ sơ đủ | Hồ sơ đạt checklist / hồ sơ được lấy mẫu |
| Tỷ lệ xử lý đúng hạn | Hạng mục hoàn tất đúng hạn / hạng mục đến hạn theo chính sách đã duyệt |
| Hạng mục quá hạn | Số lượng và tuổi tồn, phân theo mức độ |
| Sai lệch lặp lại | Số sai lệch tái diễn cùng nguyên nhân |
| Hành động khắc phục đúng hạn | Hành động hoàn tất đúng hạn / hành động đến hạn |

Phải chốt công thức, nguồn, kỳ đo và ngưỡng trước khi báo cáo. Không loại các trường hợp chưa xử lý khỏi mẫu đo chỉ vì thiếu dữ liệu.

## 10. Lưu đồ
```mermaid
flowchart TD
 A([Yêu cầu/sự kiện phát sinh]) --> B[Ghi nhận và xác định phạm vi]
 B --> C{Đúng thẩm quyền và đủ thông tin?}
 C -- Không --> D[Chờ xác minh / chuyển cấp]
 D --> C
 C -- Có --> E[Đánh giá và thực hiện kiểm soát]
 E --> F[Kiểm tra kết quả]
 F --> G{Đạt tiêu chí?}
 G -- Không --> H[Khắc phục / ứng cứu / ghi ngoại lệ]
 H --> E
 G -- Có --> I[Lưu bằng chứng, đóng hồ sơ]
 I --> J[Rà soát xu hướng và cải tiến]
```

## 11. Điều kiện ban hành
- [ ] Xác định owner, công cụ, người phê duyệt và phạm vi.
- [ ] Chốt thời hạn/retention theo chính sách và hợp đồng.
- [ ] Đối chiếu biểu mẫu và nơi lưu bằng chứng.
- [ ] Chạy thử tình huống bình thường, ngoại lệ và chuyển cấp.
- [ ] Ghi nhận/khắc phục sai lệch, đào tạo người thực hiện.
- [ ] Phê duyệt và công bố phiên bản hiệu lực.

**Lưu ý:** Tài liệu là dự thảo kiểm soát ATTT, không tự chứng minh chứng nhận ISO; phải phù hợp phạm vi ISMS, đánh giá rủi ro, SoA, hợp đồng và pháp luật áp dụng.
