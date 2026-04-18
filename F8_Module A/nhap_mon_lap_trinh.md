
# Tổng quan về lập trình Web
## 1. Các vị trí công việc trong ngành
---
- **Frontend**: Làm về giao diện người dùng.
    ### Giai đoạn 1: 
    #### 1. HTML
    - thẻ cơ bản: div, p , a, img, form
    - semantic: header, footer, section
    - form + input
      
    #### 2. CSS
    - box model
    - flexbox 
    - grid
    - responvive(media query)
    #### 3. JavaScript(core)
    - Biến, hàm, vòng lặp
    - Array, Object
    - DOM
    - event(click, submit)
    - fetch API(gọi backend)
    ### Giai đoạn 2: lib
    #### 1. UI/CSS lib
    - Bootstrap(dễ dùng)
    - Tailwind(phổ biến hơn hiện tại)
    #### 2. JS lib
    - jQuery(ít dùng nhưng nên biết)
    ### Giai đoạn 3: Framework
    - react 
    - component 
    - props, state
    - hook (useState, useEffect)
    - routing
    - redux/ Zustand(quản lý State)
    - axio(gọi API)
    ### Giai đoạn 4: Nâng cao
    - TypeScript
    - Next.js(framework của react)
    - SEO, performance
    
---
- **Backend**: Làm về dữ liệu và máy chủ.
  ### Giai đoạn 1: Nền tảng
  #### 1. Ngôn ngữ (chọn 1): học luôn JS để sync với frontend
    - JavaScript -> phổ biến(NOde.js)
    - hoặc: python, java, C#
  #### 2. Kiến thức cần có
    - HTTP/ HTTPS
    - Request/ Response
    - RERT API
    - JSON
  
  ### Giai đoạn 2: Thuần Backend
  #### Node.js
    - Node.js
    - Tạo server bằng http
  
  ### Giai đoạn 3: Framework
  #### Express.js (cơ bản nhất)
    - Express.js
    - Routing
    - Middleware
    - API
  ### Giai đoạn 4: Database
  #### SQL
    - MySQL / PostgreSQL
  #### NoSQL
    - MongoDB

  #### Học:
    - CRUD
    - Query
    - Schema
  ### Giai đoạn 5: Nâng cao Backend
    - Authentication (JWT)
    - MVC pattern
    - API bảo mật
    - Upload file
    - Deploy (Vercel, Render, VPS)
___
## 2. Xu hướng phát triển của lập trình web
### 1. AI-First Development (Kỷ nguyên AI dẫn dắt) : AI không còn là "công cụ hỗ trợ" mà trở thành hạt nhân của quy trình phát triển
- Hỗ trợ lập trình: Copilot hay mô hình AI viết code và giúp tối ưu , kiểm thử
- Edge AI: thay vì gửi yêu cầu về server, các mô hình học máy như tensorFlow.js chạy trực tiếp trên trình duyệt, cho phép, nhận diện hình ảnh, giọng nói và xử lý ngôn ngữ thực tế tại máy khách.
- Cá nhân hóa: AI phân tích hành vi người dùng để tự động thay đổi giao diện và lộ trình trải nghiệm
### 2. Sự thống trị của Meta-frameworks & TypeScript : việc viết JavaScript thuần cho các dự án chuyên nghiệp là lạc hậu
- Meta-frameworks là tiêu chuẩn : next.js(react), Nuxt(Vue) hay svelteKit trở thành lựa chọn mặc định vì chúng giải quyết tốt các bài toán về Routing, caching, và rendering(SSR/SSG).
- Hệ sinh thái TypeScript toàn diện: End-to-end type safety (an toàn dữ liệu từ frontend tới backend) là yêu cầu bắt buộc để giảm thiểu lỗi trong các hệ thống lớn.
- React Compiler: Việc tối ưu hiệu nắng(memoization) giờ đây được thực hiện tự động bởi trình biên dịch, giúp lập trình viên tập trung vào logic thay vì kĩ thuật tối ưu thủ công.
### 3. Edge Computing & Serverless (Xử lý tại "rìa"): xu hướng chuyển từ server trung tâm sang các node ở gần người dùng nhát đang bùng nổ.
- Độ trễ gần như bằng 0
- Backendless apps 
### 4. WebAssembly(Wasm) phá vở giới hạn hiệu năng: Wasm đang mang những ứng dụng vốn chỉ có trên destop lên trình duyệt
- Ứng dụng nặng: các trình chỉnh sửa video, phần mềm thiết kế 3D(như Figma, AutoCAD) và game cấu hình cao chạy mượt ngay trên web. 
- Đa ngôn ngữ: Cho phép chạy code C++, Rust, Go trên trình duyệt với tốc độ tương đương ứng dụng bản địa(native app).
### 5. Web 3.0 & bảo mật phi tập trung: 
- Identiny: Đăng nhặp không cần mật khẩu thông qua ví điện tử hoặc định dnah phi tập trung. 
- Data Ownership: Người dùng có quyền kiểm soát dữ liệu cá nhân chặt ché hơn thoogn qua các giao thức blockchain tích hợp sâu vào trình duyệt.
#### **Ngôn ngữ phổ biến:**
- **TypeScript:** Nó giải quyết vấn đề lớn nhất của JavaScript là "loạn kiểu dữ liệu". Với các dự án lớn, TypeScript giúp phát hiện lỗi ngay khi đnag viết code(compile-time), giúp bảo trì hệ thống dễ dàng.
- **Python(Backend & AI):** Python là ngôn ngữ backend phát trienr nhanh nhất nhờ làn sóng AI. Sử dụng các Framework như FastAPI hay Django để xây dựng các API xử lý dữ liệu và tích hợp mô hình ngôn ngữ lớn(LLM).
- **JavaScript:** tập trung vào các Framework như React, Vue, Svelte.
- **Rust:** Khả năng tối ưu phần cứng và an toàn bộ nhớ:
  - WebAssembly (Wasm): rust là lựa chọn số 1 để viết các module hiệu năng cao chạy trên trình duyệt (như sử lý ảnh, video, game).
  - Tooling: Các công cụ xây dựng Web (Build tools) như Vite hay Turbopack đang đucợ viết lại bằng Rust để tăng tốc độ biên dịch gắp 10-100 lần
- **Go(Golang):** đơn giản và khả năng xử lý đồng thời(concurrency) cực tốt. Chuyên trị các hệ thống Microsevices, hạ tầng cloud-native và các hệ thống backend cần xử lý hàng triệu request cùng lúc. 

| Ngôn ngữ | Độ khó | Ưu điểm chính | Phù hợp nhất cho |
| :--- | :--- | :--- | :--- |
| **TypeScript** | Trung bình | "An toàn, chuyên nghiệp" | Mọi dự án Web hiện đại |
| **Python** | Dễ | Hệ sinh thái AI khổng lồ | "Web tích hợp AI, Data" |
| **Rust** | Khó, | "Tốc độ cực nhanh, an toàn" | "WebAssembly, Hệ thống lõi" |
| **Go** | Trung bình | Xử lý song song tốt | "Microservices, Cloud" |
| **PHP** | Dễ | "Phổ biến (WordPress, Laravel)" | "Website bán hàng, tin tức" |
# 2. Cơ chế hoạt động của website
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
























