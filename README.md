This project is just a demo and practice how to use Git for coding

- Git được sử dụng để lưu lại  quá trình làm việc của 1 project
- Cách sử dụng:
Fist: Thuật ngữ
    + Working directory : Thư mục Project đang làm
    + Staging area : khu vực lưu trữ tạm thời các commit sau khi add
    + Git repository : Khu vực lưu trữ các commit đã đóng tem, gắn tên cho commit
Second: Câu lệnh
    + git init : Bất kỳ project nào cũng phải chạy git đầu tiên
    + git status : Giải thích trạng thái của các file trong project
    + git add : thêm các file mới tạo vào trong hệ thống kho của git
    + git commit : đóng cho file vừa add 1 cái tem để xác định, phân loại
        git commit -m '...' : gắn thêm mô tả, tên tem để dễ hiểu
    + git log : Show lịch sử commit
    + git show : Show sự thay đổi trong từng commit
        git show "mã commit"
    + git diff : xem thay đổi, trước khi add vào Staging area
X-> + "git checkout -- fileNAme" or "git restore fileName" : xóa thay đổi
        recommend "git restore" giống "undo", không dùng thường xuyên
    + "git reset [HEAD] fileName" or "git restore --staged fileName" : xóa file vừa add ra khỏi Staging area
        recommend "git reset fileName"