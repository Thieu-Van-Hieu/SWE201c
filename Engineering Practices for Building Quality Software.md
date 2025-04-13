# Engineering Practices for Building Quality Software

## Mục lục
- [1. Clean Code - Viết mã sạch](#1-clean-code)
- [2. Refactoring - Tái cấu trúc mã](#2-refactoring)
- [3. Software Testing - Kiểm thử phần mềm](#3-software-testing)
- [4. Continuous Integration and Continuous Deployment (CI/CD) - Tích hợp liên tục và triển khai liên tục](#4-continuous-integration-and-continuous-deployment-cicd)
- [5. Version Control - Kiểm soát phiên bản](#5-version-control)
- [6. Code Reviews & Pair Programming](#6-code-reviews--pair-programming)
- [7. Static Analysis & Linters - Phân tích tĩnh và chuẩn code](#7-static-analysis--linters)
- [8. Performance & Maintainability](#8-performance--maintainability)

<a name="1-clean-code"></a>
## 1. Clean Code
- **Định nghĩa**:
    * Clean Code là cách viết code sao cho dễ đọc, dễ hiểu và dễ bảo trì
    * Mã nguồn có cấu trúc rõ ràng, tên biến, hàm và class phải có ý nghĩa
- **Các nguyên tắc cơ bản**:
    * **Đặt tên rõ ràng**: Tên biến, tên hàm nên phản ánh chính xác chức năng của chúng
    * **Tách biệt rõ ràng**: Mỗi hàm chỉ nên thực hiện một nhiệm vụ duy nhất
    * **Không lặp lại mã**: Tránh việc sao chép mã nguồn, thay vào đó hãy tái sử dụng bằng cách tách thành hàm hoặc module riêng

<a name="2-refactoring"></a>
## 2. Refactoring
- **Định nghĩa**:
    * Là quá trình cải thiện cấu trúc của mã nguồn mà vẫn giữ nguyên chức năng
- **Mục tiêu**: Làm cho code sạch hơn
- **Các bước thường thực hiện**:
    * Xác định đoạn code khó hieru hoặc lặp lại nhiều
    * Tách riêng thành hàm hoặc class
    * Kiểm tra lại bằng các bài test để đảm bảo vẫn giữ nguyên chức năng

&rArr; Luôn chạy test sau khi refactor để đảm bảo không làm hỏng chức năng

<a name="3-software-testing"></a>
## 3. Software Testing
- **Các loại kiểm thử**:
    * **Unit Testing**: Kiểm thử từng đơn vị nhỏ của ứng dụng như hàm, module
    * **Integration Testing**: Kiểm tra sự phối hợp giữa các module, đảm bảo chúng hoạt động cùng nhau
    * **System Testing**: Kiểm tra tổng hợp hệ thống khi tất cả module được tích hợp
- **Test-Driven Development (TDD)**:
    * Viết bài test trước, sau đó mới viết code để đáp ứng bài test đó
    * Giúp đảm bảo rằng code được viết ra có mục đích rõ ràng và luôn được kiểm thử
- **Behavior-Driven Development (BDD)**:
    * Tương tự như TDD nhưng sẽ kiểm tra những việc mà người dùng sẽ thực hiện

<a name="4-continuous-integration-and-continuous-deployment-cicd"></a>
## 4. Continuous Integration and Continuous Deployment (CI/CD)
- **Khái niệm**:
    * CI (Continuous Integration): Thêm code mới và nhánh chính thường xuyên, chạy test tự động để phát hiện lỗi sớm
    * CD (Continuous Deployment): Sau khi thêm code mới, tự động triển khai lên môi trường sản xuất
- **Quy trình cơ bản**:
    1. Lập trình viên commit code lên repository
    2. Hệ thống CI (như GitHub Actions, Jenkins) tự động build và kiểm thử code
    3. Nếu tất cả các bài test đều pass, hệ thống sẽ tự động triển khai ứng dụng
- **Lợi ích**:
    * Tiết kiệm thời gian kiểm thử thủ công
    * Phát hiện lỗi khi mới commit, giúp sửa lỗi nhanh chóng

<a name="5-version-control"></a>
## 5. Version Control
- **Định nghĩa**: Là một hệ thống quản lý các phiên bản của mã nguồn qua đó giúp theo dõi cac thay đổi trong mã nguồn và hỗ trợ làm việc nhóm hiệu quả
- **Các thao tác cơ bản**:
    * **Clone**: Sao chép repository về máy
    * **Commit**: Ghi lại các thay đổi cùng thông điệp mô tả
    * **Branch**: Tạo nhanh để phát triển tính năng mới mà không ảnh hưởng đến nhanh chính
    * **Merge**: Gộp các tính năng khi đã hoàn thiện
- **Git Workflow**:
    * **Git Flow**: Chia repository thành các nhanh như develope, master và các nhanh feature/hotfix
    * **Trunk-based Development**: Toàn bộ nhóm làm việc trên một nhánh chính (trunk) và thường xuyên commit lên nhánh này
- **Ví dụ**: Khi làm một dự án mới, bạn tạo nhanh feature/login để phát triển tính năng đăng nhập. Sau khi hoàn thành và kiểm thử, nhánh này được merge vào nhánh chính

<a name="6-code-reviews--pair-programming"></a>
## 6. Code Reviews & Pair Programming
- **Code Reviews**:
    * Là quá trình các thành viên nhóm kiểm tra code của nhau để phát hiện lỗi, cải thiện chất lượng và chia sẻ kiến thức
    * Thường được thực hiện qua pull request
- **Pair Programming**:
    * Hai lập trình viên làm việc cùng nhau trên một máy tính
    * Một người viết code (Driver) và một người xem xét (Observer)
- **Lợi ích**:
    * Giảm thiểu lỗi, cải thiện chất lượng mã
    * Tăng cường giao tiếp và học hỏi giữa các thành viên

<a name="7-static-analysis--linters"></a>
## 7. Static Analysis & Linters
- **Static Analysis**: Là quá trình sử dụng công cụ để kiểm tra mã nguồn mà không cần chạy chương trình qua đó tìm ra các lỗi tiềm ẩn, vi phạm quy tắc viết code hay lỗ hổng bảo mật
- **Linters**: Là công cụ giúp kiểm tra phong cách viết code, đảm bảo code nhất quán theo quy tắc đã định
- **Cách áp dụng**:
    * Các công cụ này thường được tích hợp vào quá trình CI để tự động quét và cảnh báo lỗi
    * Giúp phát hiện lỗi sớm và cải thiện chất lượng code theo thời gian

<a name="8-performance--maintainability"></a>
## 8. Performance & Maintainability
- **Performance** (Hiệu năng)**:
    * Viết code sao cho tối ưu tốc độ và sử dụng tài nguyên hợp lý
    * Áp dụng các kỹ thuật như caching, profiling để phát hiện và tối ưu các đoạn mã chậm
- **Maintainability (Khả năng bảo trì)**:
    * Thiết kế hệ thống sao cho khi cần mở rộng hoặc sửa lỗi, bạn có thể dễ dàng thực hiện
    * Áp dụng các chuẩn thiết kế, thiết lập cấu trúc folder rõ ràng, và viết tài liệu hướng dẫn
- **Kỹ thuật thực tiễn**:
    * **Profiling**: Sử dụng các công cụ để đo lường hiệu năng
    * **Design Patterns**: Áp dụng các mẫu thiết kế để tăng tính tái sử dụng và dễ bảo trì
