____GIT BASIC____
---------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------
**Lệnh kết nối Github với Git ( 2 lệnh ):**
<br>
*Thực hiện 2 lệnh sau đây trên Git Bash để kết nối Github-Git. Nếu chưa kết nối thì sẽ không thể tương tác từ Github<->Git được:*
1. **git config --global user.name "[your-username]"**
   <br>
   *Trong đó: your-username là username bạn đặt trong tài khoản github của bạn*
   <br>
   *Ví dụ: git config --global user.name "Hkzeuss"*
2. **git config --global user.email "[your-email]"**
   <br>
   *Trong đó: your-email là email bạn liên kết/đăng ký trong tài khoản github của bạn*
   <br>
   *Ví dụ: git config --global user.email "Hoangtientrungkien2k3@gmail.com"*
-----------------------------------------------------------------------------------   
  **Các bước đẩy code lên Github bằng Git:**
  <br>
1. **git add:** Sử dụng lệnh này để thêm các thay đổi từ thư mục làm việc của bạn vào sân khấu (staging area). Điều này chuẩn bị các thay đổi để được commit.<br>
	Syntax: **git add [tên-tệp-hoặc-thư-mục]**
2. **git commit:** Sử dụng lệnh này để commit các thay đổi đã được thêm vào sân khấu vào kho lưu trữ Git cục bộ của bạn. Trong quá trình commit, bạn sẽ phải cung cấp một thông điệp commit để mô tả mục đích của commit.<br>
	Syntax: **git commit -m "Thông điệp commit của bạn"**
3. **git push:** Sau khi bạn đã commit các thay đổi vào kho lưu trữ Git cục bộ, bạn có thể sử dụng lệnh này để đẩy các thay đổi lên kho lưu trữ từ xa, ví dụ như GitHub. Khi bạn thực hiện git push, bạn sẽ được yêu cầu đăng nhập vào tài khoản GitHub của bạn (nếu chưa đăng nhập) và sau đó các thay đổi sẽ được đẩy lên kho lưu trữ từ xa.<br>
	Syntax: **git push origin [tên-nhánh]**
-----------------------------------------------------------------------------------
**Muốn xóa Folder đã đẩy lên Github:**

**Gồm có 4 bước:**

1. **Chuyển đến thư mục mà chứa folder trên PC/LAPTOP <br>
   Syntax: cd /path/to/your/repository**

2. **git rm -r [my-folder]**

3. **git commit -m "Xóa thư mục my-folder"**

4. **git push origin [branch-name]**

---------------------------------------------------------------------------------------------------------------------------
**Lệnh lấy code từ Github về Laptop/Pc:**
 <br>
     git clone [link địa chỉ kho lưu trữ GitHub]
---------------------------------------------------------------------------------------------------------------------------     
**Tổng hợp lệnh Git** <br>
1. **git init**: Khởi tạo một kho lưu trữ Git mới trong thư mục làm việc hiện tại.
2. **git clone [địa chỉ kho lưu trữ]**: Sao chép một kho lưu trữ Git từ xa vào máy tính của bạn.

3. **git status**: Kiểm tra trạng thái hiện tại của kho lưu trữ Git và xem xét các thay đổi.

4. **git add [tên-tệp-hoặc-thư-mục]**: Thêm tệp hoặc thư mục vào sân khấu (staging area) để chuẩn bị cho việc commit.

5. **git commit -m "[thông điệp commit]"**: Commit các thay đổi đã thêm vào sân khấu với một thông điệp mô tả.

6. **git log**: Xem lịch sử commit của kho lưu trữ.

7. **git branch**: Xem danh sách các nhánh và biết bạn đang ở nhánh nào.

8. **git checkout [tên-nhánh]**: Chuyển đổi sang một nhánh khác hoặc tạo ra một nhánh mới.

9. **git merge [tên-nhánh]**: Kết hợp các thay đổi từ một nhánh vào nhánh hiện tại.

10. **git remote -v**: Xem danh sách các kho lưu trữ từ xa đã được kết nối với kho lưu trữ cục bộ của bạn.

11. **git fetch**: Lấy thông tin mới nhất từ kho lưu trữ từ xa, nhưng không thực hiện thay đổi trên làm việc của bạn.

12. **git pull**: Lấy thông tin mới nhất từ kho lưu trữ từ xa và thực hiện các thay đổi trên làm việc của bạn (tương đương với git fetch + git merge).

13. **git push [tên-từ-xa] [tên-nhánh]**: Đẩy các thay đổi từ kho lưu trữ cục bộ lên kho lưu trữ từ xa.

14. **git rm [tên-tệp]**: Loại bỏ một tệp khỏi kho lưu trữ Git và cũng khỏi thư mục làm việc.

15. **git reset [tên-tệp]**: Hủy bỏ việc thêm tệp vào sân khấu.

16. **git config --global user.name "[tên người dùng]"**: Cài đặt tên người dùng toàn cầu.

17. **git config --global user.email "[địa chỉ email]"**: Cài đặt địa chỉ email toàn cầu.

18. **git remote add [tên-từ-xa] [địa chỉ-kho-lưu-trữ]**: Thêm một kho lưu trữ từ xa vào danh sách kho lưu trữ từ xa.

19. **git stash**: Ẩn các thay đổi chưa commit để có thể làm việc trên nhánh khác.

20. **git cherry-pick [commit-hash]**: Chọn một commit cụ thể và áp dụng nó vào nhánh hiện tại.

21. **git rebase [tên-nhánh-khác]**: Đặt lại các commit trên một nhánh dựa trên commit của nhánh khác.

22. **git tag [tên-tag] [commit-hash]**: Tạo một tag trên một commit cụ thể.

23. **git blame [tên-tệp]**: Xem lịch sử thay đổi của từng dòng trong một tệp.

24. **git remote remove [tên-từ-xa]**: Loại bỏ một kho lưu trữ từ xa đã kết nối.
