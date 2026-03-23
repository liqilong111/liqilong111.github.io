# 头像上传说明

## 如何添加您的头像

### 方法 1：直接上传到 GitHub（推荐）

1. 打开您的 GitHub 仓库：https://github.com/liqilong111/liqilong111.github.io
2. 点击 **images** 文件夹
3. 点击 **Add file** → **Upload files**
4. 将您的照片命名为 `profile.jpg` 并上传
5. 点击 **Commit changes**

### 方法 2：使用 Git 命令行

```bash
cd liqilong111.github.io
cp /path/to/your/photo.jpg images/profile.jpg
git add .
git commit -m "Add profile photo"
git push origin main
```

## 图片要求

- **格式**: JPG 或 PNG
- **文件名**: `profile.jpg` 或 `profile.png`
- **尺寸建议**: 正方形，至少 300x300 像素
- **文件大小**: 建议不超过 500KB

## 备选方案

如果您暂时不想上传照片，可以将以下代码改回使用默认图标：

在 `index.html` 中找到：
```html
<div class="profile-avatar">
    <img src="images/profile.jpg" alt="Dr. Qilong Li">
</div>
```

改为：
```html
<div class="profile-avatar" style="background: linear-gradient(135deg, var(--accent-color), var(--secondary-color)); display: flex; align-items: center; justify-content: center; font-size: 4rem; color: var(--white);">
    <i class="fas fa-user"></i>
</div>
```

## 更新后的网站

添加头像后，网站会自动显示在首页的个人卡片中。

访问：https://liqilong111.github.io
