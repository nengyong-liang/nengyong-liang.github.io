# 🎓 个人主页 - 正经版

基于 [DevPortfolio](https://github.com/RyanFitzgerald/devportfolio) 模板构建的现代化个人主页。

## 🌟 特性

- ⚡ **极速加载** - Astro 静态生成，<50KB JS
- 📱 **完全响应式** - 适配所有设备
- 🎨 **现代设计** - 简洁专业的 UI
- 🔍 **SEO 优化** - 优秀的搜索引擎排名
- 🌙 **暗黑模式** - 内置主题切换
- 📊 **GitHub 同步** - 自动获取最新项目数据

## 🚀 本地开发

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build

# 预览生产构建
npm run preview
```

## 📝 配置说明

### 1. 基本信息配置

编辑 `src/config.ts`:

```typescript
export const siteConfig = {
  name: "nengyong liang",           // 你的姓名
  title: "Developer & Engineer",    // 职位/头衔
  description: "I'm Ultraman Tiga", // 个人简介
  accentColor: "#1d4ed8",          // 主题色
  
  social: {
    email: "your-email@example.com",
    linkedin: "https://linkedin.com/in/yourprofile",
    twitter: "https://twitter.com/yourhandle",
    github: "https://github.com/nengyong-liang",
    blog: "https://yourblog.com",
  },
  
  aboutMe: `你的详细个人简介...`,
  
  skills: [
    "JavaScript",
    "TypeScript",
    "Python",
    // 添加更多技能
  ],
  
  projects: [
    // 项目列表（可从 GitHub 自动获取）
  ],
  
  experience: [
    // 工作经历
  ],
  
  education: [
    // 教育背景
  ],
};
```

### 2. 更新 GitHub 数据

```bash
# 从项目根目录运行
node scripts/fetch-github-data.js
```

这将自动更新：
- 个人 Profile 信息
- GitHub 仓库列表
- 项目描述和技术栈

## 🎨 自定义样式

编辑 `src/styles/global.css`:

```css
/* 自定义全局样式 */
:root {
  --accent-color: #1d4ed8;
}

/* 添加你的自定义样式 */
```

## 📦 构建和部署

### 构建

```bash
npm run build
```

输出目录：`dist/`

### 部署到 GitHub Pages

项目已配置 GitHub Actions，推送到 `main` 分支后自动部署。

**手动部署**:

```bash
# 安装 gh-pages
npm install -D gh-pages

# 部署
npx gh-pages -d dist
```

## 📁 项目结构

```
portfolio-official/
├── src/
│   ├── components/          # Astro 组件
│   │   ├── Header.astro    # 页眉
│   │   ├── Hero.astro      # 英雄区
│   │   ├── About.astro     # 关于我
│   │   ├── Projects.astro  # 项目展示
│   │   ├── Experience.astro # 工作经历
│   │   ├── Education.astro # 教育背景
│   │   └── Footer.astro    # 页脚
│   ├── pages/
│   │   └── index.astro     # 主页
│   ├── styles/
│   │   └── global.css      # 全局样式
│   └── config.ts           # 配置文件
├── public/
│   └── favicon.svg         # 网站图标
├── astro.config.mjs        # Astro 配置
├── package.json
└── README.md
```

## 🔧 技术栈

- **框架**: Astro 5.x
- **样式**: Tailwind CSS 4.x
- **构建工具**: Vite
- **语言**: TypeScript

## 📊 性能指标

目标 Lighthouse 评分：

- Performance: 95+
- Accessibility: 95+
- Best Practices: 95+
- SEO: 95+

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 许可证

基于 [DevPortfolio](https://github.com/RyanFitzgerald/devportfolio) (MIT License)

---

**Made with ❤️ by nengyong-liang**
