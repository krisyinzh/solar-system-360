# 🚀 GitHub 上传指南

项目已准备好推送到GitHub！按照以下步骤操作：

## 第一步：在GitHub上创建新仓库
1. 访问 https://github.com/new
2. 输入仓库名称，例如：`solar-system-360`
3. 添加描述：`A realistic 360° Solar System visualization with Three.js`
4. 选择 Public（公开）
5. **不要** 初始化README、.gitignore或LICENSE（我们已经有文件了）
6. 点击 "Create repository"

## 第二步：获取你的仓库URL
创建仓库后，你会看到如下命令。复制 HTTPS 或 SSH URL。
例如：
- HTTPS: `https://github.com/YOUR_USERNAME/solar-system-360.git`
- SSH: `git@github.com:YOUR_USERNAME/solar-system-360.git`

## 第三步：在本地添加远程仓库并推送
在 PowerShell 中运行以下命令（将 URL 替换为你的）：

### 如果使用 HTTPS（推荐）：
```powershell
cd C:\Users\User\Desktop\cop
git remote add origin https://github.com/YOUR_USERNAME/solar-system-360.git
git branch -M main
git push -u origin main
```

### 如果使用 SSH：
```powershell
cd C:\Users\User\Desktop\cop
git remote add origin git@github.com:YOUR_USERNAME/solar-system-360.git
git branch -M main
git push -u origin main
```

## 第四步：完成！
- 上传完成后，访问 `https://github.com/YOUR_USERNAME/solar-system-360`
- 仓库就会出现在你的GitHub个人资料上

## 项目包含的文件
- ✅ `index.html` - 完整的太阳系360°可视化程序（包含所有Three.js代码）
- ✅ `README.md` - 项目说明文档

## 项目特性
- 🌌 40,000颗逼真的星星
- 🌍 8颗行星（太阳系内）+ 月球
- 💫 真实大小比例（以太阳为参照）
- 🎯 可点击行星查看信息
- 📍 实时行星标签
- 🎮 360°自由旋转和缩放
- ✨ PBR材质和高保真渲染
