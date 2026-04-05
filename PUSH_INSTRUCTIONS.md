# 🚀 HƯỚNG DẪN PUSH LÊN GITHUB

## ⚠️ LỖI PERMISSION

Bạn đang gặp lỗi permission vì:
- Repository: `duymoon7/AI-Shop`
- Tài khoản Git hiện tại: `thuonghoangdev`

## ✅ GIẢI PHÁP

### Cách 1: Đăng nhập đúng tài khoản (Khuyến nghị)

#### Windows:
1. Mở **Credential Manager**:
   - Nhấn `Win + R`
   - Gõ: `control /name Microsoft.CredentialManager`
   - Nhấn Enter

2. Chọn **Windows Credentials**

3. Tìm và xóa credentials GitHub cũ:
   - Tìm `git:https://github.com`
   - Click → Remove

4. Push lại:
   ```bash
   git push -u origin main
   ```

5. Nhập credentials của tài khoản `duymoon7`:
   - Username: `duymoon7`
   - Password: **Personal Access Token** (không phải password thường)

#### Tạo Personal Access Token:
1. Đăng nhập GitHub với tài khoản `duymoon7`
2. Vào: https://github.com/settings/tokens
3. Click **Generate new token** → **Generate new token (classic)**
4. Đặt tên: `AI-Shop`
5. Chọn quyền: `repo` (tất cả)
6. Click **Generate token**
7. **Copy token** (chỉ hiện 1 lần!)
8. Dùng token này làm password khi push

### Cách 2: Dùng SSH (Nâng cao)

```bash
# 1. Tạo SSH key
ssh-keygen -t ed25519 -C "duymoon7@email.com"

# 2. Copy public key
cat ~/.ssh/id_ed25519.pub

# 3. Thêm vào GitHub:
# Settings → SSH and GPG keys → New SSH key

# 4. Đổi remote sang SSH
git remote set-url origin git@github.com:duymoon7/AI-Shop.git

# 5. Push
git push -u origin main
```

### Cách 3: Dùng GitHub CLI

```bash
# 1. Cài đặt GitHub CLI
# Windows: winget install --id GitHub.cli

# 2. Đăng nhập
gh auth login

# 3. Chọn:
# - GitHub.com
# - HTTPS
# - Login with a web browser

# 4. Push
git push -u origin main
```

## 📝 LỆNH ĐÃ CHẠY

```bash
✅ git init                    # Đã có rồi
✅ git add -A                  # Đã add
✅ git commit -m "..."         # Đã commit
✅ git remote add origin ...   # Đã add remote
✅ git branch -M main          # Đã đổi branch
❌ git push -u origin main     # Lỗi permission
```

## 🔄 SAU KHI SỬA PERMISSION

Chỉ cần chạy:
```bash
git push -u origin main
```

## ✅ KIỂM TRA SAU KHI PUSH

1. Mở: https://github.com/duymoon7/AI-Shop
2. Kiểm tra:
   - ✅ Có tất cả files
   - ✅ Có README.md hiển thị đẹp
   - ✅ Có các file hướng dẫn
   - ✅ Commit history đầy đủ

## 📚 CÁC FILE QUAN TRỌNG ĐÃ PUSH

- ✅ GETTING_STARTED.md - Hướng dẫn nhanh
- ✅ HUONG_DAN_CAI_DAT.md - Hướng dẫn chi tiết
- ✅ CHECKLIST.md - Checklist cài đặt
- ✅ FILES_GUIDE.md - Hướng dẫn các file
- ✅ SUCCESS.md - Hướng dẫn sử dụng
- ✅ QUICK_REFERENCE.md - Tham khảo nhanh
- ✅ README.md - Tổng quan
- ✅ .gitignore - Loại trừ files
- ✅ docker-compose.yml - Docker config
- ✅ backend/ - Backend code
- ✅ frontend/ - Frontend code

## 🎯 SAU KHI PUSH THÀNH CÔNG

### Cập nhật README trên GitHub:
1. Vào repository: https://github.com/duymoon7/AI-Shop
2. Click vào README.md
3. Kiểm tra hiển thị đẹp
4. Thêm badges (optional):
   ```markdown
   ![Docker](https://img.shields.io/badge/Docker-Ready-blue)
   ![FastAPI](https://img.shields.io/badge/FastAPI-0.104-green)
   ![Next.js](https://img.shields.io/badge/Next.js-14-black)
   ```

### Thêm Topics:
1. Vào Settings → Topics
2. Thêm:
   - `ecommerce`
   - `fastapi`
   - `nextjs`
   - `docker`
   - `postgresql`
   - `typescript`
   - `python`

### Tạo Release (Optional):
1. Vào Releases → Create a new release
2. Tag: `v1.0.0`
3. Title: `Initial Release - E-Commerce Platform`
4. Description: Copy từ README.md

## 📞 NẾU VẪN GẶP LỖI

### Lỗi 403 Forbidden:
- Sai tài khoản GitHub
- Chưa có quyền truy cập repository
- Token hết hạn

### Lỗi 404 Not Found:
- Repository chưa tồn tại
- URL sai
- Repository là private nhưng chưa có quyền

### Giải pháp:
1. Kiểm tra repository tồn tại: https://github.com/duymoon7/AI-Shop
2. Kiểm tra quyền: Settings → Collaborators
3. Tạo token mới nếu cần
4. Xóa credentials cũ trong Credential Manager

## 🎉 HOÀN THÀNH

Sau khi push thành công:
1. ✅ Code đã lên GitHub
2. ✅ Người khác có thể clone về
3. ✅ Có đầy đủ hướng dẫn
4. ✅ Sẵn sàng để chia sẻ

**Chúc mừng! 🚀**
