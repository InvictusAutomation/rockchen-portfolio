# Rock Chen 个人作品集网站方案

> 求职导向 - 高颜值静态网站完整指南

---

## 📋 目录

1. [工作流程建议](#1-工作流程建议)
2. [网站结构与定位](#2-网站结构与定位)
3. [个人特质打磨](#3-个人特质打磨)
4. [网站内容架构](#4-网站内容架构)
5. [代码资源与 Demo](#5-代码资源与-demo)
6. [交互逻辑说明](#6-交互逻辑说明)

---

## 1. 工作流程建议

### 第一阶段：规划与定位（1-2天）

```
Day 1: 需求梳理
├── 明确网站核心目标：求职展示
├── 确定风格方向：高级感、极简、克制
└── 梳理核心亮点：Voice Helper 产品

Day 2: 内容准备
├── 撰写产品文案（精炼、有力）
├── 准备素材：截图、视频、图标
└── 确定信息架构
```

### 第二阶段：技术选型与原型（2-3天）

```
技术栈选择：
├── Astro - 现代静态网站首选，性能极佳
├── Tailwind CSS - 快速样式开发
├── Framer Motion - 交互动画
└── TypeScript - 类型安全

备选方案：
├── Next.js + Tailwind
├── Vite + Vue/React
└── 纯 HTML + CSS + JS（最轻量）
```

### 第三阶段：开发与迭代（3-5天）

```
Day 1-2: 基础框架搭建
├── 项目初始化
├── 组件系统设计
└── 样式系统配置

Day 3-4: 核心页面开发
├── 首页作品展示
├── 产品详情页
└── 简历/关于页

Day 5: 细节打磨
├── 动画优化
├── 响应式检查
└── 性能优化
```

### 第四阶段：部署与测试（1-2天）

```
部署平台：
├── Vercel - 免费、CDN 加速
├── Netlify - 拖拽部署
└── GitHub Pages - 免费

测试检查：
├── 移动端适配
├── 加载速度
└── 无障碍访问
```

---

## 2. 网站结构与定位

### 🎯 核心定位

**一句话定位**：一个工程师的产品作品集网站，展示从 0 到 1 打造独立软件产品的能力。

**目标用户**：面试官、技术团队负责人

**核心诉求**：
1. 展示产品能力（Voice Helper）
2. 展示工程能力（代码、结构）
3. 展示产品思维（用户洞察、市场理解）
4. 展示审美品味（网站质感）

### 🏗️ 网站结构

```
┌─────────────────────────────────────────────┐
│  Navigation Bar                             │
│  [Logo] [作品] [产品] [关于] [简历]         │
└─────────────────────────────────────────────┘
│                                             │
│  HERO SECTION                               │
│  "我是一名工程师"                           │
│  "也是一名产品创作者"                        │
│  ↓ 向下滚动                                 │
│                                             │
├─────────────────────────────────────────────┤
│  WORKS GALLERY (首页核心)                   │
│  ┌─────────┐  ┌─────────┐                  │
│  │ Work 1  │  │ Work 2  │  ← 横向滑动     │
│  │VoiceHelper│ │ Project │                  │
│  └─────────┘  └─────────┘                  │
│                                             │
│  [View All Works →]                         │
│                                             │
├─────────────────────────────────────────────┤
│  VOICE HELPER (核心产品)                    │
│  ┌─────────────────────────────────────┐    │
│  │  Product Launch Page                │    │
│  │                                     │    │
│  │  [Download] [Watch Demo]            │    │
│  │                                     │    │
│  │  Features | Story | Research        │    │
│  └─────────────────────────────────────┘    │
│                                             │
├─────────────────────────────────────────────┤
│  ABOUT / RESUME                             │
│  技能树 | 经历 | 联系方式                    │
│                                             │
└─────────────────────────────────────────────┘
```

### 📍 重点抓准

| 层级 | 内容 | 目的 |
|------|------|------|
| 第一层 | 首页视觉冲击 | 3秒内吸引注意力 |
| 第二层 | 产品完整度 | 证明投入度和能力 |
| 第三层 | 过程展示 | 产品思维、调研能力 |
| 第四层 | 简历/联系 | 降低沟通成本 |

---

## 3. 个人特质打磨

### 💎 需要突出的核心特质

#### A. 产品思维
- **用户洞察**：为什么做这个产品？解决了什么问题？
- **市场理解**：目标用户是谁？市场空白在哪里？
- **迭代能力**：如何根据反馈改进？

#### B. 工程能力
- **架构设计**：技术选型、模块划分
- **问题解决**：遇到的最大挑战及解决方案
- **代码质量**：可维护性、性能优化

#### C. 审美品味
- **产品调性**：简洁、专业、有温度
- **细节较真**：每一像素都在乎

### 🔍 核心问题（自问清单）

在写文案前，先回答这些问题：

1. **为什么做 Voice Helper？**
   - 痛点是什么？亲身经历还是用户调研？
   - 市面上没有类似产品吗？差异化在哪里？

2. **产品取得了什么成绩？**
   - 用户数、下载量、留存
   - 用户评价、反馈
   - 媒体报道、社区讨论

3. **你在这个产品中扮演什么角色？**
   - 完全是个人项目还是团队？
   - 如果是团队，你的贡献是什么？

4. **最大的技术挑战是什么？**
   - 语音识别延迟？
   - 跨平台兼容性？
   - 如何解决的？

5. **如果重新做，会改变什么？**
   - 展示复盘能力和成长思维

### 🎯 亮点放置建议

| 位置 | 内容 | 形式 |
|------|------|------|
| Hero | 一句话产品定位 | 大字 + 动态效果 |
| 作品集卡片 | 产品截图 + 核心数据 | 悬停交互 |
| 产品页 | 完整故事线 | 时间轴 + 数据 |
| 关于页 | 技能树 + 经历 | 可视化 |

---

## 4. 网站内容架构

### 4.1 首页 (Home)

```markdown
## Hero Section
- 主标题：我叫 Rock Chen
- 副标题：一个把产品当作作品打磨的工程师
- CTA：向下滚动探索

## 作品集入口 (Featured Works)
- Voice Helper（核心产品，占最大篇幅）
- 其他项目（可选）

## 快速入口
- 查看简历
- 了解更多关于我
```

### 4.2 产品详情页 (Voice Helper)

```markdown
## 产品概览
- 产品名称 + 一句话描述
- 下载按钮 / 演示视频入口
- 核心数据（用户数、平台等）

## 功能特性
- 3-4 个核心功能点
- 每个功能配截图或动图

## 诞生过程（产品思维展示）
- 灵感来源
- 用户调研发现
- 产品迭代历程

## 技术实现（工程能力展示）
- 技术栈
- 架构亮点
- 遇到的技术挑战

## 用户反馈
- 用户评价
- 社区讨论

## 下载与联系
- 各平台下载链接
- 反馈渠道
```

### 4.3 关于/简历页 (About/Resume)

```markdown
## 个人简介
- 背景概述
- 技能标签

## 经历
- 教育背景
- 工作/实习经历
- 项目经验

## 技能栈
- 技术技能（编程语言、框架）
- 产品技能（工具、方法论）
- 设计技能（可选）

## 联系方式
- Email
- GitHub
- LinkedIn（可选）
```

### 4.4 文案原则

| 原则 | 说明 | 示例 |
|------|------|------|
| **少即是多** | 每个字都有价值 | "Voice Helper" > "一款优秀的语音助手软件" |
| **用数据说话** | 具体而非笼统 | "1000+ 用户" > "很多用户" |
| **展示过程** | 体现产品思维 | 不仅说"做了什么"，更说"为什么做" |
| **克制表达** | 不过度营销 | 事实 + 结果，让读者自己得出结论 |
| **真诚优先** | 宁可朴实不要浮夸 | 真实的故事最有力量 |

### 4.5 文案示例对比

❌ 过度营销：
> "Voice Helper 是史上最强语音助手，采用最先进的 AI 技术，帮助用户轻松完成各种任务，获得了广泛好评！"

✅ 克制有力：
> "Voice Helper，一款面向开发者的本地语音助手。完全开源，Mac/Windows 双平台支持，累计 1000+ 下载。"

---

## 5. 代码资源与 Demo

### 5.1 推荐技术栈

| 类别 | 推荐 | 特点 |
|------|------|------|
| 框架 | Astro | 性能极佳，适合静态网站 |
| 样式 | Tailwind CSS | 快速开发，一致性 |
| 动画 | Framer Motion | 强大易用，React 生态 |
| 部署 | Vercel | 免费，自动部署 |

### 5.2 高质量模板推荐

| 模板 | 特点 | 适用场景 |
|------|------|----------|
| [Astro Paper](https://github.com/satnaing/astro-paper) | 极简博客风 | 作品集、简历 |
| [Starlight](https://starlight.astro.build/) | 文档风 | 产品文档 |
| [Tailwind Creative](https://tailwind.build/) | 丰富组件 | 快速原型 |
| [Stripe Website](https://stripe.com) | 高级感 | 产品页参考 |

### 5.3 AI 生成网页工具

| 工具 | 特点 | 适用 |
|------|------|------|
| [v0.dev](https://v0.dev) | AI 生成 React 组件 | 快速原型 |
| [Galileo AI](https://galileo.ai) | AI 生成 UI | 设计参考 |
| [Locomotive Scroll](https://locomotivemtl.github.io/locomotive-scroll/) | 滚动动画 | 高级感 |
| [Scroll Reveal](https://scrollrevealjs.org/) | 滚动展示 | 动态效果 |

### 5.4 提示词技巧

#### 生成首页的优质提示词：

```
Create a high-end portfolio website for a software engineer seeking job opportunities.

Requirements:
1. Dark theme with subtle gradient accents
2. Minimalist design - every element must have purpose
3. Smooth scroll animations using Framer Motion
4. Sections: Hero, Featured Works, About, Contact
5. Color palette: #0a0a0a (bg), #ffffff (text), #3b82f6 (accent)
6. Typography: Clean sans-serif (Inter or Geist)
7. Include a "Download Resume" CTA button
8. Responsive design for mobile

The vibe should be professional, confident, and understated - like a senior engineer's portfolio.
```

#### 生成产品发布页的提示词：

```
Create a product launch page for "Voice Helper" - a local AI voice assistant for developers.

Sections needed:
1. Product hero with logo and one-line description
2. Download buttons (Mac/Windows)
3. Demo video placeholder
4. Key features (3-4 bullet points with icons)
5. "How it works" section with 3 steps
6. Technical stack used
7. User testimonials
8. Footer with links

Style: Clean, technical, professional. Dark theme preferred.
```

---

## 6. 交互逻辑说明

### 6.1 导航结构

```
┌────────────────────────────────────────────┐
│  Logo (Home)                              │
│  ─────────────────────                     │
│  [作品] → /works                          │
│  [产品] → /product (Voice Helper 详情)    │
│  [关于] → /about                          │
│  [简历] → /resume (PDF 下载)              │
└────────────────────────────────────────────┘
```

### 6.2 页面跳转关系

```
Home (/)
│
├── Hero Section
│   └── ↓ 滚动 → Works Section
│
├── Works Section
│   ├── [Voice Helper] → /product/voice-helper
│   └── [View All] → /works
│
├── Quick Links
│   ├── [简历] → /resume (或 PDF)
│   └── [关于] → /about
│
└── Footer
    ├── [GitHub] → github.com/rockchen
    └── [Email] → mailto:rockchen@xxx.com
```

### 6.3 信息组织

| 页面 | 信息内容 | 组织方式 |
|------|----------|----------|
| 首页 | 入口 + 精选作品 + 快速联系 | 垂直滚动 |
| 产品页 | 完整产品故事 + 技术细节 | 纵向深入 |
| 关于 | 个人经历 + 技能 | 卡片式布局 |
| 简历 | 教育 + 经历 + 技能 | 时间轴 + 列表 |

### 6.4 交互体验原则

1. **首屏 3 秒原则**：3 秒内传达核心价值
2. **滚动即叙事**：通过滚动引导用户阅读节奏
3. **点击即反馈**：所有交互都有视觉/触觉反馈
4. **克制动画**：动画服务于内容，不过度炫技
5. **移动优先**：先确保移动端体验，再优化桌面

---

## 📦 快速开始

### 推荐的起步方式

```bash
# 1. 使用 Astro 快速创建项目
npm create astro@latest rockchen-portfolio

# 2. 进入目录
cd rockchen-portfolio

# 3. 添加 Tailwind
npx astro add tailwind

# 4. 启动开发服务器
npm run dev

# 5. 部署到 Vercel（免费）
# 只需将项目推送到 GitHub，Vercel 会自动部署
```

---

## 📝 待完成事项

- [ ] 确定最终技术栈
- [ ] 准备 Voice Helper 素材（截图、视频）
- [ ] 撰写产品文案
- [ ] 选择并定制网站模板
- [ ] 开发核心页面
- [ ] 部署上线
- [ ] 测试与优化

---

> "The best portfolio is the one that gets you the job. Make it about the work, not about yourself."
