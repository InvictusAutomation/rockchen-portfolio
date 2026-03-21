# 🤖 Context Hub (Chub) - AI 编程代理的知识库

> Andrew Ng 推出的 AI 编程代理上下文管理工具

---

## 什么是 Context Hub (Chub)？

**Context Hub** (现在叫 **Chub**) 是吴恩达 (Andrew Ng) 推出的一个开源项目，旨在解决 AI 编程代理的核心问题：

> **问题**: 编程代理在会话中会"幻觉"API、忘记学到的知识
> **解决方案**: 为代理提供精选的、有版本控制的文档，让它们能随着每次任务变得更聪明

---

## 核心价值

| 问题 | Context Hub 解决方案 |
|------|-------------------|
| AI 幻觉 API | 提供精选的、可靠的文档 |
| 搜索结果嘈杂 | 获取精准的、有针对性的文档 |
| 代码容易出错 | 代理可以添加注释记录问题 |
| 知识无法积累 | 注释跨会话持久化 |
| 重复犯同样的错 | 下次自动提醒 |

---

## 工作原理

### 基本流程

```
1. 搜索文档
   chub search "stripe payments"

2. 获取文档
   chub get stripe/api --lang js

3. 代理读取文档，写正确代码 ✅
```

### 自学机制

```
1. 发现问题 → 添加注释
   chub annotate stripe/api "需要 raw body 验证 webhook"

2. 下次获取 → 自动显示注释
   chub get stripe/api

3. 反馈给作者 → 文档持续改进
   chub feedback stripe/api up
```

---

## 安装和使用

### 安装

```bash
npm install -g @aisuite/chub
```

### 常用命令

| 命令 | 说明 |
|------|------|
| `chub search [query]` | 搜索文档和技能 |
| `chub get <id> [--lang py\|js]` | 获取指定文档 |
| `chub annotate <id> <note>` | 给文档添加注释 |
| `chub annotate --list` | 列出所有注释 |
| `chub feedback <id> up\|down` | 反馈文档质量 |

### 使用示例

```bash
# 搜索 OpenAI 文档
chub search openai

# 获取 Python 版 OpenAI 聊天文档
chub get openai/chat --lang py

# 获取 JavaScript 版
chub get openai/chat --lang js

# 搜索 Stripe 支付文档
chub search "stripe payments"

# 获取 Stripe API 文档
chub get stripe/api --lang js

# 添加注释（下次获取时自动显示）
chub annotate stripe/api "Webhook 验证需要 raw body"

# 反馈给作者
chub feedback stripe/api up
```

---

## 支持的文档类型

### API 文档 (版本化、语言特定)

```bash
# Python 版本
chub get openai/chat --lang py

# JavaScript 版本  
chub get openai/chat --lang js
```

### 更多内容类型 (规划中)

- Agent Skills (代理技能)
- 框架文档
- 库使用指南

---

## 自学代理机制

Context Hub 的核心创新：**让代理从每次经验中学习**

### 没有 Context Hub
```
❌ 搜索网络 → 嘈杂结果
❌ 代码出错 → 下次同样出错
❌ 知识遗忘 → 下次从头开始
```

### 有 Context Hub
```
✅ 获取精选文档 → 更高成功率
✅ 遇到问题 → 添加本地注释
✅ 自动记住 → 下次自动提醒
✅ 反馈给作者 → 文档越来越好
```

---

## 渐进式获取

文档可以有多个参考文件，代理可以只获取需要的部分：

```bash
# 只获取主入口
chub get openai/chat

# 获取特定参考文件
chub get openai/chat --file references

# 获取全部内容
chub get openai/chat --full
```

这避免了浪费宝贵的 token。

---

## 适用场景

### 1. 编程代理集成

将 Chub 集成到你的 AI 编程代理中：

- **Claude Code**: 创建 `~/.claude/skills/get-api-docs/` 目录，放入 SKILL.md
- **其他代理**: 使用 `chub` CLI 命令

### 2. API 文档管理

- 版本化管理
- 语言特定变体
- 社区贡献

### 3. 团队知识库

- 内部 API 文档
- 编码规范
- 最佳实践

---

## 技术栈

| 技术 | 说明 |
|------|------|
| **Node.js** | 运行时 |
| **Markdown** | 文档格式 |
| **YAML Frontmatter** | 元数据 |
| **MIT License** | 开源协议 |

---

## 相关项目

### aisuite

Chub 是 aisuite 生态系统的一部分：

- `@aisuite/chub` - Context Hub CLI
- 更多 AI 工具正在开发中

---

## 参考资源

- **GitHub**: [github.com/andrewyng/context-hub](https://github.com/andrewyng/context-hub)
- **npm**: [@aisuite/chub](https://www.npmjs.com/package/@aisuite/chub)
- **作者**: 吴恩达 (Andrew Ng)

---

## 总结

Context Hub (Chub) 解决了一个关键问题：**让 AI 编程代理从经验中学习**。

通过：
- 精选文档 → 减少幻觉
- 本地注释 → 知识积累  
- 反馈机制 → 持续改进

它让 AI 编程从"每次都重新开始"变成"越来越聪明"。

---

> 💡 **提示**: 如果你使用 Claude Code 或其他 AI 编程代理，建议配置 Chub 作为获取文档的首选方式，这样代理会自动获取准确、最新的 API 文档。
