# 快速部署到 GitHub Pages

## 方案一：我帮您推送（推荐，最快）

### 步骤 1：您在 GitHub 创建仓库（1分钟）

1. 打开 https://github.com/new
2. 仓库名称填写：`liqilong111.github.io`
3. 选择 **Public**（公开）
4. 勾选 **Add a README file**
5. 点击 **Create repository**

### 步骤 2：给我授权（30秒）

创建完成后，告诉我："仓库已创建"

我会立即将网站文件推送到您的仓库。

### 步骤 3：启用 GitHub Pages（1分钟）

1. 打开您的新仓库页面
2. 点击 **Settings** → **Pages**（左侧菜单）
3. Source 选择 **Deploy from a branch**
4. Branch 选择 **main**，文件夹选择 **/(root)**
5. 点击 **Save**

### 步骤 4：访问您的网站

等待 1-2 分钟后访问：
**https://liqilong111.github.io**

---

## 方案二：您自己上传（无需命令行）

### 步骤 1：创建仓库

同上，创建 `liqilong111.github.io` 仓库。

### 步骤 2：上传文件

1. 在仓库页面点击 **Add file** → **Upload files**
2. 将以下文件拖入上传区域：
   - `index.html`
   - `sitemap.xml`
   - `robots.txt`
3. 点击 **Commit changes**

### 步骤 3：启用 Pages

同上，在 Settings → Pages 中启用。

---

## 方案三：使用 Git 命令行

### 在您的电脑上执行：

```bash
# 1. 克隆仓库
git clone https://github.com/liqilong111/liqilong111.github.io.git
cd liqilong111.github.io

# 2. 复制网站文件到该目录（将文件复制过来）

# 3. 提交并推送
git add .
git commit -m "Initial website deployment"
git push origin main
```

---

## 部署完成后

### 设置自定义域名（可选）

如果您有域名（如 `www.liqilong.com`）：

1. 在仓库根目录创建 `CNAME` 文件
2. 文件内容：`www.liqilong.com`
3. 在域名服务商添加 CNAME 记录指向 `liqilong111.github.io`

### 提交到搜索引擎

1. **Google**: https://search.google.com/search-console
2. **Bing**: https://www.bing.com/webmasters

### 在学术平台添加链接

- Google Scholar 个人资料
- ResearchGate
- ORCID
- 学校官网

---

## 需要帮助？

选择 **方案一** 最简单！只需要您在 GitHub 创建仓库，剩下的我帮您完成。

请回复：**"使用方案一，仓库已创建"**，我会立即推送代码。
