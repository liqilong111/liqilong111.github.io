# 个人学术网站部署指南

## 网站预览

您的个人学术网站已创建完成！网站包含以下主要内容：

### 网站特点
- **专业设计**：现代化、响应式学术个人主页
- **多设备适配**：支持桌面、平板、手机访问
- **SEO优化**：包含完整的meta标签，便于搜索引擎收录
- **动画效果**：流畅的滚动和淡入动画

### 网站内容
1. **首页 (Hero)** - 个人简介和主要成就展示
2. **关于 (About)** - 研究背景和学术亮点
3. **研究方向 (Research)** - 三大研究领域卡片
4. **发表论文 (Publications)** - 代表性论文列表
5. **荣誉奖项 (Awards)** - 时间线式荣誉展示
6. **学术服务 (Service)** - 编辑职位和审稿服务
7. **联系方式 (Contact)** - 联系信息和招生信息

---

## 部署方法（二选一）

### 方法一：GitHub Pages 部署（推荐）

这是最常用的免费学术个人网站托管方式，其他人可以通过搜索引擎找到您。

#### 步骤 1：创建 GitHub 仓库

1. 访问 https://github.com
2. 登录您的账号（如果没有，请注册）
3. 点击右上角 "+" → "New repository"
4. 仓库名称填写：`您的用户名.github.io`
   - 例如：如果您的用户名是 `qilongli`，则填写 `qilongli.github.io`
5. 选择 "Public"（公开）
6. 点击 "Create repository"

#### 步骤 2：上传网站文件

**选项 A：使用 Git 命令行**

```bash
# 克隆仓库
git clone https://github.com/您的用户名/您的用户名.github.io.git
cd 您的用户名.github.io

# 复制网站文件到该目录
# 然后将文件添加到仓库
git add .
git commit -m "Initial website deployment"
git push origin main
```

**选项 B：使用 GitHub 网页上传**

1. 进入新创建的仓库页面
2. 点击 "Add file" → "Upload files"
3. 将 `personal-website.zip` 中的所有文件拖放到上传区域
4. 点击 "Commit changes"

#### 步骤 3：启用 GitHub Pages

1. 在仓库页面，点击 "Settings"（设置）
2. 左侧菜单选择 "Pages"
3. 在 "Source" 部分，选择 "Deploy from a branch"
4. Branch 选择 "main"，文件夹选择 "/ (root)"
5. 点击 "Save"

#### 步骤 4：访问您的网站

- 等待 1-2 分钟
- 访问：`https://您的用户名.github.io`
- 例如：`https://qilongli.github.io`

---

### 方法二：Cloudflare Pages 部署（更快速）

Cloudflare Pages 提供更快的全球访问速度。

#### 步骤 1：注册 Cloudflare

1. 访问 https://dash.cloudflare.com/sign-up
2. 使用邮箱注册账号

#### 步骤 2：创建 Pages 项目

1. 登录后，点击左侧 "Pages"
2. 点击 "Create a project"
3. 选择 "Upload assets"
4. 项目名称填写您的名字，例如：`qilong-li`
5. 上传 `personal-website` 文件夹中的所有文件
6. 点击 "Deploy site"

#### 步骤 3：自定义域名（可选）

1. 在 Pages 项目设置中
2. 点击 "Custom domains"
3. 添加您自己的域名

---

### 方法三：Netlify 部署（最简单）

Netlify 提供最简单的拖拽式部署。

#### 步骤：

1. 访问 https://www.netlify.com/
2. 注册/登录账号
3. 在仪表板点击 "Add new site" → "Deploy manually"
4. 将 `personal-website` 文件夹直接拖放到上传区域
5. 等待部署完成
6. 获得一个类似 `xxx-xxx-xxx.netlify.app` 的免费域名

---

## 如何让搜索引擎收录您的网站

### 1. 提交到 Google Search Console

1. 访问 https://search.google.com/search-console
2. 登录 Google 账号
3. 点击 "添加属性"
4. 输入您的网站 URL，例如：`https://qilongli.github.io`
5. 验证网站所有权（按照 Google 提供的验证方法）
6. 提交站点地图：在左侧菜单点击 "站点地图"，添加 `sitemap.xml`

### 2. 提交到 Bing Webmaster Tools

1. 访问 https://www.bing.com/webmasters
2. 登录 Microsoft 账号
3. 添加您的网站
4. 验证所有权
5. 提交站点地图

### 3. 在学术平台添加链接

- **Google Scholar**: 在个人资料中添加网站链接
- **ResearchGate**: 添加个人网站链接
- **ORCID**: 添加个人网站链接
- **LinkedIn**: 添加个人网站链接

### 4. 在其他网站添加链接

- 学校官网个人主页
- 学院网站
- 合作者的网站
- 学术会议个人介绍

---

## 更新网站内容

### 添加新论文

编辑 `index.html` 文件，在 Publications 部分添加：

```html
<div class="publication-item fade-in">
    <span class="pub-journal">期刊缩写</span>
    <h4 class="pub-title">论文标题</h4>
    <p class="pub-authors">
        <strong>Li Q*</strong>, et al.
    </p>
    <div class="pub-meta">
        <span><i class="fas fa-star"></i> IF: XX.X</span>
        <span><i class="fas fa-layer-group"></i> QX</span>
    </div>
</div>
```

### 添加新奖项

在 Awards 部分添加：

```html
<div class="award-item fade-in">
    <div class="award-content">
        <h4 class="award-title">奖项名称</h4>
        <p class="award-org">颁发机构</p>
    </div>
</div>
```

### 修改联系方式

在 Contact 部分修改邮箱、电话等信息。

---

## 自定义域名（可选）

如果您想使用自己的域名（例如 `www.liqilong.com`）：

### 购买域名

推荐平台：
- Namecheap: https://www.namecheap.com
- Google Domains: https://domains.google
- Cloudflare Registrar: https://www.cloudflare.com/products/registrar/

### GitHub Pages 配置自定义域名

1. 在仓库根目录创建 `CNAME` 文件
2. 文件内容为您的域名，例如：`www.liqilong.com`
3. 提交文件
4. 在域名提供商处添加 DNS 记录：
   - 类型：CNAME
   - 名称：www
   - 值：您的用户名.github.io

---

## 文件说明

| 文件 | 说明 |
|------|------|
| `index.html` | 主网页文件 |
| `.github/workflows/deploy.yml` | GitHub Actions 自动部署配置 |
| `README.md` | 项目说明文档 |
| `DEPLOYMENT_GUIDE.md` | 本部署指南 |

---

## 技术支持

如需帮助，请联系：
- 邮箱：liqilong@syau.edu.cn
- 办公室：沈阳农业大学动物科学与医学学院 515 室

---

## 网站预览效果

网站采用现代化设计：
- **配色方案**：深蓝色主色调，体现学术严谨性
- **字体**：Inter + Playfair Display，专业且易读
- **布局**：响应式网格布局，适配各种设备
- **动画**：平滑的滚动和淡入效果

祝您的学术事业蒸蒸日上！
