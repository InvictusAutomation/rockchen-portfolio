# 📁 项目文件索引

## 目录结构

```
rockchen-portfolio/
├── README.md                    # 项目说明
├── docs/
│   └── PROJECT_PLAN.md         # 完整项目方案
├── demos/                      # 10 个初始网站 Demo
│   ├── 01-minimal-hero/        # 极简英雄区
│   ├── 02-interactive-gallery/ # 交互式画廊
│   ├── 03-product-launch/      # 产品发布页
│   ├── 04-dark-elegant/       # 暗色优雅
│   ├── 05-gradient-flow/      # 渐变流动
│   ├── 06-grid-masonry/       # 网格瀑布
│   ├── 07-video-hero/         # 视频背景
│   ├── 08-3d-transform/       # 3D 变换
│   ├── 09-typewriter/         # 打字机
│   └── 10-glassmorphism/      # 毛玻璃
├── demos-v2/                   # 10 个高水准设计方案 (推荐)
│   ├── 01-narrative-scroll/    # 叙事滚动 - 全屏叙事体验
│   ├── 02-bento-grid/          # 便当盒网格 - Apple 风格 Bento 布局
│   ├── 03-particle-canvas/     # 粒子画布 - Canvas 粒子网络交互
│   ├── 04-interaction-showcase/# 交互展陈 - 全交互响应式设计
│   ├── 05-research-journal/    # 研究手札 - 学术笔记本风格
│   ├── 06-noise-editorial/     # 噪点杂志 - 高级时尚杂志排版
│   ├── 07-zine-editorial/      # 独立杂志 - 独立 Zine 手工风格
│   ├── 08-bento-agency/        # Bento Agency - 顶奢创意代理风格
│   ├── 09-brutalist-diary/     # 先锋日记 - 新粗野主义设计
│   └── 10-experiential-voyage/# 体验航程 - 电影式沉浸叙事
├── prompts/                    # AI 生成提示词
│   └── ai-web-prompts.md      # 提示词模板
└── templates/                  # 备用模板
```

---

## 🚀 快速开始

### 本地预览 Demo

选择一个 Demo 目录，直接在浏览器中打开 `index.html`：

```bash
# 例如预览第一个 Demo
cd demos/01-minimal-hero
# 在浏览器中打开 index.html
```

### 使用 Ngrok 部署

```bash
# 安装 ngrok (如果未安装)
brew install ngrok  # macOS

# 启动简单 HTTP 服务器
python3 -m http.server 8000

# 另一个终端启动 ngrok
ngrok http 8000
```

---

## 📋 推荐工作流程

1. **预览所有 Demo**：找到最喜欢的风格
2. **确定技术栈**：推荐 Astro + Tailwind + Framer Motion
3. **准备内容**：产品截图、视频、文案
4. **定制开发**：基于选中风格定制
5. **部署上线**：Vercel 或 Netlify

---

## 🎨 Demo 风格对比 (demos/)

| # | 风格 | 特点 | 适用场景 |
|---|------|------|----------|
| 01 | 极简英雄区 | 大字标题、渐变背景、卡片悬浮 | 通用作品集 |
| 02 | 交互式画廊 | 自定义光标、3D卡片、鼠标跟随 | 创意展示 |
| 03 | 产品发布页 | 终端动画、功能展示、时间轴 | 产品详情 |
| 04 | 暗色优雅 | 大量留白、精致边框、克制配色 | 高级感 |
| 05 | 渐变流动 | 动态渐变、毛玻璃卡片 | 视觉冲击 |
| 06 | 网格瀑布 | 瀑布流布局、不规则卡片 | 作品多样 |
| 07 | 视频背景 | 视频背景、文字遮罩 | 沉浸感 |
| 08 | 3D 变换 | 3D 透视、悬停效果 | 技术感 |
| 09 | 打字机 | 终端风格、代码风格 | 开发者风 |
| 10 | 毛玻璃 | 磨砂玻璃、光晕效果 | 现代感 |

---

## 🔥 高水准设计方案 (demos-v2/ 推荐)

> 这些方案围绕 Voice Helper 语音助手项目设计，突出产品思维、AI 自主性与交互性研究、用户体验框架等核心内容。
> 每个方案都是完全不同的设计风格，均包含文本、多媒体和交互式内容的展示空间。

| # | 风格 | 设计语言 | 核心亮点 | 氛围 |
|---|------|----------|----------|------|
| 01 | 叙事滚动 | 暖色调 · Playfair Display | 全屏 scroll-snap、视差、逐行文字揭示、水平滚动子章节 | 电影感叙事 |
| 02 | 便当盒网格 | 暗色 · Apple Bento | 多尺寸卡片网格、旋转渐变边框、声波动画、悬停变形 | 科技精品 |
| 03 | 粒子画布 | 深空黑 · Canvas | 130 粒子网络、鼠标排斥、滚动变形态、麦克风轮廓聚散 | 赛博朋克 |
| 04 | 交互展陈 | 米白 · 强交互 | 磁性按钮、文字 scramble、3D 倾斜卡片、拖拽元素、涟漪效果 | 互动实验室 |
| 05 | 研究手札 | 牛皮纸 · 学术风 | 手写批注、便签、框架图、进度时间线、术语定义卡 | 研究者笔记 |
| 06 | 噪点杂志 | 黑白 · 时装杂志 | 非对称布局、超大字体、跑马灯、杂志跨页、噪点纹理 | 高级时装 |
| 07 | 独立杂志 | 拼贴 · Riso 印刷 | 手绘装饰、胶带相片、贴纸标签、宣言式排版、手绘分割线 | 独立书店 |
| 08 | Bento Agency | 黑金 · 创意代理 | 加载动画、打字机标题、水平拖拽滚动、电影画幅 Demo、金色奢华 | 奢华代理 |
| 09 | 先锋日记 | 粗野主义 · 像素 | 终端文件名、报错框、可展开卡片、源代码展示、可拖拽元素 | 黑客先锋 |
| 10 | 体验航程 | 渐变色温 · 沉浸 | 全视口场景、色彩温度渐变、星座概念图、声音波动画、电影质感 | 沉浸旅程 |

### 本地一键预览所有 V2 方案

```bash
cd rockchen-portfolio
python3 -m http.server 8000
# 浏览器打开 http://localhost:8000/demos-v2/
```

---

## 📦 技术栈推荐

### 核心框架
- **Astro** - 静态网站首选，性能极佳
- **Next.js** - 需要动态功能时

### 样式
- **Tailwind CSS** - 快速开发
- **CSS Modules** - 复杂样式

### 动画
- **Framer Motion** (React)
- **GSAP** - 高级动画
- **CSS Transitions** - 简单动画

### 部署
- **Vercel** - 免费、自动部署
- **Netlify** - 拖拽部署
- **GitHub Pages** - 免费

---

## 📝 下一步

1. 选择一个 Demo 作为起点
2. 根据 `docs/PROJECT_PLAN.md` 准备内容
3. 使用 `prompts/ai-web-prompts.md` 优化 AI 生成
4. 部署到 Vercel
5. 测试和优化

---

## 📧 联系

- Email: [your email]
- GitHub: [@rockchen]
- LinkedIn: [linkedin]

---

> Made with ❤️ for job seekers
