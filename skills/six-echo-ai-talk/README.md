# six-echo-ai-talk

六叔（Six-Echo）的个人 AI 演讲页面与知识工作流设计 Skill。

它把 Esther 不二设计系统的视觉方法，和本项目在真实演讲页面中反复验证的内容架构、图示方式、交互规范、响应式排版、可访问性与发布检查，整理成一套可以直接调用的专属 Skill。

> **一句话**：把一份中文 AI 主题资料，变成一份讲得清、看得懂、能互动、可公开分享的 HTML 演讲页面。

> **当前版本**：v1.0.0 · 2026-08-04

如果你只是想看最终效果，请先打开 [在线演讲页面](https://6ix-echo.github.io/Six_Echo_Html/)；如果你想让 AI 按同样的方法继续生成页面，再安装并调用本 Skill。

---

## 适合什么时候使用

当你需要以下任务时，可以调用本 Skill：

- 把 AI 演讲草稿做成单页 HTML
- 设计 AI 大会、分享会或个人主题演讲页面
- 讲清 Agent、Harness、Prompt、Skill、MCP 等概念
- 为六叔个人 IP 生成带天狗面具头像的页面或海报
- 把 AI 工具和工作经验整理为个人 Skill 体系
- 给已有页面增加翻转卡、标签页、复制按钮和章节导航
- 检查页面的交互、响应式布局、视觉统一性和 GitHub Pages 发布准备

## 不适合什么时候使用

这个 Skill 不是通用的 UI 组件库，也不是只负责“把文字变漂亮”的排版工具。以下任务更适合使用其他专用工具：

- 只需要写一段普通文章或新闻稿
- 只需要完成后端接口、数据库或业务逻辑
- 只需要做数据分析图表而没有演讲叙事需求
- 只需要生成与六叔个人 IP 无关的品牌视觉系统

如果任务同时包含 AI 主题内容、演讲结构和 HTML 交互页面，则优先使用本 Skill。

---

## 核心方法

```text
原始资料
   ↓
演讲叙事：焦虑 → 认知 → 术语 → 工作系统 → 方法 → 行动
   ↓
视觉结构：时间线 / 关系图 / 对照板 / 案例漫画 / 分类标签
   ↓
交互增强：翻转 / Tab / 复制 / 导航 / 返回顶部
   ↓
QA：内容、视觉、交互、响应式、发布
   ↓
可直接打开和分享的 HTML
```

Skill 的重点不是套用固定模板，而是把设计判断转化为可执行约束：先让内容成体系，再选择能帮助观众理解的视觉结构。

---

## 内置工作流

| 步骤 | 做什么 | 目的 |
| --- | --- | --- |
| 1 | 判断页面类型、受众、章节数、素材和硬约束 | 不自作主张改变目标 |
| 2 | 读取 Esther 设计系统和对应场景规范 | 先学视觉规矩再动手 |
| 3 | 提炼演讲线和不可遗漏项 | 防止只做漂亮页面而漏内容 |
| 4 | 选择不同的 Section 布局 | 保持长页面节奏 |
| 5 | 用图示解释关系与流程 | 降低术语理解成本 |
| 6 | 加入必要交互与讲者辅助内容 | 页面既能读也能讲 |
| 7 | 做响应式、键盘、打印和资源检查 | 交付可直接使用的页面 |

---

## 默认内容架构

### 1. 为什么焦虑

用视觉分层、对照和核心观点解释焦虑，不使用夸张或恐吓式表达。

### 2. Agent 与六角色系统

完整呈现：

`LLM → RAG → Agent → Harness → Skill → MCP`

其中 Harness 必须位于 Agent 之后，突出：

> Model 提供能力，Agent 负责行动，Harness 组织可靠执行。

### 3. Harness 露营派对

用“组织一次户外露营烧烤派对”解释 Harness：

1. 接单：目标、人数、地点、时间和边界
2. 翻车：天气、物资、车辆、人员和安全信息没有同步
3. Harness 接管：上下文、状态、工具权限、并行协作和检查点
4. 办成并变好：记录失败、复盘并生成下一次工作记忆

### 4. Prompt 五段式

完整保留：

- Context
- Request
- Output format
- Constraints
- Checkpoint

样例应该以可复制文本呈现，而不是只放截图。

### 5. Skill 体系

从真实重复工作、失败记录和隐性经验出发，沉淀规则、参考、模板、脚本、边界与 Checkpoint，最终形成可复用能力。

Skill 样例采用分类 Tab 展示：

- 内容与视觉
- 研发与工作流
- 知识与研究
- 组织与 AI 员工

条目可以完整保留，但不要全部挤在一屏。

---

## 视觉基因

- 白色主背景，局部使用淡米色卡片或深色收束带
- 蓝色承担主结构，黄色承担节奏，红色承担强调
- 彩色横条、角标、编号和细线优先于大面积彩色方块
- 中文衬线标题 + 清晰无衬线正文
- 手绘感用于漫画和个人 IP，不使用表情包或通用 AI 插画风
- 六叔头像保持红色花纹帽、天狗面具、不露脸、自然比例和肌肉线条
- 头像金句保持原文，只优化排版位置与层级

默认 CSS 变量：

```css
--paper: #ffffff;
--milk: #f8f4e9;
--ink: #1a1a2e;
--muted: #686b78;
--blue: #2b7fd8;
--yellow: #f4d758;
--red: #ee4862;
```

---

## 交互规范

- 头像与二维码使用可访问的翻转按钮
- Tab 使用 `aria-selected` 和 `hidden`
- Prompt 使用复制按钮和成功/失败状态
- 顶部导航支持章节锚点，页面提供返回顶部
- 所有操作控件提供清晰的 `:focus-visible`
- 尊重 `prefers-reduced-motion`
- 触控目标不小于 44px
- 所有内容在移动端单列可读，不依赖 hover 才能理解

---

## 文件结构

```text
six-echo-ai-talk/
├── SKILL.md                    ← 主工作流和触发条件
├── references/
│   ├── project-patterns.md     ← 页面骨架、视觉层级和常见修正
│   └── qa-checklist.md         ← 内容、视觉、交互、发布检查
└── evals/
    └── evals.json              ← 3 个真实使用测试用例
```

可下载的安装包位于：

[six-echo-ai-talk.skill](https://github.com/6ix-Echo/Six_Echo_Html/raw/main/skills/six-echo-ai-talk.skill)

注意：安装包只包含运行 Skill 所需的 `SKILL.md` 和 `references/`，评测用例位于源目录的 `evals/`，用于维护者测试，不会被打进发布包。

---

## 怎么用

将 Skill 安装到你的 AI 工作环境后，直接说：

> 使用 six-echo-ai-talk skill，把这份 AI 资料整理成一份可公开分享的演讲 HTML，保留完整内容，并按六叔的视觉和交互规范实现。

也可以针对单个模块调用：

> 使用 six-echo-ai-talk skill，只重做 Harness 露营派对章节，要求图文可视化、边框统一、照片融入背景板。

### 本地安装

```bash
mkdir -p ~/.codex/skills
unzip six-echo-ai-talk.skill -d ~/.codex/skills/six-echo-ai-talk
```

安装后重新打开 AI 工作环境。如果你的工具支持直接读取 GitHub Skill，也可以使用本目录中的 `SKILL.md` 作为规则源。

### 如何提出更好的请求

为了让输出更接近预期，建议同时说明：

- 页面类型：演讲页、教程页、Landing Page 还是单节解释页
- 受众：技术背景、阅读设备、预计分享时长
- 必须保留的内容：观点、案例、图片、人物信息或原始金句
- 交互要求：翻转卡、Tab、复制、打印或键盘可用性
- 交付方式：本地 HTML、GitHub Pages、Vercel 或其他静态托管

示例：

> 使用 six-echo-ai-talk skill，把这份关于 AI Agent 的草稿做成 15 分钟中文演讲页面。保留所有观点，加入一个露营派对 Harness 案例，白色主背景，移动端可读，Prompt 样例需要支持复制，最后给出 GitHub Pages 发布检查。

## 维护方式

新增规范时，优先判断它属于哪一层：

- 触发条件和总流程 → 修改 `SKILL.md`
- 页面骨架、命名和常见修正 → 修改 `references/project-patterns.md`
- 内容、视觉、交互和发布检查 → 修改 `references/qa-checklist.md`
- 测试输入 → 修改 `evals/evals.json`

修改后应重新检查 YAML frontmatter、资源链接、示例是否可执行，并同步更新版本号和 CHANGELOG。

---

## Credits

- Esther 视觉方法参考：[esthersjw/esther-design-system](https://github.com/esthersjw/esther-design-system)
- 本 Skill 的项目化内容、AI 演讲结构和六叔个人 IP 规范：Six-Echo

## License

本 Skill 中适配 Esther 设计系统的部分遵循 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)，必须保留原作者署名，禁止未经许可的商业使用，修改后以相同协议分享。

六叔个人 IP、头像、社群素材和项目内容归 Six-Echo 所有，未经许可请勿用于商业用途或冒充官方身份。
