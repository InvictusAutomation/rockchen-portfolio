# 📁 项目文件索引

## 目录结构

```
rockchen-portfolio/
├── README.md                    # 项目说明
├── docs/
│   └── PROJECT_PLAN.md         # 完整项目方案
├── demos/                      # 10 个网站 Demo
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

## 🎨 Demo 风格对比

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
