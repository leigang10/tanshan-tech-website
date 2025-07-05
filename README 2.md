# 北京探山科技有限公司官网部署指南

## 📋 项目概述

这是一个为北京探山科技有限公司开发的静态展示网站，包含以下功能：

- ✅ 响应式设计（支持手机、平板、电脑）
- ✅ 四个主要页面（首页、关于我们、服务产品、联系我们）
- ✅ 现代美观的界面设计
- ✅ 移动端友好的导航菜单
- ✅ 联系表单功能
- ✅ FAQ常见问题解答
- ✅ SEO优化

## 🚀 快速部署到 GitHub Pages

### 方法一：使用 GitHub Desktop（推荐新手）

#### 步骤 1：注册 GitHub 账号
1. 访问 [GitHub.com](https://github.com)
2. 点击右上角 "Sign up" 注册账号
3. 验证邮箱地址

#### 步骤 2：下载并安装 GitHub Desktop
1. 访问 [desktop.github.com](https://desktop.github.com)
2. 下载并安装 GitHub Desktop
3. 使用 GitHub 账号登录

#### 步骤 3：创建仓库并上传代码
1. 打开 GitHub Desktop
2. 点击 "File" → "New Repository"
3. 填写仓库信息：
   - **Name**: `tanshan-tech-website` （或您喜欢的名称）
   - **Description**: 北京探山科技有限公司官网
   - **Local path**: 选择您的项目文件夹位置
   - 勾选 "Initialize this repository with a README"
4. 点击 "Create Repository"

#### 步骤 4：上传网站文件
1. **复制文件到仓库文件夹**：
   - 打开您的项目文件夹（MYAPP文件夹）
   - 选择所有文件和文件夹（Ctrl+A 或 Cmd+A）
   - 复制（Ctrl+C 或 Cmd+C）
   - 打开GitHub Desktop创建的仓库文件夹
   - 粘贴（Ctrl+V 或 Cmd+V）所有文件

   **具体需要复制的文件**：
   ```
   index.html
   about.html
   services.html
   contact.html
   css/style.css
   js/script.js
   images/README.md
   README.md
   ```

2. **验证文件复制**：
   - 确保仓库文件夹中包含以下结构：
   ```
   仓库文件夹/
   ├── index.html
   ├── about.html
   ├── services.html
   ├── contact.html
   ├── css/
   │   └── style.css
   ├── js/
   │   └── script.js
   ├── images/
   │   └── README.md
   └── README.md
   ```

3. **在GitHub Desktop中提交**：
   - 回到GitHub Desktop，您会看到所有文件被列为 "Changes"
   - 在底部填写提交信息：
     - **Summary**: "Initial website upload"
     - **Description**: "上传探山科技官网文件"
   - 点击 "Commit to main"
   - 点击 "Push origin" 上传到GitHub

**替代方法（如果上述方法不工作）**：
- 在GitHub Desktop中，点击 "Repository" → "Show in Finder"（Mac）或 "Show in Explorer"（Windows）
- 这会直接打开仓库文件夹
- 将您的项目文件直接拖拽到这个文件夹中
- 回到GitHub Desktop，文件会自动显示在 "Changes" 中

**常见问题解决**：
- **如果看不到文件变化**：在GitHub Desktop中点击 "Fetch origin" 刷新
- **如果文件结构错误**：确保文件夹结构正确，不要嵌套多层文件夹
- **如果复制失败**：尝试一个一个文件复制，或者使用拖拽方式

#### 步骤 5：启用 GitHub Pages
1. 在 GitHub Desktop 中点击 "Repository" → "View on GitHub"
2. 在 GitHub 网页中，点击 "Settings" 标签
3. 在左侧菜单中找到 "Pages"
4. 在 "Source" 部分，选择 "Deploy from a branch"
5. 在 "Branch" 下拉菜单中选择 "main"，文件夹选择 "/ (root)"
6. 点击 "Save"
7. 等待几分钟，GitHub 会显示您的网站地址

### 方法二：使用 Vercel（更简单）

#### 步骤 1：注册 Vercel 账号
1. 访问 [vercel.com](https://vercel.com)
2. 点击 "Sign Up" 注册账号
3. 选择 "Continue with GitHub" 使用 GitHub 账号登录

#### 步骤 2：上传项目
1. 登录后点击 "New Project"
2. 选择 "Upload" 选项
3. 将整个项目文件夹拖拽到上传区域
4. 点击 "Deploy"

#### 步骤 3：获取网站地址
1. 部署完成后，Vercel 会自动生成一个网址
2. 您可以在项目设置中自定义域名

## 🔧 自定义域名设置

### GitHub Pages 自定义域名
1. 在 GitHub 仓库的 "Settings" → "Pages" 中
2. 在 "Custom domain" 输入框中输入您的域名（如：www.tanshan.com.cn）
3. 点击 "Save"
4. 在您的域名提供商处添加 CNAME 记录：
   - **类型**: CNAME
   - **名称**: www
   - **值**: `您的GitHub用户名.github.io`

### Vercel 自定义域名
1. 在 Vercel 项目设置中点击 "Domains"
2. 添加您的域名
3. 按照 Vercel 提供的 DNS 记录配置您的域名

## 📝 内容修改指南

### 修改文字内容
所有文字内容都在 HTML 文件中，您可以直接编辑：

#### 公司信息修改
- **文件**: `index.html`, `about.html`, `contact.html`
- **位置**: 查找包含公司名称、联系方式等信息的标签
- **示例**: 
  ```html
  <!-- 修改公司名称 -->
  <h1>北京探山科技有限公司</h1>
  
  <!-- 修改联系方式 -->
  <p>(+86) 15011531282</p>
  <p>lingfei@tanshan.com.cn</p>
  ```

#### 服务内容修改
- **文件**: `services.html`
- **位置**: 查找服务描述、特点等文字内容
- **示例**:
  ```html
  <!-- 修改服务描述 -->
  <p>我们提供全面的医药不良反应数据分析和评估服务...</p>
  ```

### 替换图片
1. 准备您的图片文件
2. 将图片放入 `images` 文件夹
3. 按照 `images/README.md` 中的说明重命名文件
4. 刷新网页查看效果

### 修改颜色主题
- **文件**: `css/style.css`
- **主要颜色变量**:
  ```css
  /* 主色调 */
  #3498db  /* 蓝色 */
  #2c3e50  /* 深灰色 */
  #667eea  /* 渐变蓝色 */
  #764ba2  /* 渐变紫色 */
  ```

## 📱 移动端测试

### 本地测试
1. 在浏览器中打开网站
2. 按 F12 打开开发者工具
3. 点击设备模拟器图标（手机/平板图标）
4. 选择不同的设备尺寸进行测试

### 真机测试
1. 部署网站后，在手机浏览器中访问网站地址
2. 测试导航菜单、表单提交等功能
3. 检查在不同屏幕尺寸下的显示效果

## 🔍 SEO 优化

网站已包含基本的 SEO 优化：

### 页面标题和描述
每个页面都有独特的标题和描述：
```html
<title>页面标题 - 北京探山科技有限公司</title>
<meta name="description" content="页面描述内容">
```

### 语义化标签
使用了正确的 HTML5 语义化标签：
- `<header>` - 页头
- `<nav>` - 导航
- `<main>` - 主要内容
- `<section>` - 区块
- `<footer>` - 页脚

### 图片优化
- 所有图片都有 `alt` 属性
- 使用适当的图片格式和大小

## 🛠️ 技术栈说明

- **HTML5**: 页面结构
- **CSS3**: 样式设计，包含 Flexbox 和 Grid 布局
- **JavaScript**: 交互功能
- **Font Awesome**: 图标库
- **响应式设计**: 适配各种设备

## 📞 技术支持

如果您在部署过程中遇到问题：

1. **检查文件结构**: 确保所有文件都在正确的位置
2. **查看浏览器控制台**: 按 F12 查看是否有错误信息
3. **验证 HTML**: 使用在线 HTML 验证工具检查语法
4. **联系技术支持**: 如有技术问题，请联系开发团队

## 🎯 成功标准

部署完成后，您应该能够：

- ✅ 在浏览器中正常访问网站
- ✅ 在手机和电脑上都能正常显示
- ✅ 导航菜单正常工作
- ✅ 联系表单可以提交
- ✅ 所有页面都能正常跳转
- ✅ 图片正常显示

## 📈 后续维护

### 定期更新
- 及时更新公司信息
- 添加新的服务内容
- 更新团队介绍
- 优化网站性能

### 备份建议
- 定期备份网站文件
- 保存重要的修改记录
- 考虑使用版本控制工具

---

**恭喜！** 您的公司官网已经成功部署。如果您需要进一步的定制或功能增强，请随时联系开发团队。 