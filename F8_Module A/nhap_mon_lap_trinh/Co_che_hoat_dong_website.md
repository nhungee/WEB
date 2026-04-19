## 1. Mô hình client-server
### A. Giới thiệu:
- Mô hình client - server là mô hình giúp máy tính giao tiếp truyền tải dữ liệu cho nhau
- Client và server về bản chất thì nó là hai máy tính giao tiếp và truyền tải hai dữ liệu cho nhau:
    - Máy tính đóng vai trò là máy khách - client : với vai trò máy khách chúng sẽ không cung cấp tài nguyên đến các máy tính khác mà chỉ sử dụng tài nguyên được cung cấp từ máy chủ. Một client trong mô hình này có thể là một server cho mô hình khác, tùy thuộc nhu cầu người sử dụng.
    - Máy tính đóng vai trò là máy chủ - server : là máy tính có khả năng cung cấp tài nguyên và các dịch vụ đến máy tính khác trong hệ thống mạng. server đóng vai trò hỗ trợ cho hoạt động của máy tính khách_ client diễn ra hiệu quả hơn.
### B. Mô Hình Client- server là gì?
- Mô hình client server là mô hình mạng máy tính trong đó có máy tính con được đóng vài trò là một máy khách, chúng làm nhiệm vụ gửi yêu cầu đến với máy chủ. Để máy chủ xử lý yêu cầu và trả kêt quả cho máy khách. 
### C. Nguyên tắc hoạt động
- Để máy khách và máy chủ có thể giao tiếp được với nhau thì giữa chúng phải có một chuẩn nhất định, và chuẩn đó được gọi là giao thức. Một số giao thức được sử dụng phổ biến hiện nay như: HTTPS, TCP/IP, FTP,...
- Nếu máy khách muốn lấy được thông tin từ máy chủ, chúng phải tuân theo một giao thức mà máy chủ đó đưa ra. Nếu yêu cầu đó được chấp nhận thì máy chủ sẽ thu thập thông tin và trả về kết quả cho máy khách yêu cầu. Bởi vì Server - máy chủ luôn luôn trong trạng thái sẵn sàng để nhận request từ client nên chỉ cần client gửi yêu cầu tín hiệu và chấp nhận yêu cầu đó thì server sẽ trả kết quả về phía client trong thời gian ngắn nhất.
### D. Ưu điểm của mô hình
- có thể làm việc trên bất kì một máy tính nào có hỗ trợ giao thức truyền thông.
- Có thể có nhiều server cùng làm một dịch vụ
- Chỉ mang đặc điểm của phần mềm mà không hề liên quan đến phần cứng
- Hỗ trợ người dùng nhiều dịch vụ đa dạng và sự tiện dụng bởi khả năng truy cập từ xa.
- Cung cấp một nền tảng lý tưởng, cho phép cung cấp tích hợp các kỹ thuật hiện đại như mô hình thiết kế hướng đối tượng, hệ chuyên gia, hệ thông tin địa lý (GIS).
### E. Nhược điểm
- Vấn đề bảo mật dữ liệu thông tin đôi khi còn chưa được an toàn lắm. Vì do phải trao đổi dữ liệu giữa 2 máy tính khác nhau ở 2 khu vực địa lý cách xa nhau. Và đây cũng nhược điểm duy nhất của mô hình này.
- Tuy nhiên vấn đề này thì có một số giao thức đã hỗ trợ bảo mật dữ liệu khi truyền tải. Giao thức được sử dụng phổ biến như HTTPS.
## 2. Request: 
### A. Request là gì? 
- Request(yêu cầu): là một thông điệp yêu cầu từ một chương trình máy tính(client) tới một chương trình máy tính khác(server) để yêu cầu một hành động hoặc một tài nguyên cụ thể nào đó. Nó là một phần cốt lỗi của giao tiếp giữa các hệ thống trogn môt trường mạng, đặc biệt trên Web.
- VD: Như việc bạn gọi tới tổng đài dịch vụ để yêu cầu thoogn tin hoặc thực hiện giao dịch. Cuộc gọi của bạn chính là HTTP Request mang thông tin bạn muốn yêu cầu và server sẽ phản hồi lại yêu cầu đó.
- Theo định nghĩa của các nhà phát triển, HTTP Request là tập các phương thức được định nghĩa để có thể thực hiện một số hành động dựa trên các tài nguyên gửi lên cho web server. Mọi tương tác của người dùng trên web dều bắt nguồn từ chuỗi request. 
- Về bản chất, request giống như việc gửi một lá thư kỹ thuật số đến địa chỉ cụ thể(URL trên server) với yêu cầu rõ ràng(method). Lá thưu này có tiêu đề kèm theo thông tin bổ sung(headers) và đoi khi có cả nội dung dữ liệu cần gửi(Body).
### B. HTTP Request hoạt động như thế nào?
-  HTTP request giống như khi trình duyệt của bạn kết nối với máy chủ để yêu cầu truy cập một tài nguyên cụ thể hoặc gửi dữ liệu đến đó. Có nhiều loại phương thức yêu cầu (request method) trong HTTP, và mỗi loại sẽ tạo ra một kiểu phản hồi khác nhau từ máy chủ. Những phương thức phổ biến nhất bao gồm:
  - GET: Đây là phương thức HTTP đucợ sử dụng phổ biến nhát. Một yêu cầu GET sẽ yêu cầu máy chủ cung cấp thoogn tin hacowj tài nguyên cụ thể. Khi mà bạn truy cập trang Web thì trình duyệt của bạn sẽ gửi lên hệ thông nhiều yêu cầu GET để nhận được các dữ liệu cần thiết để tải trang.
  - HEAD: Với yêu cầu HEAD bạn chỉ nhận được phần thông tin tiêu đề(header) của trang mà bạn muốn tải. loại yêu cầu này thường dung kiểm tra kích thước của tài liệu trước khi tải về bằng phương thức GET.
  - POST: Trình duyệt sử dụng phương thức POST khi cần gửi dữ liệu lên máy chủ. VD: Khi bạn điền một biểu mẫu lên trang web và bạn nhấn gửi là bạn đang thực hiện một lệnh post để máy chủ nhận được dữ liệu đó.
  - PUT: Phương thức PUT tương tự POST nhưng thay vì gửi dữ liệu mới thì PUT được dùng để cập nhật thông tin có sẵn trên máy chủ đích.
- Ngoài ra còn một số phương thức HTTP khác như DELETE, PATCH , OPTIONS, tuy nhiên chúng ít được sử dụng trong các tình huống thông thường.
- Khi bạn gặp lỗi HTTP thường là vì máy chủ khoogn thể thực hiện yêu cầu của bạn. Mã lỗi HTTP mà bạn nahanj đucợ sẽ giải thích nguyên nhân. Một số nguyên nhân phổ biến gây ra lỗi HTTP là khoogn thể kết nối với máy chủ hoặc không tìm thấy tài nguyên được yêu cầu.
### C. Tầm quan trọng của việc hiểu HTTP Request
- Giúp gỡ rối : giúp xác định vấn đề nằm ở đâu 
- Tối ưu hiệu suất: Hiểu các request hoạt động giúp tối ưu header, body , method ...
- Bảo mật: Hiểu các yêu càu được truyền đi giúp bảo mật thông tin nhạy cảm
- Tương tác với API: Hầu hết các API đều sử dụng Request làm phương thức giao tiếp.
### D. Thành phần chính của một HTTP Request: một HTTP Request tiêu chuẩn giống như một bức thư gửi đến máy chủ
 #### 1. Request Line (Dòng yêu cầu): dòng đầu tiên trong một HTTP Request.
 - method(phương thức): hành động muốn thực hiện
 - path(đường dẫn): Dùng để xác định tài nguyên mà client yêu cầu: địa chỉ cụ thể của tài nguyên. Đường dẫn này bắt buộc phải bắt đầu bằng dấu “/”.(VD: /trang-chu hoặc /img/logo.png).
 - HTTP Version: Phiên bản giao thức(Thường là HTTP/1.1 hoặc HTTP/2).
#### 2. Request Headers (Tiêu đề yêu cầu): 
 - Thành phần thứ hai trong HTTP Request chính là headers. Header chứa các thông tin bổ sung được gửi kèm theo yêu cầu giữa client và server. Nó giúp Server hiểu rõ hơn về ngữ cảnh của Client:
     - Host: Địa chỉ của server (ví dụ: google.com).
     - User-Agent: Thông tin về trình duyệt và hệ điều hành của em (ví dụ: Chrome trên Windows).
     - Accept: Loại định dạng mà trình duyệt có thể đọc được (như text/html, application/json).
     - Cookie: Các thông tin định danh để Server nhận ra em là ai (đã đăng nhập chưa).
 - Tương tự các phần khác của HTTP Request, header phân biệt chữ hoa và chữ thường, được viết theo định dạng: tên header, theo sau là dấu “:” và một giá trị cụ thể.
#### 3. Message Body
Phải thể hiện được cấu trúc cơ bản của một 
http request.
## 3. Response 

