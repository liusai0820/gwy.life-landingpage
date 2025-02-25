# GWY.LIFE 落地页

这是 gwy.life 的主域名落地页项目，提供导航到各个子域名应用的链接。

## 项目特点

- 纯静态HTML/CSS实现，无需任何框架依赖
- 响应式设计，适配各种设备尺寸
- 轻量级，加载速度快
- 美观现代的UI设计

## 部署指南

### 步骤1：克隆仓库

```bash
git clone https://github.com/your-username/gwy-landing-page.git
cd gwy-landing-page
```

### 步骤2：在Vercel上部署

可以通过以下方式部署到Vercel：

1. 使用GitHub集成直接部署
2. 使用Vercel CLI命令行工具部署：

```bash
npm install -g vercel
vercel login
vercel
```

### 步骤3：域名配置

在Vercel控制台中：

1. 添加自定义域名 `gwy.life`
2. 按照提示更新DNS记录
3. 等待DNS生效

## 更新子域名应用

在 `index.html` 文件中修改应用卡片：

```html
<a href="https://your-app.gwy.life" class="app-card" target="_blank" rel="noopener noreferrer">
  <div class="p-6 flex-1">
    <div class="icon-container">
      <img src="./public/icons/your-icon.svg" alt="应用名称" width="32" height="32">
    </div>
    <h2 class="text-xl font-semibold text-gray-800 mb-2">应用名称</h2>
    <p class="text-gray-600">应用描述</p>
  </div>
  <div class="card-footer">
    访问应用
  </div>
</a>
```

## 本地开发

可以使用任何静态服务器本地开发：

```bash
# 使用 Python 的简易HTTP服务器
python -m http.server

# 或使用 Node.js 的 http-server
npx http-server
```

访问 http://localhost:8000 预览网站。 