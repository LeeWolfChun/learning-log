# Learning log 01 — Xác định MVP



Ngày viết: 11/10/2026

## 1. Bối cảnh và mục tiêu của tôi

Mình đang học java + SQL, mình lựa chọn project này vì nó có thể giúp mình học được cách thiết kế 1 database thực tế như thế nào, queue, sử lý có 2 client đăng kí cùng lúc, mình muốn học được cách thiết kế hệ thống logic phía sau 1 trang web hay 1 ứng dụng, và xử lý các tình huống dễ phát sinh lỗi

## 2. Những việc tôi đã thực sự làm

Mình có viết node về những dữ liệu cần có cho 3 đối tượng như user, evnet, registration, một yêu cầu bạn đã sửa, một quyết định bạn đã chọn. Phân biệt việc bạn tự làm,tôi và Mentor đã thảo luân là việc nên chọn prọject nào để làm lựa chon đầu tiên, tôi sẽ học gi từ nó và hỗ trợ tôi lưu những dấu vết khi làm prọect như thế nào như cái mà tôi đang viết. file requirement.md là do chatgpt dựa trên note của tôi và hỗ trợ tôi hệ thống lại những MVP tôi đưa ra và những tính năng cơ bản có lỗ hỗng gì hay không. template lod cũng do chatgpt tạo

## 3. Một điểm tôi hiểu rõ hơn

việc khôi phục những đăng ký hủy bởi ban tổ chức và đăgn kí hủy bởi sinh viên. ex: nếu ban tổ chức hủy sự kiện thì tất cả đăng ký có hiệu lực sẽ bị đánh dấu hủy và khi khôi phục những đăng ký trong database của sự kiện thì vấn đề xảy ra là những đăng kí hủy bởi sinh viên cũng sẽ được khôi phục -> số chỗ không đủ -> bug. đấy là lý do cần đặt rõ quy tắc gán nhãn hủy do sinh viên và hủy do ban tổ chức tránh tình trạng được nên ra trong ví dụ.

## 4. Quyết định của tôi và lý do

Q-01: hiển thị và thời điểm mở đăng ký 
- chi tiếtL: thêm vào database event - registrationStart (thời gian mở đăng ký) nó dẫn đến danh sách khi GET event sẽ gồm: sự kiện chưa mở đăng kí. đang mở đăng ký , hết hạn đăng ký sẽ hiển thị "đã đóng đăng ký".
- Lý do: điều này sẽ giúp sinh viên dễ tìm hiểu về các sự kiện sắp diễn ra và camp đăng kí vì nếu chỉ hiển thi sự kiện đẫ mở đăng kí thì lúc sinh viên đăng ký có thể đã hết chỗ.

## 5. Điều còn chưa rõ


## 6. Bước phân tích yêu cầu tiếp theo

 Tiếp theo sẽ là lựa chọn 1 stack để bắt đầu thực hiện , cái tôi đang có dự định chọn là java + spring boot.

## Tự kiểm tra trước khi lưu

- [x] Mỗi việc ghi là đã làm đều có trải nghiệm hoặc dấu vết thực tế của tôi.
- [x] Tôi phân biệt đóng góp của mình với hỗ trợ từ mentor/assistant.
- [x] Tôi phân biệt quyết định đã chọn với đề xuất còn mở.
- [x] Tôi không ghi đã xây dựng, kiểm thử hoặc hoàn thành chức năng chỉ vì đã viết acceptance criteria.
- [x] Nội dung log tập trung vào bước phân tích yêu cầu.
