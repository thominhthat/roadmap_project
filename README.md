# **Roadmap cho dự án laughmanga.com**
## **1. Tổng quan về Front-end và Back-end server**
![The FE_Server_Architecture.!](/img/FE_Server_Architecture.jpg "FE_Server_Architecture - 1 map")
> Khi bạn sở hữu một server farm, một số máy chủ sẽ được chỉ định cho mục đích nhận requests và gửi chúng đến các máy chủ khác. Các máy chủ này được gọi là front-end server.
Các máy chủ thực hiện các quá trình xử lý thực tế được gọi là back-end servers.
Điều này cải thiện khả năng mở rộng của các dịch vụ. Bạn có thể cung cấp nhiều front-end servers truy cập cùng một back-end server hoặc một front-end server với nhiều back-end servers, nơi front-end server hoạt động như một bộ cân bằng tải (load balancer).
> Vậy dự án laughmanga.com của chúng ta với các thành phần front-end và back-end sẽ hoạt động như thế nào? Dự án laughmanga.com vẫn được xây dựng theo hai phần chuyên biệt là front-end và back-end tuy nhiên chúng ta không sử dụng server riêng cho front-end hoặc back-end mà chúng ta sẽ chỉ sử dụng một server cho cả front-end và back-end chạy 2 cổng khác nhau.
> Front-end: https://www.laughmana.com/
> Back-end: https://www.laughmanga.com/api/v1
> Ví dụ về trường hợp sử dụng server riêng cho front-end và back-end (khác IP nên sẽ khác domain):
truyenqqpro.com
> Front-end: http://truyenqqpro.com/
> Back-end: http://truyenvua.xyz/
> Ví dụ về trường hợp chỉ sử dụng một server cho cả front-end và back-end (cùng IP nên sẽ cùng domain):
www.nettruyenme.com
> Front-end: https://www.nettruyenme.com/
> Back-end: https://www.nettruyenme.com/Comic/Services/ComicService.asmx
cuutruyen.net
> Front-end: https://www.cuutruyen.net/
> Back-end: https://kakarot.cuutruyen.net/api/v1/mangas
## **2. Phân chia bố cục và các chức năng chính**
### Trang chủ
> #### Trang chủ chia làm 4 phần: Top, Content 1, Content 2 và Bot
> #### Top gồm 5 chức năng: 
![The top.!](/img/Top_edited.png "Top - 5 functions")
> Chức năng 1: Đăng ký, năng nhập, phân quyền
> Chức năng 2: Hiển thị danh sách user đã theo dõi
> Chức năng 3: Hiển thị thông báo cho user
> Chức năng 4: Tìm kiếm
> Chức năng 5: Hiển thị những truyện nổi bật gần đây trên 1 slide lớn

> #### Content 1
![The content1.!](/img/content1_edited.png "Content1 - 2 functions")
> Chức năng 6: Hiển thị 20 truyện mới cập nhật gần nhất trên slide
> Chức năng 7: Hiển thị toàn bộ truyện theo thời gian truyện được cập nhật

> #### Content 2
![The content2.!](/img/content1_edited.png "Content2 - 1 function")
> Chức năng 8: Hiển thị 20 truyện nổi bật trong tuần, tháng, mọi lúc trên slide

> #### Bot
![The bot.!](/img/bot_edited.png "bot - 1 function")
> Chức năng 9: Hiển thị những nhóm dịch truyện có đóng góp hàng đầu

### Trang thông tin truyện 
![The detail1.!](/img/detail1_edited.png "detail1 - 1 function")
> Chức năng 10: Hiển thị toàn bộ thông tin liên quan đến truyện

### Trang đọc truyện (chap cụ thể)
![The detail2_top.!](/img/detail2_top_edited.png "detail2_top - 4 function")
![The detail2_bot.!](/img/detail2_bot_edited.png "detail2_bot - 1 function")
> Chức năng: 11: Hiển thị tên chap và nút chuyển chap
> Chức năng 12: Bình luận
> Chức năng 13: Hiển thị thanh cuộn đánh dấu vị trí đọc
> Chức năng 14: Chuyển chap tiến lùi và lên đầu trang

## **3. Roadmap chi tiết**
![The roadmap.drawio.!](/img/roadmap.drawio.png "roadmap.drawio - 1 map")
