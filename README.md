# user-manual
1. git init: tạo nơi lưu lại lịch sử thư mục

2. git status: theo dõi những thứ đc viết mới vào và thông báo màu đỏ (thêm vào nhưng chưa đc check)

3. git add: check những thứ thêm vào (thông báo chuyển màu xanh)

4. git commit: đóng gói những thay đổi vào dán 1 cái tem (git commit -m '...')

5. git log: xem lại lịch sử đã commit những gì

6. git show: hiện ra toàn bộ những thay đổi trong một hộp có nhãn commit

7. git diff: xem thay đổi của những file modifile

8. git checkout: xóa thay đổi của một file khi chưa đc add

9. git restore: xóa file khoỉ staging area sau khi file đc add(xanh)

10. git reset --soft: để uncommmit, file đc quay lại ở staging area
    git reset --mixed: để uncommit + unadd, file đc quay lại ở working directory, chưa đc chay git add
    git reset --hard: để unall, file quay lại như chưa đc làm gì

11. git revert: xóa thay đôỉ trong code của file ngay cả khi đã đc add, có tác dụng với commit gần nhất

12. .gitignore: file đc sửa nhưng mà k muốn hiện lên khi có lệnh git status


============================= 


11. working directory: chứa những file trong phần code như Mouse, Cat

12. staging area: những file đc chạy git add thì sẽ có trong staging area (là file xanh sau git add), chỉ những file đc add vào staging area mới đc commit(đc chạy lệnh git commit)

13. git repository: lưu những thay đổi của 1 commit



==============================


Github

===push

b0: git ssh (public key)

b1: git remote add origin 'link'

b2: git add .

b3: git commit -m '...'

b4: git push origin master

====pull

1. git clone: tải code về máy

2. git pull: dung khi bên A thay đổi, bên B sẽ tải cái thay đổi đó mà k phải tải lại hết code


===============================

- git branch -D 'ten branch': xóa branch
- git checkout master: chuyển về branch master

Dùng github nhóm

1. git branch: git checkout -b feature/horse: tạo branch mới

2. git push origin feature/horse: đẩy branch lên git

3. pull request: comment trên github để ghép code từ branch khác vào branch master(branch chính)

Tham khảo thêm: 
https://viblo.asia/p/tim-hieu-mot-so-khai-niem-va-ki-thuat-thuong-dung-trong-git-phan-1-naQZR4pP5vx

https://viblo.asia/p/tim-hieu-mot-so-khai-niem-va-ki-thuat-thuong-dung-trong-git-phan-2-Az45b9BOlxY

https://rogerdudler.github.io/git-guide/index.vi.html

https://stackoverflow.com/questions/26042390/git-add-asterisk-vs-git-add-period
