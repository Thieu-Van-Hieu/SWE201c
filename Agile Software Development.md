# Agile Software Development

## Mục lục
1. [Khái niệm](#1-khai-niem)
2. [Các Framework/Phương pháp áp dụng Agile](#2-cac-frameworkphuong-phap-ap-dung-agile)
    1. [Scrum](#1-scrum)
    2. [Kanban](#2-kanban)
    3. [Extreme Programming (XP)](#3-extreme-programming-xp)
3. [Ưu, nhược điểm của Agile](#3-uu-nhuoc-diem-cua-agile)
4. [Ứng dụng của Agile](#4-ung-dung-cua-agile)
5. [Phương pháp làm việc Agile](#5-phuong-phap-lam-viec-agile)
6. [Tài liệu và Công cụ hỗ trợ Agile](#6-tai-lieu-va-cong-cu-ho-tro-agile)

<a name="1-khai-niem"></a>
## 1. Khái niệm

## Agile là gì?
- Agile là một phương pháp phát triển phần mềm
- Phương pháp này chia dự án thành các chu kỳ làm việc ngắn (Iteration hoặc Sprint)
- Mỗi chu kỳ sẽ có một sản phẩm hoàn chỉnh, có thể đưa vào sử dụng
- Sau khi đưa ra sản phẩm, sẽ đánh giá phản hồi và cải tiến cho các chu kfy tiếp theo

## Tư duy Agile
- **Giao tiếp và cộng tác**: Ưu tiên sự tương tác giữa các thành viên trong nhóm và khách hàng thay vì các tài liệu cứng nhắc
- **Phản hồi nhanh**: Sản phẩm được phát triển dựa trên phản hồi từ khách hàng, cho phép điều chỉnh nhanh theo thay đổi
- **Linh hoạt thay đổi**: Không bị ràng buộc bởi một kế hoạch cố định từ đầu, có thể thay đổi theo yêu cầu thực tế

&rArr; Thay vì lên kế hoạch chi tiết cho toàn bộ ứng dụng từ đầu, ta chỉ cần lên kế hoạch ngắn hạn cho mỗi Sprint (thường là 2-4 tuần), triển khai một số tính năng cơ bản, kiểm thử + nhận phản hồi &rarr; Điều chỉnh cho Sprint tiếp theo

<a name="2-cac-frameworkphuong-phap-ap-dung-agile"></a>
## 2. Các Framework/Phương pháp áp dụng Agile
Có một số framework và phương pháp luận thường dduocj áp dụng trong Agile:

<a name="1-scrum"></a>
### 1. Scrum
- **Cách hoạt động**:
    * Chia dự án thành các Sprint (thường là 2-4 tuần)
    * Tổ chức các cuộc họp: Sprint Planning, Daily Standup, Sprint Review, Sprint Retrospective
- **Vài trò chính**:
    * Product Owner: Xác định yêu cầu và ưu tiên trong Product Backlog
    * Scrum Master: Điều phối quy trình, hỗ trợ nhóm vượt qua các trở ngại
    * Development Team: Nhóm phát triển phần mềm làm chung trong một Sprint

<a name="2-kanban"></a>
### 2. Kanban
- **Cách hoạt động**:
    * Sử dụng bảng Kanban (Các cột "To Do", "Doing", "Done") để theo dõi tiến trình
    * Giới hạn số lượng công việc đang thực hiện (Work In Progress - WIP) để đảm bảo không quá tải
- **Đặc điểm**:
    * Không có Sprint cố định, công việc được xử lý liên tục dựa trên luồng công việc hàng ngày
    * Nhấn mạnh việc tối ưu hóa dòng công việc và tăng hiệu suất thông qua quan sát trực quan

<a name="3-extreme-programming-xp"></a>
### 3. Extreme Programming (XP)
- **Cách hoạt động**:
    * Tập trung vào việc phát triển phần mềm thông qua các kỹ thuật lập trình tốt nhất như:
        + Pair Programming (Lập trình cặp): Hai lập trình viên làm việc cùng nhau trên một máy tính, một người viết mã, một người kiểm thử
        + Test-Driven Development (TDD): Viết các bài kiểm thử trước khi viết mã
        + Continuous Integration: Tích hợp mã liên tục để phát hiện lỗi sớm
        + Refactoring: Cải tiến mã nguồn liên tục để duy trì chất lượng
- **Đặc điểm**:
    * Đảm bảo chất lượng code thông qua việc kiểm thử liên tục
    * Thường áp dụng cho môi trường đòi hỏi sản phẩm phải ổn định và bảo trì cao

<a name="3-uu-nhuoc-diem-cua-agile"></a>
## 3. Ưu, nhược điểm của Agile

### Ưu điểm
- **Linh hoạt**: Dễ dàng thay đổi yêu cầu dựa trên phản hồi của khách hàng
- **Nhanh chóng đưa ra sản phẩm**: Phát triển theo Sprint cho phép ra mắt phiên bản chạy ngay, dù không hoàn thiện 100%
- **Tăng cường giao tiếp**: Các cuộc họp thường xuyên và giao tiếp giữa các thành viên giúp nắm bắt kịp thời các bấn đề
- **Cải tiến liên tục**: Các phiên retrospective của Scrum giúp nhóm không ngừng học hỏi và cải tiến quy trình

### Nhược điểm
- **Không phù hợp với các dự án có yêu cầu cố định**: Đối với các dự án yêu cầu chi tiết ngay từ đầu (ví dụ phần mềm y tế, hệ thống an toàn), Agile có thể không đủ chặt chẽ
- **Kinh nghiệm của nhóm**: Cần có một đội ngũ có kinh nghiệm trong Agile để triển khai hiệu quả
- **Khó khăn trong việc báo cáo**: Vì yêu cầu thay đổi liên tục, việc dự báo chi phí và thời gian có thể trở nên khó khăn

<a name="4-ung-dung-cua-agile"></a>
## 4. Ứng dụng của Agile

### Agile trong các lĩnh vực
- **Ứng dụng di động và web**: Thị trường thay đổi liên tục, sản phẩm phải được cải tiến liên tục
- **Dự án khởi nghiệp (Startup)**: Có thể phát triển tính năng dựa trên phản hồi người dùng giúp tạo ra sản phẩm phù hợp
- **Dự án sáng tạo và nghiên cứu**: Khi yêu cầu không rõ ràng, Agile giúp nhóm có thể thử nghiệm và điều chỉnh dễ dàng

### Ví dụ ứng dụng cụ thể
- **Ứng dụng quản lý công việc**: Nhóm phát triển sử dụng Scrum để phân chia công việc, cập nhật tiến độ và nhận phản hồi của khách hàng sau mỗi Sprint
- **Hệ thống hỗ trợ khách hàng**: Sử dụng Kanban để theo dõi các yêu cầu hỗ trợ, đảm bảo mọi yêu cầu được xử lý kịp thời

<a name="5-phuong-phap-lam-viec-agile"></a>
## 5. Phương pháp làm việc Agile
Các yếu tố cơ bản trong phương pháp làm việc Agile:

### 1. Iterative & Incremental Development
- **Iterative**: Phát triển sản phẩm qua các vòng lặp, mỗi vòng lặp là một phiên bản cải tiến của sản phẩm
- **Incremental**: Xây dựng từng phần của sản phẩm một cách độc lập, sau đó kết hợp lại thành sản phẩm hoàn chỉnh

### 2. Các cuộc họp định kỳ
- **Daily Standup**: Họp ngắn mỗi ngày (~ 15 phút) để cập nhật tiến độ, vấn đề gặp phải
- **Sprint Planning**: Lên kế hoạch cho Sprint tiếp theo, xác định các tính năng cần phát triển
- **Sprint Review & Retrospective**: Sau mỗi Sprint, nhóm đánh giá lại sản phẩm đã hoàn thành và rút ra kinh nghiệm cải thiện quy trình làm việc

### 3. Tập trung vào giao tiếp và hợp tác
- Cộng tác giữa Product Owner, Scrum Master và Development Team giúp đảm bảo mọi người có cùng mục tiêu và hiểu rõ yêu cầu khách hàng

<a name="6-tai-lieu-va-cong-cu-ho-tro-agile"></a>
## 6. Tài liệu và Công cụ hỗ trợ Agile
Các công cụ phổ biến

### Quản lý công việc
- **Jira**: Quản lý dự án, theo dõi các task, bug và sắp xếp Sprint
- **Trello**: Quản lý công việc theo bảng Kanban, dễ sử dụng và trực quan

### Giao tiếp
- **Slack hoặc Microsoft Teams**: Tạo kênh trao đổi cho nhóm, hỗ trợ chia sẻ nhanh thông tin

### Công cụ tự động kiểm thử
- **GitHub Actions, GitLab CI/CD**: Tự động kiểm thử, tích hợp và triển khai sản phẩm

### Kiểm thử và theo dõi
- **SonarQube**: Phân tích chất lượng mã nguồn
- **TestRail**: Quản lý kế hoạch và kết quả kiểm thử

### Tài liệu và Quản lý yêu cầu
- **Confluence**: Lưu trữ tài liệu, ghi nhận yêu cầu của dự án
- **Notion**: Cũng là công cụ linh hoạt để quản lý tài liệu, ý tường và quy trình
