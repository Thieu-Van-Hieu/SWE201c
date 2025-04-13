# Lean Software Development

## Mục lục
1. [Lean là gì?](#1-lean-la-gi)
2. [Nguyên tắc Lean](#2-nguyen-tac-lean)
3. [So sánh Lean và Agile](#3-so-sanh-lean-va-agile)
4. [Ứng dụng Lean trong phần mềm](#4-ung-dung-lean-trong-phan-mem)
5. [Các công cụ hỗ trợ Lean](#5-cac-cong-cu-ho-tro-lean)
6. [Ưu, nhược điểm của Lean](#6-uu-nhuoc-diem-cua-lean)

<a name="1-lean-la-gi"></a>
## 1. Lean là gì?
- Lean Software Developerment là ứng dụng tư duy "Lean", triết lý trong ngành sản xuất ô tô của Toyota vào phát triển phần mềm
- **Mục tiêu**: Tôi đa hóa giá trị mang lại cho khách hàng bằng cách loại bỏ hoạt động không cần thiết ("lãng phí") trong quy trình làm việc
- **Tư duy**:
    * Tập trung vào việc tạo giá trị thực sự cho người dùng
    * Liên tục cải tiến quy trình, giảm thời gian phát triển và nguồn lực lãng phí
- **Ví dụ**: Thay vì đầu từ thời gian vào việc tạo tài liệu hay các bước xử lý phức tạp không trực tiếp giúp phần mềm trở nên hữu ích, nhóm Lean sẽ tập trung nhanh chóng phát triển tính năng cốt lõi để khách hàng có thể sử dụng và phản hồi

<a name="2-nguyen-tac-lean"></a>
## 2. Nguyên tắc Lean
1. **Loại bỏ lãng phí (Eliminate Waste)**
    - **Ý nghĩa**: Xác định và loại bỏ những thứ không mang lại giá trị cho khách hàng
    - **Áp dụng**:
        * Loại bỏ tính năng thừa thãi, quy trình không cần thiết
        * Tối ưu hóa quy trình làm việc, tránh các bước "cho có"
    - **Ví dụ**: Nếu một module được xây dựng nhưng lại không được sử dụng hoặc ít mang lại lợi ích, nhóm có thể bỏ hoặc giảm bớt đầu tư vào nó
2. **Tăng cường học hỏi (Amplify Learning)**
    - **Ý nghĩa**: Luôn thu thập, xử lý và áp dụng phản hồi từ khách hàng vào quá trình phát triển
    - **Áp dụng**:
        * Thường xuyên tổ chức các cuộc họp retrospective để đánh giá quy trình làm việc
        * Áp dụng các thử nghiệm nhỏ để kiểm tra ý tưởng mới
    - **Ví dụ**: Sau mỗi vòng phát triển, nhóm họp lại và đánh giá xem tính năng có đáp ứng được nhu cầu người dùng không và học hỏi từ lỗi sai để cải thiện trong vòng kế tiếp
3. **Ra quyết định càng muộn càng tốt (Decide as late as possible)**
    - **Ý nghĩa**: Không quyết định sớm mà đợi đến khi đủ thông tin để đưa ra quyết định chính xác hơn
    - **Áp dụng**:
        * Không có định quá sớm các chi tiết thiết kế hay công nghệ
        * Cho phép các thay đổi thiết kế khi có thêm dữ liệu và phản hồi
    - **Ví dụ**: Trong giai đoạn đầu dự án, nhóm có thể chọn một kiến trúc mềm dẻo, sau đó tinh chỉnh các quyết định về công nghệ cho phù hợp khi biết rõ hơn về khối lượng và tính chất của dữ liệu thực tế
4. **Giao hàng càng sớm càng tốt (Deliver as fast as possible)**
    - **Ý nghĩa**: Tốc độ đưa sản phẩm ra thị trường nhanh giúp nhận được phản hồi sớm từ khách hàng qua đó có thể cải thiện sản phẩm cho phù hợp hơn
    - **Áp dụng**:
        * Triển khai sản phầm dưới dạng MVP (Minimum Viable Product) - phiên bản với tính năng cốt lõi
        * Rút ngắn thời gian phát triển bằng cách chia nhỏ dự án thành các phiên bản nhỏ
    - **Ví dụ**: Một startup sẽ đưa ra MVP để kiểm chứng thị trường thay vì chờ sản phẩm hoàn thiện 100% trong vài năm
5. **Trao quyền nhóm (Empower the Team)**
    - **Ý nghĩa**: Tạo điều kiện cho đội nhóm chủ động sáng tạo và giải quyết vấn đề
    - **Áp dụng**:
        * Khuyến khích nhóm tự quyết định để giải quyết vấn đề
        * Tạo môi trường làm việc cởi mở, nơi mọ ý kiến được lắng nghe và trọn dụng
    - **Ví dụ**: Nhóm phát triển Agile-lean có thể đưa ra quyết định về cách tối ưu lập trình mà không cần phê duyệt từ cấp trên cho từng chi tiết nhỏ, từ đó tăng tốc độ và tính sáng tạo
6. **Tích hợp chất lượng (Build Quality In)**
    - **Ý nghĩa**: Đảm bảo chất lượng được xây dựng ngay từ đầu thay vì kiểm tra sau cùng
    - **Áp dụng**:
        * Áp dụng kiểm thử tự động
        * Lập trình theo tiêu chuẩn và thực hành refactoring định kỳ
    - **Ví dụ**: Khi sử dụng kiểm thử trước, lập trình viên sẽ viết bài test trước và chỉ tiếp tục viết mã khi bài test đó pass, đảm bảo chất lượng ngay từ đầu
7. **Tối ưu hóa toàn bộ (Optimize the Whole)**
    - **Ý nghĩa**: Xem xét toàn bộ hệ thống thay vì từng phần riêng lẻ, giúp tránh các vấn đề phát sinh do các phần nhỏ không tương thích
    - **Áp dụng**:
        * Xem xét toàn bộ luồng công việc từ đầu đến cuối
        * Điều chỉnh quy trình làm việc dựa trên phản hồi từ toàn bộ hệ thống
    - **Ví dụ**: Một công ty có thể đầu tư vào hệ thống quản lý dự án, qua đó xác định nút thắt trong quy trình và từ đó cải thiện hiệu suất tổng thể

<a name="3-so-sanh-lean-va-agile"></a>
## 3. So sánh Lean và Agile
- **Lean**:
    * Tập trung vào tối ưu hóa quy trình, loại bỏ các hoạt động không tạo giá trị
    * Nhấn mạnh vào việc giảm thời gian, nguồn lực lãng phí và cải tiến liên tục
- **Agile**:
    * Tập trung vào linh hoạt thay đổi, giao tiếp và phản hồi từ khách hàng
    * Agile sử dụng các vòng lặp ngắn để phát triển phần mềm nhanh, sau đó nhận phản hồi và cải tiến
- **So sánh**:
    * Lean và Agile đều hướng tới cải tiến quy trình và tạo ra sản phẩm có giá trị
    * Agile chú trọng đến sự linh hoạt, điều chỉnh nhanh qua các vòng lặp ngắn
    * Lean chú trọng vào việc tối ưu quy trình, tránh lãnh phí

<a name="4-ung-dung-lean-trong-phan-mem"></a>
## 4. Ứng dụng Lean trong phần mềm
- **Phát triển MVP**: Áp dụng Lean để loại bỏ các tính năng cốt lõi, loại bỏ tính năng không cần thiết
- **Quy trình phát triển tối ưu**: Áp dụng các nguyên tắc của Lean để tái cấu trúc quy trình, giảm thời gian và chi phí phát triển
- **Liên tục cải tiến**: Thu thập số liệu và phản hồi từ khách hàng để cải tiến quy trình phát triển
- **Các dự án khởi nghiệp**: Lean giúp các Startup nhanh chóng ra mắt sản phẩm và nhận phản hồi để cải tiến dự án

<a name="5-cac-cong-cu-ho-tro-lean"></a>
## 5. Các công cụ hỗ trợ Lean
- **Kanban Board**: Sử dụng công cụ như Trello, Jira để theo dõi tiến độ công việc và xác định các bước bị tắc nghẽn
- **Value Stream Mapping**: Vẽ sơ đồ quá trình từ lúc nhận ý tưởng đến khi giao sản phẩm cho khác, để nhận diện các bước gây lãng phí
- **Metrics**: Theo dõi các thông số qua đó cải tiến hiệu suất
- **Công cụ giao tiếp và hợp tác**: Slack, Microsoft Teams giúp nhóm làm việc hiệu quả hơn

<a name="6-uu-nhuoc-diem-cua-lean"></a>
## 6. Ưu, nhược điểm của Lean

### Ưu điểm
- **Giảm lãng phí**: Loại bỏ những hoạt động không tạo ra giá trị &rarr; Giúp tiết kiệm thời gian và nguồn lực
- **Ra mắt sản phẩm nhanh**: Tập trung vào tính năng cốt lõi để ra mắt sản phẩm nhanh chóng
- **Cải tiến liên tục**: Luôn tìm cách cải tiến quy trình và sản phẩm
- **Tăng cường thích ứng**: Nhờ vào việc ra quyết định muộn, sản phẩm sẽ có khả năng thích ứng tốt hơn với nhu cầu thực tế

### Nhược điểm
- **Đòi hỏi hiểu biết sâu sắc**: Lean yêu cầu nhóm phải hiểu rõ quy trình và các bước để tối ưu quy trình
- **Khó đo lường**: Nếu không có thông tin rõ ràng, việc xác định các bước lãng phí có thể khó khăn
- **Không phù hợp với mọi loại dự án**: Lean không phù hợp với một số dự án đòi hỏi quy trình cứng nhắc hơn vì yêu cầu bảo mật, an toàn
