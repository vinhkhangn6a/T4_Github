**TÌM HIỂU VỀ GITHUB**

**(TỔ 4)**

## Mục lục

A.Giới thiệu

*   *   Git là gì?
    *   Git được sử dụng để làm gì?
    *   Cách hoạt động của Git

B.GitHub

*   *   GitHub là gì?
    *   GitHub được sử dụng để làm gì?

C.Tích hợp Git và GitHub

D.Kết nối GitHub với VSCode

*   *   Push project lên GitHub
    *   Clone project về máy

E.Làm việc nhóm với GitHub

*   *   Khởi tạo dự án nhóm
    *   Thao tác branch
    *   Pull request và merge
    *   Khi nào nên dùng GitHub cho project nhóm

F.Markdown

# A.Giới thiệu

**GIT LÀ GÌ?**

Git là một hệ thống quản lý phiên bản phân tán (Distributed Version Control System _– DVCS_), nó là một trong những hệ thống quản lý phiên bản phân tán phổ biến nhất hiện nay. Git cung cấp cho mỗi lập trình viên kho lưu trữ (repository) riêng chứa toàn bộ lịch sử thay đổi.

**GIT ĐƯỢC SỬ DỤNG ĐỂ LÀM GÌ?**

**_Theo dõi sự thay đổi_**: Git cho phép bạn theo dõi tất cả các thay đổi trong mã nguồn, giúp bạn biết được ai đã thực hiện thay đổi gì và khi nào.

**_Phối hợp nhóm_**: Git cho phép nhiều lập trình viên làm việc trên cùng một dự án mà không lo sợ về việc xung đột mã nguồn.

**_Quản lý phiên bản_**: Git lưu trữ tất cả các phiên bản của mã nguồn, cho phép bạn dễ dàng quay lại phiên bản cũ nếu cần thiết.

**_Phân nhánh và gộp nhánh_**: Git cho phép tạo ra các nhánh để phát triển các tính năng mới, sửa lỗi, mà không ảnh hưởng đến nhánh chính (main branch). Khi hoàn thành, bạn có thể gộp (merge) nhánh đó vào nhánh chính.

**CÁCH HOẠT ĐỘNG CỦA GIT**

Có 3 phần chính của một dự án Git: Cây làm việc (the working tree) hay thư mục làm việc (the working directory), Vùng tổ chức (the staging area) và Thư mục Git (the Git directory). Quy trình làm việc của Git theo 3 phần chính như sau:

1.  Bạn sửa đổi các tập tin trong cây làm việc của mình.
2.  Bạn chọn lọc giai đoạn chỉ những thay đổi mà bạn muốn lưu trữ tiếp theo, điều này xác nhận rằng bạn chỉ thêm những thay đổi đó vào khu vực tổ chức.
3.  Bạn thực hiện một cam kết, thao tác này sẽ nhận các tệp như chúng nằm trong khu vực tổ chức và lưu trữ ảnh chụp nhanh đó vĩnh viễn vào thư mục Git của bạn.

Nếu một phiên bản cụ thể của tệp nằm trong thư mục Git thì nó được coi là đã cam kết (committed). Nếu nó đã được sửa đổi và được thêm vào khu vực tổ chức, nó sẽ được coi là đã tổ chức (staged). Và nếu nó đã được thay đổi kể từ khi được kiểm tra nhưng chưa được dàn dựng thì nó sẽ có trạng thái là đã được sửa đổi (modified).

# B.GITHUB

**GITHUB LÀ GÌ?**

GitHub là một nền tảng dựa trên web, chuyên cung cấp dịch vụ lưu trữ kho mã nguồn sử dụng hệ thống kiểm soát phiên bản Git. Nền tảng GitHub không chỉ là nơi lưu trữ code mà còn là một mạng xã hội lớn cho các lập trình viên trên toàn cầu. GitHub giúp các dự án phần mềm được quản lý minh bạch, cho phép nhiều người cùng đóng góp vào một cơ sở mã duy nhất.

**GITHUB ĐƯỢC SỬ DỤNG ĐỂ LÀM GÌ?**

**_1\. Lưu trữ mã nguồn online (cloud)_**

GitHub giúp bạn lưu code lên server thay vì chỉ để trong máy cá nhân → không sợ mất code, có thể truy cập từ bất cứ đâu.

 **_2. Làm việc nhóm / cộng tác_**

Nhiều người có thể cùng làm chung một dự án:

 • Mỗi người làm ở nhánh riêng (branch)

 • Tạo Pull Request để xin phép gộp code

 • Review code (xem xét, góp ý)

GitHub giúp điều phối teamwork cực hiệu quả.

 **_3. Theo dõi lịch sử thay đổi bằng Git_**

GitHub lưu toàn bộ phiên bản dự án:

 • Ai chỉnh sửa

 • Sửa lúc nào

 • Sửa cái gì

 • Có thể khôi phục phiên bản cũ

 **_4. Quản lý lỗi (Issues) và giao việc_**

Bạn có thể tạo:

 • Issue: báo lỗi hoặc yêu cầu tính năng

 • Projects/Boards: giống Trello để quản lý task

 **_5\. Open-source (mã nguồn mở)_**

GitHub là nền tảng của hầu hết dự án open source:

 • Ai cũng có thể xem code

 • Fork, đóng góp, sửa lỗi cho dự án lớn

Ví dụ: React, Node.js, Linux kernel… đều dùng GitHub.

 **_6. Deploy website / ứng dụng_**

GitHub Pages cho phép:

 • Host website miễn phí

 • Triển khai dự án tĩnh (HTML/CSS/JS)

 • Dùng để làm portfolio, blog…

 **_7. Lưu trữ tài liệu, file cấu hình, notebook_**

Không chỉ lưu code → GitHub còn lưu:

 • Tài liệu Markdown

 • Tài liệu hướng dẫn

 • Data, script, notes…

 **_8\. Tích hợp CI/CD (GitHub Actions)_**

Cho phép tự động:

 • Build code

 • Kiểm tra lỗi

 • Deploy

 • Gửi thông báo

→ Mỗi lần commit/push là tự chạy pipeline.

# C.CÁCH TÍCH HỢP GIT VÀ GITHUB

Sau khi cài đặt Git trên máy tính, người dùng mở cửa sổ dòng lệnh và khai báo tên cùng địa chỉ email để Git nhận diện tác giả trong các lần lưu phiên bản. Trên GitHub, tạo một kho lưu trữ (repository) mới để chứa mã nguồn. Tiếp đó, trong thư mục dự án trên máy, khởi tạo Git bằng lệnh git init, rồi đưa toàn bộ tệp vào hệ thống quản lý phiên bản bằng git add . và tạo bản ghi đầu tiên với git commit -m "first".

Khi kho lưu trữ trên GitHub đã sẵn sàng, liên kết dự án trong máy với kho trực tuyến thông qua lệnh git remote add origin <đường-dẫn-repo>. Sau đó, tải toàn bộ mã nguồn lên GitHub bằng git push -u origin main.

Từ thời điểm này, mỗi lần thay đổi mã nguồn, người dùng chỉ cần thêm các thay đổi vào Git, tạo thông điệp mô tả và đẩy lên GitHub bằng chuỗi lệnh git add ., git commit -m "ghi chú", và git push. Nếu muốn cập nhật mã từ GitHub về máy, có thể sử dụng lệnh git pull.

# D.CÁCH ĐỂ KẾT NỐI GITHUB VỚI VSCODE VÀ PUSH PROJECT LÊN VÀ LẤY PROJECT VỀ MÁY

**Hướng Dẫn push Code lên GitHub**

1.  **Tạo tài khoản Github và tải Vscode và Git**

lên trang chủ của Github và tạo tài khoảng Github , sau đó tải Vscode và Git về và kết nối tài khoản Github với Vscode theo các bước: Mở Vscode > vào view > Command Palette > Gõ “GitHub: Sign in” > Bấm Authorize

Link tải Git: [https://git-scm.com/install/](https://git-scm.com/install/)

Link tải Vscode :[https://code.visualstudio.com/download](https://code.visualstudio.com/download)

**2)Push code lên GitHub**

+Mở trang web GitHub lên chọn vào tài khoản đã đăng nhập vào phần Repositories và chọn New

+Tiếp theo là đặt tên cho Rep của bạn và có thể ghi thêm mô tả ở Description và copy link HTTPS

+Quay về màn hình desktop và click chuột phải và chọn “Open Git Bash here” sau đó gõ “git clone”

\+ link HTTPS đã copy trước đó bằng cách bấm chuột phải để “paste” , sau đó ấn phím “Enter” để tạo ra một folder .git

+Vào Vscode chọn File ở thanh trên cùng > chọn “Open Folder” > chọn vào folder git có tên mà bạn đã đặt cho Repositories.

+Khi đã chọn xong thì chúng ta tiến hành tạo thử một file code có đuôi là .cpp bằng cách click chuột phải chọn new file

+Sau đó vào phần “Source Control” hình 3 nhánh cây ở thanh bên tay trái sau đó “Commit”

+Cuối cùng là để ý thanh dưới góc trái màn hình và click vào 2 mũi tên xoay chiều để Push lên Github.Sau đó vào trang Github để kiểm tra.

**Hướng Dẫn Clone Code Từ GitHub Về Visual Studio Code Bằng Extension**

1\. Chuẩn bị

1.  **Visual Studio Code**: tải và cài đặt từ [https://code.visualstudio.com/](https://code.visualstudio.com/)
2.  **Git**: tải và cài đặt từ [https://git-scm.com/](https://git-scm.com/)
3.  **Tài khoản GitHub**: nếu muốn clone repository private.

2\. Cài Extension trong VS Code

1.  Mở VS Code → nhấn **Ctrl + Shift + X** hoặc chọn **Extensions**.  
    
2.  Tìm và cài **GitHub Pull Requests and Issues** hoặc **GitHub Repositories**.

Chỉ cần cài 1 trong 2 là đủ.

3\. Lấy link GitHub Repository

1.  Vào trang repository trên GitHub.
2.  Nhấn **Code → HTTPS → Copy link**.

4\. Clone Repository trong VS Code

1.  Nhấn **Ctrl + Shift + P  
    **
2.  Gõ **Git: Clone  
    **
3.  Dán link repository → Enter  
    
4.  Chọn thư mục lưu project

5\. Mở project

Sau khi clone xong → chọn **Open** để mở project.

# E.XÂY DỰNG - THAO TÁC REPOSITORY LÀM VIỆC NHÓM & KHI NÀO NÊN DÙNG GITHUB TẠO DỰ ÁN NHÓM

**I/ Khởi tạo dự án nhóm:**

1.  Chọn một repository muốn làm dự án nhóm.
2.  Thêm thành viên trong nhóm:
    1.  Vào repository, chọn “setting”:
3.  Chọn “Collaborators”:
4.  Chọn “Add people”:
5.  Nhập đúng tên account người người dùng (thành viên trong nhóm) rồi chọn “Add collaborator” - Thành viên được thêm sẽ phải check mail và accept để vào dự án.
6.  Thành viên Clone code từ Branch “main” trong dự án về và tạo Branch mới trước khi làm việc..
7.  Lưu ý: mỗi thành viên khi clone về đồng thời tạo một branch(nhánh) riêng biệt để không làm ảnh hưởng đến code main(chính), để tạo Branch sau khi Clone, ta cần:
    1.  Vào project vừa clone về bằng VScode (đã được kết nối với github).
    2.  Chọn biểu tượng như trong hình:
8.  Chọn biểu tượng “...” trên dòng “CHANGES”:
9.  Chọn “Branch” → “Create Branch From …”, sau đó sẽ hiện ra cửa sổ như hình, chọn branch chính trong repository nhóm của bạn (trong trường hợp ví dụ trong hình là “main”):
10.  Sau khi làm xong, chưa chắc sẽ gộp lại vào Branch main thì cứ Push lên bình thường bên Branch của mình, còn nếu muốn gộp với Branch chính thì:
    1.  Lên GitHub → Repository → tab Pull requests  
          
        
    2.  Bấm New pull request  
          
        
    3.  Chọn Branch của bạn → Create pull request  
          
        
    4.  Các thành viên khác sẽ:  
          
        1.  Review  
              
            
        2.  Comment  
              
            
        3.  Approve  
              
            
    5.  Khi hợp lệ → bấm Merge pull request

**II/ Khi nào nên dùng github làm project nhóm:**

1.  Dự án với số lượng thành viên lớn.
2.  Dự án có cấu trúc phức tạp, có nhiều File và các file chồng chéo lên nhau.
3.  Dự án nhiều giai đoạn, version và có nhu cầu lưu trữ code.
4.  Dự án cần thử nghiệm nhiều tính năng, có độ rủi ro cao, dễ lỗi.

# F.MARKDOWN

Markdown là một ngôn ngữ đánh dấu dạng **văn bản thuần (plain text)** được sử dụng để định dạng nội dung.  
Thay vì dùng thanh công cụ như trong Word, Markdown sử dụng các ký tự đặc biệt để tạo tiêu đề, in đậm, in nghiêng, bảng, danh sách,…

Markdown được dùng phổ biến trong:

*   GitHub / GitLab
*   File README.md của dự án lập trình
*   Notion
*   Visual Studio Code
*   Viết tài liệu kỹ thuật

Ví dụ so sánh Word và Markdown

| Chức năng | Word | Markdown |
| --- | --- | --- |
| In đậm | Ctrl + B | **nội dung** |
| In nghiêng | Ctrl + I | *nội dung* |
| Tiêu đề | Chọn Heading | # Tiêu đề |
| Danh sách | Insert Bullets | - mục 1 / - mục 2 |

Markdown dễ viết, gọn, nhẹ, hiển thị đẹp và đặc biệt phù hợp cho lập trình và lưu tài liệu online.

Có nhiều cách để chuyển đổi, tùy thiết bị và nhu cầu sử dụng.

**Cách 1: Chuyển trực tuyến (Online – dễ nhất)**

Một số trang web miễn phí hỗ trợ chuyển đổi:

*   Convertio.co
*   Cloudconvert.com
*   Pandoc.org/try

**Cách thực hiện:**

1.  Truy cập trang web
2.  Tải file .doc hoặc .docx lên
3.  Chọn định dạng đích: Markdown (.md)
4.  Tải file Markdown về máy

**Cách 2: Dùng Visual Studio Code**

Thích hợp nếu bạn dùng Markdown trên GitHub hoặc viết tài liệu.

**Thao tác:**

1.  Cài **Visual Studio Code**
2.  Cài extension **Docs to Markdown**
3.  Mở file Word bằng VS Code
4.  Nhấn chuột phải → **Convert to Markdown**
5.  Lưu file .md