# AI 生成网页提示词模板

> 收集和整理用于 AI 生成网页的优质提示词

---

## 1. 基础框架提示词

### A. 作品集首页

```markdown
Create a portfolio website for a software engineer job seeker.

Requirements:
- Dark theme with subtle gradient accents (#0a0a0a background)
- Minimalist design - every element must have purpose
- Sections: Hero, Featured Works, About, Contact
- Color palette: #0a0a0a (bg), #ffffff (text), #3b82f6 (accent blue)
- Typography: Clean sans-serif (Inter or Geist)
- Include a "Download Resume" CTA button
- Responsive design for mobile

The vibe should be professional, confident, and understated.
```

### B. 产品发布页

```markdown
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

## 2. 进阶提示词

### A. 高级交互动画

```markdown
Enhance the portfolio with:
- Smooth scroll animations using Framer Motion
- Staggered fade-in for project cards
- Hover effects with subtle scale and glow
- Custom cursor following mouse
- Parallax scrolling for hero section
- Progress indicator on scroll
```

### B. 移动端优先

```markdown
Requirements:
- Mobile-first design approach
- Touch-friendly tap targets (min 44px)
- Swipe gestures for gallery
- Collapsible navigation menu
- Optimized images for mobile
- Lazy loading for performance
```

---

## 3. 场景化提示词

### A. 招聘网站风格

```markdown
Create a tech recruiter-friendly portfolio:
- Clean, scannable layout
- Clear value proposition in first 3 seconds
- Skills listed with proficiency levels
- Work experience in reverse chronological order
- Links to GitHub, LinkedIn, resume PDF
- Contact form or direct email
```

### B. 产品导向风格

```markdown
Create a product-focused portfolio:
- Featured project takes 70% of above-the-fold content
- Show, don't tell - use screenshots/videos
- Include metrics: users, downloads, engagement
- Link to live products or demos
- Product story: why, how, what happened
```

---

## 4. 最佳实践

### 提示词结构

```
1. 角色定义 (Role)
   "You are a senior frontend developer..."

2. 任务描述 (Task)
   "Create a portfolio website for..."

3. 具体要求 (Requirements)
   - Must have: [list]
   - Must avoid: [list]

4. 风格指导 (Style)
   - Tone: professional yet approachable
   - Vibe: confident, not arrogant

5. 技术约束 (Technical)
   - Framework: Astro/Next.js
   - Styling: Tailwind CSS
   - Animations: Framer Motion
```

### 迭代优化技巧

1. **先粗后细**: 先生成基本框架，再细化细节
2. **具体化**: 用具体颜色值、字号替代模糊描述
3. **提供参考**: 给出参考网站或风格
4. **分步骤**: 复杂页面分多次生成

---

## 5. 常用参考风格

| 风格 | 描述 | 适用场景 |
|------|------|----------|
| Stripe-like | 简洁、渐变、微动画 | 产品页 |
| Apple | 大量留白、大图、克制 | 品牌展示 |
| Linear | 深色、霓虹点缀、终端风 | 开发者 |
| Vercel | 黑色、白色文字、极速感 | 技术产品 |
| Brutalist | 原始、大胆、醒目 | 创意展示 |

---

## 6. 常用颜色方案

### 深色主题
```css
background: #0a0a0a
surface: #171717
border: #262626
text: #fafafa
text-muted: #a3a3a3
accent: #3b82f6 (blue)
```

### 浅色主题
```css
background: #ffffff
surface: #f5f5f5
border: #e5e5e5
text: #171717
text-muted: #737373
accent: #2563eb (blue)
```

### 渐变主题
```css
gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%)
```

---

## 7. 模板使用建议

1. **从简单开始**: 先用基础模板，验证效果后再加细节
2. **保持一致性**: 整个网站使用统一的设计系统
3. **内容优先**: 设计服务于内容，不要喧宾夺主
4. **性能考量**: 动画不要影响加载速度
5. **测试验证**: 在真实设备和浏览器上测试

---

## 8. Variant.com AI 设计工具

详细使用 Variant.com AI 设计工具生成网页的完整指南，详见 [variant-guide.md](variant-guide.md)

### Variant 快速提示词示例

```markdown
# 暗色优雅
Minimalist dark portfolio for software engineer,
hero with name and title, works grid, about section, contact,
#0a0a0a background, #3b82f6 accent, smooth animations

# 渐变流动
Dynamic gradient portfolio with glassmorphism cards,
animated background, hero with centered text,
project cards with hover effects, #667eea → #764ba2 gradient

# 终端风格
Developer portfolio in terminal aesthetic,
dark background (#0d1117), green accent (#39d353),
monospace font, command-line inspired UI
```

---

## 9. AI 前端工具全景指南

详细收录了 15+ 个最新 AI 和设计工具的完整指南，详见 [ai-design-tools-guide.md](ai-design-tools-guide.md)

### 工具分类速查

| 类别 | 工具 |
|------|------|
| AI 设计生成 | Framer, Dora AI, Google Stitch, Variant |
| UI 组件库 | shadcn/ui, React Bits |
| 动画交互 | Framer Motion, GSAP, Three.js |
| 设计灵感 | Mobbin, Dribbble, Awwwards |
| AI 编程 | Kimi, Cursor, v0 |

### 推荐工作流

```
Kimi (需求) → Figma (设计) → shadcn/ui (组件) 
→ Framer Motion (动画) → Vercel (部署)
```
