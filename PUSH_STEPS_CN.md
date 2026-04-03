# 📤 GitHub 推送步骤（详细指南）

你的本地项目已准备好！现在按照下面的步骤把它推送到 GitHub。

## 🎯 第一步：在 GitHub 创建新仓库

1. **访问 GitHub**
   - 打开浏览器访问 https://github.com
   - 登录你的 GitHub 账号（如果没有，先注册）

2. **创建新仓库**
   - 点击右上角 `+` 图标 → 选择 `New repository`
   - 或直接访问 https://github.com/new

3. **填写仓库信息**
   ```
   Repository name: solar-system-360
   Description: A realistic 360° Solar System visualization with Three.js
   Public: ✓ (选择公开)
   Initialize this repository with: 不勾选任何选项
   ```

4. **点击 "Create repository" 按钮**

---

## 🔐 第二步：获取你的 GitHub 仓库 URL

创建仓库后，你会看到一个页面，上面显示：

```
Quick setup — if you've done this kind of thing before
HTTPS | SSH | GitHub CLI
https://github.com/YOUR_USERNAME/solar-system-360.git
```

**复制这个 URL**（HTTPS 版本最简单）

---

## ⌨️ 第三步：在 PowerShell 中执行推送命令

打开 PowerShell，运行以下命令：

### 1️⃣ 添加远程仓库
```powershell
cd C:\Users\User\Desktop\cop
git remote add origin https://github.com/YOUR_USERNAME/solar-system-360.git
```

**⚠️ 注意**：将 `YOUR_USERNAME` 替换为你的 GitHub 用户名

### 2️⃣ 重命名分支为 main
```powershell
git branch -M main
```

### 3️⃣ 推送到 GitHub
```powershell
git push -u origin main
```

此时可能会要求输入 GitHub 凭证：
- **用户名**：输入你的 GitHub 用户名
- **密码**：输入你的 GitHub 密码或 Personal Access Token

---

## ✅ 第四步：验证上传成功

1. **在浏览器中打开**
   ```
   https://github.com/YOUR_USERNAME/solar-system-360
   ```

2. **你应该看到**
   - ✓ index.html 文件
   - ✓ README.md 文件
   - ✓ GITHUB_UPLOAD_GUIDE.md 文件
   - ✓ 完整的提交历史

---

## 🚀 可选：启用 GitHub Pages（在线演示）

如果想让别人直接在网页上玩你的太阳系项目：

1. 进入仓库页面
2. 点击 **Settings** → **Pages**
3. **Source** 选择 `Deploy from a branch`
4. **Branch** 选择 `main` 和 `/ (root)`
5. 点击 **Save**

几分钟后，你会看到你的项目在线地址：
```
https://YOUR_USERNAME.github.io/solar-system-360/
```

---

## 🐛 常见问题解决

### ❌ 错误："fatal: remote origin already exists"
```powershell
git remote remove origin
git remote add origin https://github.com/YOUR_USERNAME/solar-system-360.git
```

### ❌ 错误："Please tell me who you are" 
```powershell
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### ❌ 认证失败
- 使用 **Personal Access Token** 代替密码
- 在 GitHub 设置中生成：Settings → Developer settings → Personal access tokens

### ❌ "Permission denied (publickey)"（如果用 SSH）
- 改用 HTTPS 方式
- 或配置 SSH 密钥

---

## 💡 后续操作

推送成功后，你可以：

1. **与朋友分享**
   ```
   https://github.com/YOUR_USERNAME/solar-system-360
   ```

2. **启用 Pages 后分享演示链接**
   ```
   https://YOUR_USERNAME.github.io/solar-system-360/
   ```

3. **继续开发**
   - 修改文件后：`git add .`
   - 提交更改：`git commit -m "描述你的修改"`
   - 推送到GitHub：`git push`

4. **添加更多功能**
   - 更多行星卫星
   - 行星轨道编辑器
   - 性能优化
   - 移动端适配

---

## 📞 需要帮助？

- 访问 [GitHub 文档](https://docs.github.com)
- 查看 [Pro Git 书籍](https://git-scm.com/book/zh/v2)
- 在 [Stack Overflow](https://stackoverflow.com) 搜索问题

---

**祝贺！你的太阳系项目即将在 GitHub 上线！🎉**
