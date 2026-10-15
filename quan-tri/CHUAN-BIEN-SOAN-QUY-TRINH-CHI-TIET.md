# CHUẨN BIÊN SOẠN VÀ RÀ SOÁT QUY TRÌNH VẬN HÀNH MSTAR

> **Trạng thái:** Chuẩn biên soạn dự thảo v0.1. Dùng làm tiêu chí nâng cấp toàn bộ quy trình; chưa thay thế phê duyệt tài liệu chính thức.

## 1. Mục tiêu

Đảm bảo mọi quy trình không chỉ mô tả mục tiêu mà còn hướng dẫn nhân viên thực hiện nhất quán, xác định được thẩm quyền, tiêu chí đạt/không đạt, bằng chứng, chuyển cấp và điều kiện đóng hồ sơ. Tài liệu phải dễ hiểu với nhân viên mới nhưng vẫn đủ kiểm soát cho vận hành dịch vụ và đánh giá nội bộ.

## 2. Cấu trúc tối thiểu bắt buộc của một quy trình

1. **Kiểm soát tài liệu:** mã, tên, phiên bản, chủ sở hữu, người soạn/rà soát/duyệt, ngày hiệu lực, lịch sử sửa đổi, chu kỳ rà soát.
2. **Mục đích và kết quả mong đợi:** vấn đề cần kiểm soát, đầu ra cụ thể.
3. **Phạm vi:** đối tượng, dịch vụ, hệ thống, địa điểm; nội dung loại trừ; ranh giới trách nhiệm Mstar/khách hàng/nhà cung cấp.
4. **Thuật ngữ và viết tắt:** định nghĩa ngắn gọn các từ có thể gây hiểu nhầm.
5. **Nguyên tắc và điều cấm:** các kiểm soát không được bỏ qua; cách xử lý khi không đáp ứng.
6. **Vai trò và thẩm quyền:** người thực hiện, kiểm tra, phê duyệt, tư vấn, được thông báo; quy định tách biệt nhiệm vụ và kiểm soát bù trừ.
7. **Đầu vào và điều kiện bắt đầu:** thông tin, quyền, hợp đồng, phê duyệt, công cụ, tài sản và năng lực cần có.
8. **Quy trình từng bước:** mỗi bước nêu rõ các mục tại phần 3 dưới đây.
9. **Lưu đồ:** phản ánh các quyết định thật, nhánh không đạt, nhánh thiếu thông tin/quyền, nhánh chuyển cấp và vòng lặp làm lại.
10. **Ngoại lệ và tình huống bất thường:** tiêu chí dừng, người cần báo, biện pháp giảm thiểu, thẩm quyền phê duyệt, thời hạn ngoại lệ.
11. **Bằng chứng và hồ sơ:** mẫu cần dùng, trường bắt buộc, người lập/kiểm tra, nơi lưu, phân quyền, thời hạn lưu và liên kết hồ sơ liên quan.
12. **KPI và giám sát:** định nghĩa, công thức, nguồn dữ liệu, chu kỳ, owner, ngưỡng cảnh báo được phê duyệt.
13. **Đào tạo và kiểm tra hiệu lực:** đối tượng cần đào tạo, cách kiểm tra, lấy mẫu hồ sơ, xử lý sai lệch.
14. **Phụ lục theo khách hàng:** phạm vi, SLA, đầu mối, quyền, dữ liệu, thông báo, RTO/RPO, retention, nhà cung cấp và yêu cầu hợp đồng.
15. **Điều kiện ban hành:** kiểm tra tính đầy đủ, chạy thử, sửa lỗi, rà soát, phê duyệt và công bố phiên bản hiệu lực.

## 3. Cấu trúc bắt buộc cho từng bước

Mỗi bước trong bảng tác nghiệp cần có:

| Trường | Câu hỏi phải trả lời |
|---|---|
| Mã bước/tên bước | Đang ở giai đoạn nào? |
| Người chịu trách nhiệm | Ai trực tiếp thực hiện? Ai hỗ trợ? Ai kiểm tra/phê duyệt? |
| Điều kiện vào | Cần có gì trước khi bắt đầu? |
| Thao tác | Làm theo thứ tự nào? Dùng hệ thống/công cụ/runbook nào? |
| Tiêu chí quyết định | Dựa trên thông tin nào để chọn nhánh? |
| Tiêu chí hoàn thành | Bằng chứng nào chứng minh bước đã đạt? |
| Khi không đạt | Dừng, bổ sung, làm lại, rollback hay chuyển cấp? Ai quyết định? |
| SLA/thời hạn | Thời hạn lấy từ hợp đồng/ma trận đã duyệt nào? Không tự bịa thời hạn. |
| Hồ sơ/bằng chứng | Ghi vào biểu mẫu/ticket/log nào? Ai lưu ở đâu? |
| Rủi ro và kiểm soát | Điều gì có thể sai và biện pháp phòng ngừa/phát hiện là gì? |

Không chấp nhận các chỉ dẫn chung như “xử lý phù hợp”, “kiểm tra đầy đủ”, “lưu bằng chứng tương ứng” nếu không có tiêu chí hoặc ví dụ cụ thể.

## 4. Quy tắc viết dễ hiểu

- Dùng câu ngắn, động từ hành động: kiểm tra, đối chiếu, ghi nhận, xác minh, phê duyệt, thực hiện, kiểm thử, chuyển cấp, đóng.
- Một bước chỉ nên có một mục tiêu chính; nếu có nhiều quyết định thì tách bước hoặc dùng nhánh.
- Lần đầu xuất hiện thuật ngữ phải giải thích; có thể thêm ví dụ nhưng phải ghi rõ là ví dụ.
- Nêu điều kiện và kết quả cụ thể, tránh câu mơ hồ như “nếu cần”, “khi phù hợp” mà không chỉ rõ ai quyết định dựa trên tiêu chí nào.
- Với nội dung phụ thuộc khách hàng/hợp đồng, ghi rõ “theo phụ lục khách hàng đã phê duyệt” và chỉ ra trường dữ liệu nào phải cấu hình.
- Không đặt SLA, thời hạn lưu hồ sơ, ngưỡng KPI hoặc nghĩa vụ pháp lý chung nếu chưa được xác minh.
- Không ghi thông tin bí mật, mật khẩu, token, khóa riêng hoặc dữ liệu khách hàng thực vào tài liệu mẫu/repository.
- Không tuyên bố chứng nhận ISO chỉ vì quy trình có mapping tiêu chuẩn.

## 5. Tiêu chuẩn tối thiểu của biểu mẫu

Mỗi biểu mẫu phải có:
- Mã và tên; quy trình liên quan; phiên bản/trạng thái.
- Mục đích và điều kiện sử dụng; hướng dẫn điền.
- Mã hồ sơ duy nhất, ngày giờ, khách hàng/hệ thống (nếu áp dụng), người lập/owner.
- Trường nghiệp vụ riêng của biểu mẫu; không chỉ lặp một bộ trường chung cho mọi biểu mẫu.
- Nhật ký hành động/kết quả/bằng chứng khi phù hợp.
- Người kiểm tra, người phê duyệt và điều kiện phê duyệt khi áp dụng.
- Checklist hoàn tất; trạng thái; nơi lưu; phân loại thông tin; thời hạn lưu theo danh mục đã duyệt.
- Trường liên kết ticket/change/incident/asset/vendor để truy nguyên.
- Ghi “N/A” kèm lý do khi trường không áp dụng; không để trống trường trọng yếu mà không giải thích.

Biểu mẫu có thể dùng chung một số trường hành chính, nhưng phần nghiệp vụ phải khác nhau theo mục đích. Không coi việc tạo nhiều mẫu có cùng trường chung là đủ để chứng minh quy trình đã được vận hành hóa.

## 6. Tiêu chí lưu đồ

- Có điểm bắt đầu và kết thúc rõ.
- Mỗi hình thoi là câu hỏi có câu trả lời xác định, ví dụ “Đã có phê duyệt hợp lệ?”.
- Có nhánh Không/Chưa đạt và chỉ rõ bước tiếp theo.
- Thể hiện điểm dừng an toàn, chuyển cấp, rollback, ngoại lệ hoặc kích hoạt quy trình liên quan.
- Các bước trên lưu đồ khớp với số bước và thuật ngữ trong nội dung.
- Không vẽ đường vòng lặp vô hạn; chỉ rõ điều kiện thoát hoặc thời điểm chuyển cấp.

## 7. Quy tắc quản lý ba lớp tài liệu

1. **Chuẩn Mstar:** cách làm chung, vai trò chuẩn, kiểm soát tối thiểu, quy trình và mẫu nền.
2. **Phụ lục khách hàng:** phạm vi hợp đồng, hệ thống, SLA, đầu mối, quyền, dữ liệu, thông báo, nhà cung cấp, RTO/RPO, retention và các khác biệt được phê duyệt.
3. **Bằng chứng vận hành:** ticket, log, phê duyệt, kết quả kiểm thử, biên bản, báo cáo và hồ sơ CAPA thực tế.

Không đưa dữ liệu thực hoặc bí mật khách hàng vào tài liệu chuẩn. Không thay đổi chuẩn chung chỉ để hợp thức hóa một trường hợp ngoại lệ; ngoại lệ phải được đánh giá, phê duyệt và có thời hạn.

## 8. Checklist rà soát trước khi trình ký

- [ ] Người đọc mới có thể hiểu thuật ngữ, vai trò và các bước mà không cần giải thích miệng.
- [ ] Phạm vi/điều kiện bắt đầu và trường hợp loại trừ rõ ràng.
- [ ] Mỗi bước có người chịu trách nhiệm, thao tác, tiêu chí đạt, nhánh không đạt và bằng chứng.
- [ ] Quyền, phê duyệt, tách biệt nhiệm vụ và kiểm soát bù trừ được xác định.
- [ ] SLA/thời hạn lấy từ nguồn được phê duyệt; không tự giả định.
- [ ] Lưu đồ khớp nội dung và có nhánh ngoại lệ/chuyển cấp.
- [ ] Link biểu mẫu đúng, mở được và biểu mẫu có trường nghiệp vụ phù hợp.
- [ ] Bằng chứng, nơi lưu, quyền truy cập và thời hạn lưu được xác định.
- [ ] KPI có định nghĩa, công thức, nguồn, chu kỳ và owner.
- [ ] Có kịch bản chạy thử và bằng chứng kết quả chạy thử.
- [ ] Sai lệch chạy thử có hành động khắc phục và được kiểm tra lại.
- [ ] Có rà soát ATTT, hợp đồng/pháp lý và chủ hệ thống khi nội dung liên quan.
- [ ] Người có thẩm quyền phê duyệt; phiên bản hiệu lực được công bố và phiên bản cũ được kiểm soát.

## 9. Lưu ý ISO và ban hành

Chuẩn này hỗ trợ cách biên soạn và kiểm soát tài liệu; nó không thay thế ISO/IEC 27001, ISO/IEC 27002, đánh giá rủi ro, SoA, yêu cầu pháp lý hoặc hợp đồng. Việc gán điều khoản/kiểm soát ISO phải được rà soát theo phạm vi ISMS và bản tiêu chuẩn áp dụng. Mọi quy trình đang trong trạng thái dự thảo chỉ được dùng cho rà soát/chạy thử có kiểm soát cho đến khi được phê duyệt.
