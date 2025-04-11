# Software Development Processes and Methodologies

## Nội dung
1. [Software Development Processes là gì?](#1-software-development-processes-la-gi)
2. [Các giai đoạn trong Software Development Lifecycle (SDLC)](#2-cac-giai-doan-trong-software-development-lifecycle-sdlc)
    - [Các giai đoạn chính](#cac-giai-doan-chinh)
    - [Requirements Analysis (Phân tích yêu cầu)](#1-requirements-analysis-phan-tich-yeu-cau)
    - [Design (Thiết kế)](#2-design-thiet-ke)
    - [Implementation (Lập trình)](#3-implementation-lap-trinh)
    - [Testing (Kiểm thử)](#4-testing-kiem-thu)
    - [Deployment (Triển khai)](#5-deployment-trien-khai)
    - [Maintenance (Bảo trì)](#6-maintenance-bao-tri)
3. [Các mô hình phổ biến trong Software Development](#3-cac-mo-hinh-pho-bien-trong-software-development)
    - [Khái quát về các mô hình phát triển phần mềm](#khai-quat-ve-cac-mo-hinh-phat-trien-phan-mem)
    - [Waterfall Model](#1-waterfall-model)
    - [V-Model](#2-v-model)
    - [Iterative Model](#3-iterative-model) 
    - [Incremental Model](#4-incremental-model)
    - [Spiral Model](#5-spiral-model)
    - [Agile Model](#6-agile-model)
4. [Các phương pháp luận (Methodologies)](#4-cac-phuong-phap-luan-methodologies)
    - [Khái quát về các phương pháp luận](#khai-quat-ve-cac-phuong-phap-luan)
    - [RUP (Rational Unified Process)](#1-rup-rational-unified-process)
    - [Scrum](#2-scrum)
    - [Kanban](#3-kanban)
    - [Extreme Programming (XP)](#4-extreme-programming-xp)
    - [Lean Software Development](#5-lean-software-development)
5. [Cách chọn mô hình và phương pháp phát triển phần mềm](#5-cach-chon-mo-hinh-va-phuong-phap-phat-trien-phan-mem)
6. [Công cụ hỗ trợ phát triển phần mềm](#6-cong-cu-ho-tro-phat-trien-phan-mem)
7. [Functional vs Non-Functional Requirements](#7-functional-vs-non-functional-requirements)

<a name="1-software-development-processes-la-gi"></a>
## 1. Software Development Processes là gì?

### Định nghĩa
- Software Development Process hay Quy trình phát triển phần mềm là tập hợp các bước, hoạt động, quy tắc và phương pháp được sử dụng để xây dựng một phần mềm từ ý tưởng &rarr; triển khai &rarr; bảo trì. 

&rArr; Đây là cách để biến "ý tưởng" thành một sản phẩm phần mềm hoàn chỉnh

### Vì sao cần có quy trình?
- Nếu không có quy trình:
  * Dễ bị rối, không biết làm gì trước, làm gì sau
  * Dễ sai yêu cầu khách hàng
  * Khó quản lý thời gian, ngân sách và nhân lực
  * Chất lượng phần mềm thấp, nhiều lỗi, khó mở rộng
- Tác dụng:
  * Làm đúng yêu cầu người dùng
  * Kiểm soát chất lượng phần mềm
  * Dễ phối hợp nhóm

<a name="2-cac-giai-doan-trong-software-development-lifecycle-sdlc"></a>
## 2. Các giai đoạn trong Software Development Lifecycle (SDLC)

<a name="cac-giai-doan-chinh"></a>
### Khái quát về các giai đoạn
| Giai đoạn                                    | Mô tả                                 | Kết quả                 |
|----------------------------------------------|---------------------------------------|-------------------------|
| 1. Requirements Analysis (Phân tích yêu cầu) | Xác định yêu cầu của khách hàng       | Tài liệu yêu cầu (SRS)  |
| 2. Design (Thiết kế)                         | Thiết kế kiến trúc, UI/UX, DB         | UI/UX, ERD, kế hoạch    |
| 3. Implementation (Lập trình)                | Viết mã nguồn theo thiết kế           | Chạy được phần mềm      |
| 4. Testing (Kiểm thử)                        | Đảm bảo phần mềm chạy đúng và ổn định | Phần mềm ổn định        |
| 5. Deployment (Triển khai)                   | Đưa phần mềm vào sử dụng              | Người dùng sử dụng được |
| 6. Maintenance (Bảo trì)                     | Sửa lỗi, cập nhật khi có yêu cầu mới  | Phần mềm lâu dài        |

&rArr; Thứ tự của các giai đoạn có thể thay đổi tùy theo mô hình phát triển phần mềm

### Các giai đoạn

<a name="1-requirements-analysis-phan-tich-yeu-cau"></a>
#### 1. Requirements Analysis (Phân tích yêu cầu)
- **Mục tiêu**:
    * Hiểu khách hàng muốn gì
    * Xác định các chức năng, tính năng phần mềm cần có
- **Ai tham gia**:
    * Bussiness Analyst, khách hàng, Project Manager, Developer
- **Công việc**:
    * Phỏng vấn khách hàng, khảo sát, họp
    * Ghi lại yêu cầu (functional, non-functional)
    * Viết tài liệu (Software Requirements Specification - SRS)

<a name="2-design-thiet-ke"></a>
#### 2. Design (Thiết kế)
- **Mục tiêu**:
    * Biến yêu cầu thành thiết kế chi tiết về giao diện, cơ sở dữ liệu, kiến trúc
- **Ai tham gia**:
    * System Architect, UI/UX Designer, Dev lead
- **Công việc**:
    * Thiết kế giao diện người dùng (mockup, wireframe)
    * Thiết kế cơ sở dữ liệu (ERD)
    * Thiết kế kiến trúc hệ thống (microservice, MVC, ...)
    * Lập kế hoạch kỹ thuật (công nghệ, công cụ sẽ dùng)

<a name="3-implementation-lap-trinh"></a>
#### 3. Implementation (Lập trình)
- **Mục tiêu**:
    * Viết mã nguồn theo thiết kế
- **Ai tham gia**:
    * Developer (Frontend, Backend, Mobile, ...), DevOps
- **Công việc**:
    * Lập trình theo module đã thiết kế
    * Đẩm bảo viết code sạch, đúng chuẩn
    * Tạo pull request, review code

<a name="4-testing-kiem-thu"></a>
#### 4. Testing (Kiểm thử)
- **Mục tiêu**:
    * Đảm bảo phần mềm chạy đúng yêu cầu, không lỗi
- **Ai tham gia**:
    * QA Tester, Developer
- **Các loại kiểm thử**:
    * Unit test: Kiểm thử từng hàm nhỏ
    * Integration test: Kiểm thử các phần có hoạt động chung với nhau không
    * System test: Kiểm thử toàn bộ hệ thống
    * Acceptance test: Kiểm thử với khách hàng

<a name="5-deployment-trien-khai"></a>
#### 5. Deployment (Triển khai)
- **Mục tiêu**:
    * Đưa phần mềm vào sử dụng thực tế
- **Ai tham gia**:
    * DevOps, Developer, Project Manager
- **Công việc**:
    * Cấu hình server, build project, upload code
    * Cài đặt database, domain, SSL, ...
    * Dùng CI/CD để tự động hóa (Jenkins, GitHub Actions, ...)

<a name="6-maintenance-bao-tri"></a>
#### 6. Maintenance (Bảo trì)
- **Mục tiêu**:
    * Giữ cho phần mềm ổn định, sửa lỗi, cập nhật tính năng mới
- **Ai tham gia**:
    * Developer, QA, DevOps, Support
- **Công việc**:
    * Sửa lỗi nếu người dùng báo
    * Thêm tính năng mới
    * Cập nhật công nghệ và vá lỗi bảo mật

<a name="3-cac-mo-hinh-pho-bien-trong-software-development"></a>
## 3. Các mô hình phổ biến trong Software Development

<a name="khai-quat-ve-cac-mo-hinh-phat-trien-phan-mem"></a>
### Khái quát về các mô hình phát triển phần mềm

#### Khái quát
| Mô hình     | Đặc điểm chính                                                         | Phù hợp với                                   |
|-------------|------------------------------------------------------------------------|-----------------------------------------------|
| Waterfall   | Tuần tự, không quay lại bước trước                                     | Yêu cầu rõ ràng, ít thay đổi                  |
| V-Model     | Giống Waterfall, nhưng tập trung vào kiểm thử song song với phát triển | Hệ thống lớn, yêu cầu kiểm thử cao            |
| Iterative   | Phát triển qua nhiều vòng lặp, cải tiến dần                            | Yêu cầu chưa rõ ràng, cần kiểm nghiệm dần     |
| Incremental | Chia nhỏ thành nhiều phần, mỗi phần hoạt động độc lập                  | Dự án có thể chia nhỏ module                  |
| Spiral      | Kết hợp giữa lặp và quản lý rủi ro                                     | Dự án lớn, phức tạp, rủi ro cao               |
| Aigle       | Linh hoạt, phản hồi nhanh với thay đổi                                 | Dự án thay đổi thường xuyên, cần teamwork tốt |

#### So sánh nhanh
| Mô hình     | Linh hoạt | Phản hồi nhanh | Kiểm thử kỹ | Quản lý dễ | Phù hợp với                |
|-------------|-----------|----------------|-------------|------------|----------------------------|
| Waterfall   | Không     | Không          | Trung bình  | Dễ         | Dự án nhỏ, yêu cầu rõ ràng |
| V-Model     | Không     | Không          | Cao         | Dễ         | Dự án cần kiểm thử kỹ      |
| Iterative   | Có        | Có             | Cao         | Trung bình | Dự án cần cái tiến dần     |
| Incremental | Có        | Có             | Cao         | Dễ         | Dự án chia phần được       |
| Spiral      | Có        | Có             | Cao         | Khó        | Dự án lớn, rủi ro cao      |
| Agile       | Có        | Có             | Cao         | Dễ         | Dự án thay đổi liên tục    |

&rArr; Các mô hình không cạnh tranh nhau mà tùy vào dự án sẽ chọn mô hình phù hợp

### Các mô hình

<a name="1-waterfall-model"></a>
#### 1. Waterfall Model
- **Đặc điểm**:
    * Làm theo trình tự cố định
    * Từng bước rõ ràng từ trên xuống dưới
    * Không quay lại bước trước
    * Mỗi bước phải hoàn thành mới đến bước tiếp theo
- **Phù hợp với**:
    * Dự án nhỏ 
    * Có yêu cầu rõ ràng, ít thay đổi
- **Cách làm**: Tuần tự theo 6 giai đoạn đã liệt kê ở trên
- **Ưu điểm**:
    * Quá trình rõ ràng 
    * Dễ kiểm soát tiến độ
- **Nhược điểm**: 
    * Thiếu tính linh hoạt
    * Khi thay đổi yêu cầu sẽ phải làm lại từ đầu

<a name="2-v-model"></a>
#### 2. V-Model
- **Đặc điểm**:
    * Giống Waterfall nhưng tập trung vào kiểm thử
    * Khi xong mỗi bước là thực hiện kiểm thử cho bước đó
    * Hình dạng chứ "V" ám chỉ mối quan hệ đối xứng giữa phát triển và kiểm thử
- **Phù hợp với**:
    * Dự án lớn
    * Yêu cầu kiểm thử cao
    * Đảm bảo chất lượng chặt chẽ
- **Cách làm**:
    1. Xác định yêu cầu và lên ý tường
    2. Thiết kế tổng thể và chi tiết
    3. Khi lập trình kết hợp song song với kiểm thử cho từng phần
    4. Thực hiện kiểm thử đơn vị, tích hợp và hệ thống tương ứng sau mỗi giai đoạn
- **Ưu điểm**: Giúp phát hiện lỗi sớm
- **Nhược điểm**:
    * Thiếu linh hoạt
    * Cần nhiều chi phí, thời gian phát triển do cần kiểm thử từng phần

<a name="3-iterative-model"></a>
#### 3. Iterative Model
- **Đặc điểm**:
    * Tập trung xây dựng phiên bản đầu tiên của sản phẩm (Dù chưa hoàn thiện)
    * Sau đó cải tiến dần qua nhiều vòng lặp
    * Mỗi vòng lặp là một phiên bản cải tiến
- **Phù hợp với**:
    * Dự án có yêu cầu ban đầu chưa rõ ràng
    * Cần thu thập phản hồi từ người dùng để điều chỉnh
- **Cách làm**:
    1. Phát triển một phiên bản cơ bản của sản phẩm
    2. Thu thập phản hồi từ người dùng và đánh giá những điểm chưa hoàn thiện
    3. Điều chỉnh, bổ sung và nâng cấp sản phầm trong phiên bản tiếp theo
    4. Lặp lại quá trình này cho đến khi sản phẩm hoàn thiện
- **Ưu điểm**: Linh hoạt, dễ thay đổi theo yêu cầu
- **Nhược điểm**:
    * Không có phhieen bản hoàn thiện từ đầu
    * Việc lặp lại liên tục có thể gây tốn thời gian

<a name="4-incremental-model"></a>
#### 4. Incremental Model
- **Đặc điểm**: 
    * Chia sản phẩm thành các phần nhỏ, độc lập
    * Mỗi phần là một tính năng hoàn chỉnh
    * Các thành phần sẽ được hợp lại để tạo thành sản phẩm
- **Phù hợp với**:
    * Dự án có thể chia nhỏ
    * Các tính năng độc lập
- **Cách làm**:
    1. Xác định tính năng hoặc phần của sản phẩm cần phát triển
    2. Phát triển từng tính năng một cách độc lập
    3. Kết hợp các tính năng lại với nhau để thành hệ thống hoàn chỉnh
- **Ưu điểm**:
    * Cho phép phát hành sớm các tính năng hoàn chỉnh
    * Ít rủi ro tổng thể vì mỗi phần được xây dựng độc lập
- **Nhược điểm**: Việc kết hợp các phần lại với nhau có thể gặp khó khăn nếu không có sự đồng bộ và thiết kế ban đầu không chặt chẽ

<a name="5-spiral-model"></a>
#### 5. Spiral Model
- **Đặc điểm**:
    * Kết hợp giữa Iterative và việc quản lý rủi ro
    * Mỗi vòng xoắn bao gồm việc xác định mục tiêu, lập kế hoạch, phát triển, kiểm thử và đánh giá rủi ro
- **Phù hợp với**:
    * Dự án lớn, phức tạp
    * Có nhiều rủi ro cần được quản lý
- **Cách làm**:
    1. Xác định yêu cầu và mục tiêu cho vòng đầu tiên
    2. Lập kế hoạch, thực hiện phát triển và kiểm thử, đồng thời đánh giá các rủi ro liên quan
    3. Dựa vào kết quả và đánh giá, lập kế hoạch cho vòng xoắn tiếp theo với các cải tiến cần thiết
    4. Lặp lại quá trình cho đến khi sản phẩm hoàn thiện
- **Ưu điểm**:
    * Quản lý rủi ro tốt
    * Linh hoạt trong việc thay đổi theo các rủi ro mới
- **Nhược điểm**:
    * Phức tạp và tốn kém
    * Cần nhiều thời gian, kinh phí để quản lý và đánh giá liên tục
    * Có thể không phù hợp với dự án nhỏ

<a name="6-agile-model"></a>
#### 6. Agile Model
- **Đặc điểm**:
    * Phát triển theo các khoảng thời gian ngắn thường gọi là vòng hoặc giai đoạn
    * Mỗi vòng là một phiên bản hoàn chỉnh của sản phẩm
- **Phù hợp với**:
    * Dự án cần đáp ứng nhanh, thay đổi liên tục
    * Cần sự hợp tác chặt chẽ giữa nhóm phát triển và khách hàng
- **Cách làm**:
    1. Chia dự án thành các giai đoạn ngắn (Thường là 1-4 tuần)
    2. Phát triển trong mỗi giai đoạn một số tính năng cụ thể
    3. Sau mỗi giai đoạn, nhóm phát triển thu thập đánh giá, phản hồi để cải tiến trong giai đoạn tiếp theo
    4. Tiếp tục cải tiến cho đến khi được sản phẩm cuối cùng
- **Ưu điểm**:
    * Rất linh hoạt, thích ứng nhanh với thay đổi
    * Sản phẩm phù hợp với nhu cầu người dùng
- **Nhược điểm**:
    * Đòi hỏi sự hợp tác và giao tiếp liên tục
    * Có thể khó kiểm soát nếu không có quy trình rõ ràng

<a name="4-cac-phuong-phap-luan-methodologies"></a>
## 4. Các phương pháp luận (Methodologies)

<a name="khai-quat-ve-cac-phuong-phap-luan"></a>
### Khái quát về các phương pháp luận
| Phương pháp luận | Đặc điểm chính                                                               |
|------------------|------------------------------------------------------------------------------|
| RUP              | Chia dự án thành 4 giai đoạn: Khởi đầu, lên kế hoạch, phát triển và bàn giao |
| Scrum            | Làm việc theo các giai đoạn ngắn gọi là Sprint (2-4 tuần)                    |
| Kanban           | Quản lý công việc bằng bảng với các cột như "Cần làm", "Đang làm", "Đã xong" |
| XP               | Tập trung vào việc phát triển + kiểm thử thường xuyên và làm việc nhóm       |
| Lean             | Tối ưu quy trình phát triển, ưu tiên sản phẩm                                |

&rArr; Hiểu đơn giản thì các phương pháp luận là cách mà ta áp dụng các mô hình phát triển phần mềm

### Các phương pháp luận

<a name="1-rup-rational-unified-process"></a>
#### 1. RUP (Rational Unified Process)
- **Khái niệm**:
    * Là một quy trình phát triển phần mềm hướng đối tượng
    * Có quy trình rõ ràng, được chia thành 4 giai đoạn
- **4 giai đoạn chính**:
    * **Inception (Khởi đầu)**:
        + Xác định mục tiêu
        + Xác định phạm vi dự án
        + Xác minh tính khả thi
    * **Elaboration (Lên kế hoạch)**:
        + Phân tích yêu cầu
        + Xây dựng kiến trúc sơ bộ
        + Lên kế hoạch chi tiết
    * **Construction (Phát triển)**:
        + Phát triển phần mềm
        + Kiểm thử các module
    * **Transition (Bàn giao)**:
        + Triển khai phần mềm
        + Thu thập phản hồi và điều chỉnh
- **Điểm nổi bật**:
    * Phù hợp với các dự án lớn, yêu cầu quy trình rõ ràng
    * Kiểm soát rủi ro tốt qua từng giai đoạn phát triển

<a name="2-scrum"></a>
#### 2. Scrum
- **Khái niệm**:
    * Là một phương pháp Agile phổ biến
    * Chia dự án thành các chu kỳ làm việc ngắn gọi là Sprint (2-4 tuần)
- **Các vai trò chính**:
    * Product Owner: Đại diện khách hàng, quyết định thứ tự ưu tiên các yêu cầu
    * Scrum Master: Hỗ trợ nhóm, gỡ rối và đảm bảo quy trình Scrum được thực hiện đúng
    * Development Team: Nhóm phát triển chịu trách nhiệm xây dựng sản phẩm
- **Quy trình cơ bản**:
    * Product Backlog: Danh sách các yêu cầu cần làm
    * Sprint Planning: Chọn yêu cầu từ backlog cho sprint hiện tại
    * Sprint: Làm việc trong khoảng thời gian cố định
    * Daily Scrum: Họp hàng ngày để cập nhật tiến độ
    * Sprint Review & Retrospective: Đánh giá kết quả và cải tiến quy trình
- **Điểm nổi bật**:
    * Tạo ra sản phẩm theo từng đợt
    * Linh hoạt thay đổi khi có phản hồi

<a name="3-kanban"></a>
#### 3. Kanban
- **Khái niệm**:
    * Là một phương pháp tập trung vào quản lý công việc theo luồng liên tục
    * Sử dụng bảng Kanban để theo dõi tiến độ công việc
    * Giới hạn số lượng công việc đang thực hiện để tránh quá tải
- **Cách hoạt động của bảng Kanban**:
    * Các cột trên bảng: "To Do", "In Progress", "Done"
    * Giới hạn số lượng công việc: Xác định số lượng công việc tối đa cho mỗi cột, đảm bảo nhóm tập trung hoàn thành công việc hiện tại trước khi nhận thêm việc mới
- **Điểm nổi bật**:
    * Giúp theo dõi trạng thái công việc một cách trực quan
    * Linh hoạt thích ứng với các thay đổi và ưu tiên mới

<a name="4-extreme-programming-xp"></a>
#### 4. Extreme Programming (XP)
- **Khái niệm**:
    * Là một phương pháp tập trung vào chất lượng mã nguồn và thực hành kỹ thuật lập trình
    * Khuyến khích viết code sạch, kiểm thử liên tục và hợp tác nhóm chặt chẽ
- **Kỹ thuật chính**:
    * **Pair Programing**: Hai lập trình viên làm việc chung, một người viết code, một người check code
    * **Test-Driven Development (TDD)**: Viết các bài kiểm thử, sau đó viết mã nguồn để vượt qua các bài kiểm thử đó
    * **Continuous Integration (CI)**: Tích hợp mã nguồn liên tục, kiểm thử tự động
    * **Refactoring**: Cải tiến mã nguồn liên tục mà không thay đổi chức năng tổng thể
- **Điểm nổi bật**:
    * Tạo ra mã nguồn chất lượng cao, dễ bảo trì
    * Nhấn mạnh việc kiểm thử và cải tiến liên tục

<a name="5-lean-software-development"></a>
#### 5. Lean Software Development
- **Khái niệm**:
    * Là một phương pháp phát triển phần mềm dựa trên triết lý sản xuất của Toyota
    * Tối ưu hóa quy trình làm việc bằng cách loại bỏ mọi lãng phí và tập trung vào việc tạo giá trị cao nhất cho khách hàng
- **Nguyên tắc cốt lõi**:
    * **Loại bỏ lãng phí (Eliminate Waste)**: Xác định và loại bỏ những hoạt động không cần thiết
    * **Khuếch đại học hỏi (Amplify Learning)**: Luôn học hỏi và cải tiến từng giai đoạn
    * **Quyết định càng trễ càng tốt (Decide as Late as Possible)**: Chỉ đưa ra quyết định khi có đủ thông tin, cơ hội tối đa và thật sự cần thiết
    * **Giao hàng nhanh (Deliver as Fast as Possible)**: Tạo ra sản phẩm nhanh chóng để nhận phản hồi
    * **Trao quyền cho nhóm (Empower the Team)**: Đưa quyền quyết định cho nhóm làm việc trực tiếp với vấn đề
    * **Xây dựng chất lượng (Build Quality In)**: Đảm bảo chất lượng từ đầu, không phải sửa chữa sau
    * **Tối ưu hóa toàn cục (Optimize the Whole)**: Không tối ưu từng phần mà cần nhìn nhận tổng thể quy trình
- **Điểm nổi bật**:
    * Giúp giảm thiểu lãng phí về thời gian, nguồn lực và chi phí
    * Tập trung vào việc cải tiến liên tục và tạo giá trị thực cho khác hàng

<a name="5-cach-chon-mo-hinh-va-phuong-phap-phat-trien-phan-mem"></a>
## 5. Cách chọn mô hình và phương pháp phát triển phần mềm
| Tình huống                                     | Khuyến nghị                     |
|------------------------------------------------|---------------------------------|
| Dự án lớn, yêu cầu rõ dần, cần tài liệu đầy đủ | RUP                             |
| Yêu cầu rõ, không thay đổi                     | Waterfall, V-Model              |
| Yêu cầu mở hồ, thay đổi liên tục               | Agile (Scrum, Kaban), Iterative |
| Dự án lớn, phức tạp, cần phân tích rủi ro      | Spiral                          |
| Hệ thống có thể chia thành các module rõ ràng  | Incremental                     |
| Ưu tiên chất lượng code                        | XP                              |
| Tối ưu hiệu quả, loại bỏ lãng phí              | Lean                            |

<a name="6-cong-cu-ho-tro-phat-trien-phan-mem"></a>
## 6. Công cụ hỗ trợ phát triển phần mềm

| Công cụ                 | Chức năng                          |
|-------------------------|------------------------------------|
| Jira, Trello            | Quản lý công việc, sprint, backlog |
| Confluence              | Ghi chú tài liệu, yêu cầu          |
| Git, Github, GitLab     | Quản lý mã nguồn, version control  |
| Figma, Lucidchart       | Thiết kế UI, sơ đồ hệ thống        |
| Jenkins, GitHub Actions | Tự động hóa build, test, deploy    |

<a name="7-functional-vs-non-functional-requirements"></a>
## 7. Functional vs Non-Functional Requirements

### Functional Requirements là gì?
- Là các yêu cầu về chức năng, nhưng việc phần mềm cần làm
- Nó trả lời cho câu hỏi "Phần mềm này cần làm gì?"

### Non-Functional Requirements là gì?
- Là các yêu cầu liên quan đến cách phần mềm hoạt động như chất lượng, hiệu suất, bảo mật, khả năng mở rộng, ...
- Nó trả lời cho câu hỏi "Phần mềm này cần hoạt động như thế nào?"

### So sánh
|                         | Functional                        | Non-Functional                   |
|-------------------------|-----------------------------------|----------------------------------|
| Trả lời cho câu hỏi gì? | Hệ thống làm gì?                  | Hệ thống hoạt động như thế nào?  |
| Dạng yêu cầu            | Tính năng cụ thể                  | Đặc tính chất lượng              |
| Ví dụ                   | Đăng nhập, tìm kiếm               | Nhanh, ổn định, bảo mật, dễ dùng |
| Kiểm thử như thế nào?   | Kiểm tra chức năng hoạt động đúng | Kiểm tra hiệu năng, bảo mật, ... |

### Ví dụ
| Loại yêu cầu   | Ví dụ                                               |
|----------------|-----------------------------------------------------|
| Functional     | Người dùng có thể thêm sản phẩm vào giỏ hàng        |
| Functional     | hệ thống tính tiền tự động                          |
| Non-Functional | Ứng dụng tải xong trong vòng 1 giây trên điện thoại |
| Non-Functional | Giao diện hiển thị tốt trên mọi kích cỡ màn hình    |
