# ⚡ Hướng Dẫn Nhanh - Git Commit Lên GitHub

## 🚀 Cách nhanh nhất (3 bước)

### Bước 1: Stage file
```bash
git add .
```

### Bước 2: Commit
```bash
git commit -m "feat: mô tả thay đổi"
```

### Bước 3: Push
```bash
git push origin main
```

---

## 📝 Ví dụ cụ thể cho file hiện tại

Bạn đang có 3 file chưa commit:
- `.gitignore` (mới)
- `GIT_GUIDE.md` (mới)  
- `Database/initdb.d/QLTV.NGUOIDUNG.json` (đã sửa)

### Cách 1: Commit tất cả cùng lúc
```bash
git add .
git commit -m "docs: thêm .gitignore, hướng dẫn git và cập nhật database"
git push origin main
```

### Cách 2: Commit riêng từng loại
```bash
# Commit tài liệu
git add .gitignore GIT_GUIDE.md
git commit -m "docs: thêm .gitignore và hướng dẫn git commit"
git push origin main

# Commit database
git add Database/initdb.d/QLTV.NGUOIDUNG.json
git commit -m "chore(database): cập nhật dữ liệu người dùng mẫu"
git push origin main
```

---

## 🎯 Các loại commit message phổ biến

| Loại | Ví dụ | Khi nào dùng |
|------|-------|--------------|
| `feat` | `feat(backend): thêm API đăng nhập` | Thêm tính năng mới |
| `fix` | `fix(frontend): sửa lỗi validation` | Sửa lỗi |
| `docs` | `docs: cập nhật README` | Cập nhật tài liệu |
| `chore` | `chore(database): thêm dữ liệu mẫu` | Cập nhật config, data |
| `refactor` | `refactor(backend): tách routes` | Refactor code |
| `style` | `style: format code` | Format code |

---

## 🔄 Quy trình làm việc hàng ngày

### Khi bắt đầu:
```bash
git pull origin main
```

### Khi hoàn thành tính năng:
```bash
git add .
git commit -m "feat(scope): mô tả tính năng"
git push origin main
```

---

## ⚠️ Lỗi thường gặp

### "Updates were rejected"
```bash
git pull origin main
git push origin main
```

### "Authentication failed"
- Sử dụng Personal Access Token thay vì password
- Hoặc cấu hình SSH key

---

## 📚 Xem thêm

- Chi tiết đầy đủ: `GIT_GUIDE.md`
- Hướng dẫn GitHub: `GITHUB_COMMIT_GUIDE.md`
- Script tự động: `commit-and-push.ps1`

---

**💡 Tip**: Luôn commit message rõ ràng để dễ theo dõi tiến độ!

