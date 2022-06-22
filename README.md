# This project is just a demo and practice how to use Git for coding

## Git được sử dụng để lưu lại  quá trình làm việc của 1 project
### Cách sử dụng:

#### Fist: Thuật ngữ
    - Working directory : Thư mục Project đang làm
    - Staging area : khu vực lưu trữ tạm thời các commit sau khi add
    - Git repository : Khu vực lưu trữ các commit đã đóng tem, gắn tên cho commit
    
#### Second: Câu lệnh
    - git init : Bất kỳ project nào cũng phải chạy git đầu tiên
    - git status : Giải thích trạng thái của các file trong project
    - git add : thêm các file mới tạo vào trong hệ thống kho của git
        "git add ." : add all
    - git commit : đóng cho file vừa add 1 cái tem để xác định, phân loại
      - git commit -m '...' : gắn thêm mô tả, tên tem để dễ hiểu
    
    - git log : Show lịch sử commit
    - git show : Show sự thay đổi trong từng commit
      - git show "commit ID"
    - git diff : xem thay đổi, trước khi add vào Staging area

    - "git checkout -- <file NAme>" or "git restore <file Name>" : xóa thay đổi
        > recommend "git restore" giống "undo", không dùng thường xuyên
    - "git reset [HEAD] <file Name>" or "git restore --staged <file Name>" : xóa file vừa add ra khỏi Staging area
        > recommend "git reset <file Name>"
        
    - "git reset --soft <commit ID>" : đưa commit được chỉ định và những commit sau đó về dạng staging area
    - "git reset --mixed <commit ID>" : đưa commit được chỉ định và những commit sau đó về dạng working directory
    - "git reset --hard <commit ID>" : xóa luôn commit được chỉ định và những commit sau đó
    - "git revert <commit ID>" : tạo 1 commit mới có nội dung là xóa những thay đổi của commit được chỉ định (bản chất là xóa commit được chỉ định)  
        
    - git checkout --b <branch Name> : Tạo nhánh mới (bản chất là một project demo chức năng mới nhằm mục đích làm và test chức năng mới của project), ok thì nhập vào nhánh chính.
    - git branch : kiểm tra các nhánh hiện có
    - git checkout <branch Name> : chuyển đổi giữa các branch
    - git merge : nhập nhánh bất kỳ vào nhánh hiện làm việc
        "git merge <branch Name>
        
#### Third: USE GITHUB (Đại loại là mạng xã hội cho coder)
    - git push : push all commit lên gitHub
      - > "git push origin <path>" : push lần đầu, 
           > lần sau chỉ cần "git push"
           > "git push origin <branch>" : push nhánh
    - git clone <project path>: Download 1 project nào đó về máy.
      - git pull : Sau khi download về máy thì pull (kéo về) / push (đẩy lển) tất cả commit bình thường
      - git fetch <branch Name> : để pull nhánh về
          > NOTE: - Khác nhau cơ bản giữa pull và fetch là: sau khi kéo 1 commit về thì pull sẽ merge các branch remote commit này với local commit, fetch thì không. 
                  -Nên chỉ nên dùng Pull khi muốn đồng bộ dữ liệu trên gitHub xuống local
        
        