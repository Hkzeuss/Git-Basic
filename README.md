## **1. Cấu hình Git**
### Thiết lập thông tin người dùng:
```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```
### Kiểm tra thông tin cấu hình:
```bash
git config --list
```
### Đổi trình soạn thảo mặc định:
```bash
git config --global core.editor "code --wait"  # VSCode
```

---

## **2. Khởi tạo & Clone Repository**
### Khởi tạo repository mới:
```bash
git init
```
### Clone repository từ GitHub:
```bash
git clone [repository-url]
```

---

## **3. Trạng thái & Lịch sử**
### Kiểm tra trạng thái làm việc:
```bash
git status
```
### Xem lịch sử commit:
```bash
git log
```
### Xem lịch sử commit theo dạng ngắn gọn:
```bash
git log --oneline
```

---

## **4. Thêm & Commit File**
### Thêm file vào staging area:
```bash
git add [file]
```
### Thêm tất cả file vào staging area:
```bash
git add .
```
### Commit thay đổi với mô tả:
```bash
git commit -m "Mô tả thay đổi"
```
### Commit với mô tả chi tiết:
```bash
git commit
```

---

## **5. Làm việc với Remote Repository**
### Liên kết repository từ xa:
```bash
git remote add origin [repository-url]
```
### Xem danh sách remote:
```bash
git remote -v
```
### Push code lên repository từ xa:
```bash
git push origin [branch-name]
```
### Pull code từ repository từ xa:
```bash
git pull origin [branch-name]
```
### Fetch thay đổi từ repository từ xa (không merge ngay):
```bash
git fetch
```

---

## **6. Làm việc với Branch**
### Xem danh sách branch:
```bash
git branch
```
### Tạo branch mới:
```bash
git branch [branch-name]
```
### Chuyển đổi branch:
```bash
git checkout [branch-name]
```
### Tạo và chuyển đổi sang branch mới:
```bash
git checkout -b [branch-name]
```
### Xóa branch:
```bash
git branch -d [branch-name]
```
### Merge branch vào branch hiện tại:
```bash
git merge [branch-name]
```

---

## **7. Reset & Undo**
### Hủy thay đổi chưa commit:
```bash
git checkout -- [file]
```
### Hủy toàn bộ thay đổi chưa commit:
```bash
git reset --hard
```
### Reset về commit trước:
```bash
git reset HEAD~1
```
### Revert một commit đã push:
```bash
git revert [commit-hash]
```

---

## **8. Stash (Lưu trữ tạm thời)**
### Lưu trữ thay đổi chưa commit:
```bash
git stash
```
### Xem danh sách stash:
```bash
git stash list
```
### Áp dụng lại stash gần nhất:
```bash
git stash apply
```
### Xóa stash sau khi áp dụng:
```bash
git stash drop
```
### Áp dụng và xóa stash cùng lúc:
```bash
git stash pop
```

---

## **9. Làm việc với Tag**
### Tạo tag:
```bash
git tag [tag-name]
```
### Xóa tag:
```bash
git tag -d [tag-name]
```
### Push tag lên repository từ xa:
```bash
git push origin [tag-name]
```

---

## **10. Cherry-pick & Rebase**
### Chọn một commit cụ thể và áp dụng vào branch hiện tại:
```bash
git cherry-pick [commit-hash]
```
### Rebase branch lên branch khác:
```bash
git rebase [branch-name]
```

---

## **11. Xóa file & Thư mục**
### Xóa file khỏi repository:
```bash
git rm [file]
```
### Xóa folder khỏi repository:
```bash
git rm -r [folder]
```
### Xóa file khỏi Git nhưng giữ lại trên local:
```bash
git rm --cached [file]
```

---

## **12. Quản lý Remote Repository**
### Xóa remote:
```bash
git remote remove [remote-name]
```
### Đổi tên remote:
```bash
git remote rename [old-name] [new-name]
```

---

## **13. Kiểm tra & Debug**
### Kiểm tra ai đã thay đổi một dòng code:
```bash
git blame [file]
```
### Kiểm tra khác biệt giữa hai commit:
```bash
git diff [commit1] [commit2]
```

---

## **14. Git Submodules**
### Thêm submodule vào project:
```bash
git submodule add [repository-url]
```
### Cập nhật submodule:
```bash
git submodule update --remote
```

---

## **15. Git Hooks (Tự động hóa quy trình Git)**
### Tạo pre-commit hook (chạy script trước khi commit):
```bash
touch .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```

---
