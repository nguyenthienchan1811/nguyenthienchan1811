Git là một hệ thống quản lý phiên bản phân tán cực kỳ phổ biến (được tạo bởi Linus Torvalds). Khi học Git, bạn nên nắm vững các khái niệm cơ bản và một số lệnh thường dùng dưới đây.

---

# 🧠 1. Khái niệm cơ bản

* **Repository (repo)**: Kho lưu trữ mã nguồn
* **Commit**: Một lần lưu trạng thái code
* **Branch**: Nhánh phát triển riêng
* **Merge**: Gộp nhánh
* **Remote**: Repo trên server (ví dụ GitHub)

---

# ⚙️ 2. Cài đặt và cấu hình ban đầu

```bash
git config --global user.name "Tên của bạn"
git config --global user.email "email@example.com"
```

Kiểm tra:

```bash
git config --list
```

---

# 📁 3. Tạo và clone repository

### Tạo repo mới

```bash
git init
```

### Clone repo có sẵn

```bash
git clone <url>
```

---

# 📌 4. Các lệnh làm việc cơ bản

### Kiểm tra trạng thái

```bash
git status
```

### Thêm file vào staging

```bash
git add <file>
git add .   # thêm tất cả
```

### Commit thay đổi

```bash
git commit -m "Mô tả thay đổi"
```

### Xem lịch sử commit

```bash
git log
```

---

# 🌿 5. Làm việc với branch

### Tạo branch mới

```bash
git branch ten-branch
```

### Chuyển branch

```bash
git checkout ten-branch
```

(hoặc dùng gọn hơn)

```bash
git checkout -b ten-branch
```

### Xem danh sách branch

```bash
git branch
```

---

# 🔀 6. Merge (gộp nhánh)

```bash
git checkout main
git merge ten-branch
```

---

# ☁️ 7. Làm việc với remote (GitHub)

### Thêm remote

```bash
git remote add origin <url>
```

### Đẩy code lên

```bash
git push -u origin main
```

### Kéo code về

```bash
git pull
```

---

# 🔄 8. Một số lệnh hữu ích khác

### Xem sự khác biệt

```bash
git diff
```

### Hủy thay đổi file

```bash
git checkout -- <file>
```

### Xóa file khỏi staging

```bash
git reset <file>
```

---

# 🎯 9. Workflow cơ bản

1. `git clone` repo
2. Tạo branch mới
3. Code → `git add` → `git commit`
4. `git push`
5. Tạo Pull Request trên GitHub

---

# 🚀 Gợi ý học tiếp

* Học về **merge conflict**
* Sử dụng **rebase**
* Làm việc với **stash**
* Quy trình Git Flow
