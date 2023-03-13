# upptime
Upptime là một dịch vụ giám sát hoạt động và trang web trạng thái miễn phí và mã nguồn mở. Nó rất khác biệt so với các dịch vụ trang trạng thái khác vì nó không yêu cầu một máy chủ - mọi thứ được cung cấp bởi GitHub:

GitHub Actions được sử dụng làm bộ giám sát hoạt động.
GitHub Issues được sử dụng cho các báo cáo sự cố.
GitHub Pages được sử dụng cho trang web trạng thái.
Khái niệm:

Bộ giám sát hoạt động sử dụng GitHub Actions:
Sử dụng GitHub Actions, người dùng có thể lên lịch cho các luồng công việc chạy tự động mỗi x phút. Khoảng thời gian ngắn nhất là 5 phút. Vì vậy, mỗi 5 phút, Upptime sẽ truy cập vào trang web của bạn và đảm bảo rằng nó đang hoạt động.
Chúng tôi cũng ghi lại thời gian phản hồi mỗi ngày và commit nó vào lịch sử git. Như vậy, chúng tôi có thể vẽ biểu đồ các xu hướng dài hạn trong thời gian phản hồi của trang web của bạn bằng cách xem lại lịch sử commit git. Chúng tôi tạo ra các biểu đồ này một lần mỗi ngày, cũng sử dụng lịch trình.

Báo cáo sự cố sử dụng GitHub Issues:
Khi một điểm cuối được chỉ định bị gián đoạn, Upptime sẽ tự động mở một vấn đề mới trong kho lưu trữ GitHub của bạn. Bạn có thể sử dụng vấn đề này để thêm thông tin về sự cố, chẳng hạn như bạn đang điều tra, điều gì đã gây ra sự gián đoạn, vv. Bạn cũng có thể chọn tự động gán một số thành viên từ nhóm của bạn cho vấn đề và gửi thông báo đến các dịch vụ kết nối như Slack và Telegram.
Để thêm thông tin về một sự cố, bạn có thể thêm nhận xét vào vấn đề. Mặc định, vấn đề sẽ bị khóa, vì vậy chỉ các thành viên trong nhóm của bạn được phép bình luận trên nó. Khi trang web của bạn trở lại, vấn đề sẽ tự động đóng lại.

Trang web trạng thái sử dụng GitHub Pages:
Cuối cùng, bạn sẽ nhận được một trang web trạng thái được tạo tĩnh đẹp mắt. Trang web này sẽ hiển thị trạng thái hoạt động của trang web của bạn, lịch sử sự cố và biểu đồ thời gian phản hồi. Trang web luôn cập nhật bằng cách sử dụng API của GitHub để lấy dữ liệu theo thời gian thực và được xây dựng bằng Svelte và Sapper. Bạn có thể tùy chỉnh logo, bản sao và nhiều hơn nữa để làm cho nó trở thành của riêng bạn.
