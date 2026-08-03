# Six-Echo AI Talk

一个面向公开分享的 AI 主题演讲网页与个人知识工作流。

把“AI 时代的人与人、AI 焦虑、Agent、Harness、Prompt、Skill”从一份演讲草稿，整理成一套可以阅读、讲解、互动和持续维护的单页 HTML。

> **在线演讲页面**：https://6ix-echo.github.io/Six_Echo_Html/

> **主讲人**：六叔（Six-Echo）  
> 移动互联网早期连续创业者 · 数十年互联网、自动驾驶、机器人及 AI 领域从业 · 机器人认知智能硕士

---

## Demo

### 🎙️ 在线演讲页面

一份可直接对外分享的长页面演讲稿，适合会议分享、主题演讲、个人主页或会后资料复盘。

🔗 [打开在线页面](https://6ix-echo.github.io/Six_Echo_Html/)

页面内置：

- 六叔个人 IP 头像与社群二维码翻转卡
- AI 焦虑的视觉化解释
- 技术跃迁时间线
- LLM / RAG / Agent / Harness / Skill / MCP 六角色工作系统
- 露营烧烤派对 Harness 生活化案例
- Prompt 五段式模板与完整示例
- Skill 体系搭建与分类浏览
- 演讲提示、章节导航、复制按钮、返回顶部和打印样式

---

## 这不是一个更大的聊天框

这份页面试图建立一条完整的认知路径：

```text
AI 焦虑
   ↓
看见技术范式变化
   ↓
理解 LLM / RAG / Agent / Harness / Skill / MCP 的分工
   ↓
把 Prompt 写成工作说明书
   ↓
把真实工作沉淀成个人 Skill
   ↓
用可复用的 AI 工作流拉开行动差距
```

核心判断是：AI 不会简单地把人变成“无用的人”，但会重新组织那些没有持续更新工作方法的人。工具是放大器，人是方向盘。

---

## 内容结构

| Section | 讨论什么 | 页面表达 |
| --- | --- | --- |
| 为什么焦虑 | AI 会不会淘汰人类，以及焦虑从哪里来 | 分层观点、对照和行动差距 |
| 技术跃迁 | 为什么旧经验不会自动适配新范式 | 时间线与先行者视角 |
| Agent | Agent 在 AI 工作系统中负责什么 | 六角色关系图 |
| Harness | 如何让 Agent 稳定把事办成 | 露营派对漫画、流程和对照 |
| Prompt | 如何把请求写成清晰的工作说明书 | 五段式流程、样例、复制 |
| 搭建 Skill | 如何从真实失败中积累工作记忆 | 输入—Skill—输出系统图 |
| Skill 样例 | 哪些方法值得沉淀成可复用技能 | 分类标签页与条目说明 |
| 行动 | 听完之后从哪里开始 | 三个可执行动作 |

---

## 六角色 AI 工作系统

| 角色 | 页面中的比喻 | 责任 |
| --- | --- | --- |
| LLM | 大脑 | 思考、理解与生成，但不等于掌握全部事实 |
| RAG | 开卷考试 | 先查资料，再基于资料回答 |
| Agent | 手脚 | 从目标走向规划、调用、执行和检查 |
| Harness | 组织系统 | 管理上下文、状态、工具、权限、验证和复盘 |
| Skill | 做事方法 | 把规则、参考、模板、脚本和边界沉淀下来 |
| MCP | 万能插板 | 连接模型与文件、数据库、服务和外部工具 |

页面刻意把 Harness 放在 Agent 之后：模型提供能力，Agent 负责行动，Harness 组织可靠执行。

---

## 设计与交互

本项目采用 Esther 不二设计系统的视觉方法，并结合六叔个人 IP 做了项目化适配：

- 白色主背景，搭配蓝、黄、红三色作为信息强调
- 中文衬线标题与无衬线正文形成阅读层级
- 彩色横条、角标、编号和细线代替无意义的色块堆叠
- 每个 Section 使用不同布局，保持长页面的节奏
- 天狗面具头像保持不露脸，头像与二维码使用可点击翻转卡
- 术语、流程、案例和 Skill 条目都采用可视化结构，避免长段文字堆叠
- 支持移动端、键盘操作、`prefers-reduced-motion` 和打印样式

---

## 文件结构

```text
Six_Echo_Html/
├── index.html                         ← GitHub Pages 入口
├── assets/                            ← 页面图片和视觉素材
│   ├── liu-shu-ip.png                 ← 六叔个人 IP 头像
│   ├── liu-shu-community-qr.png       ← 社群二维码
│   ├── liu-shu-community-poster.jpg   ← 社群海报
│   ├── harness-camp-*.webp             ← Harness 露营案例漫画
│   ├── term-*.png                      ← AI 术语图示
│   └── prompt-*.png                    ← Prompt 图示
├── skills/
│   ├── six-echo-ai-talk/               ← 专属 Skill 源文件
│   └── six-echo-ai-talk.skill          ← 可迁移安装包
└── .nojekyll                           ← GitHub Pages 静态发布标记
```

---

## 怎么使用

### 直接阅读

打开 [在线页面](https://6ix-echo.github.io/Six_Echo_Html/)，通过顶部导航跳转到对应章节。

### 本地打开

```bash
git clone https://github.com/6ix-Echo/Six_Echo_Html.git
cd Six_Echo_Html
open index.html
```

页面采用相对资源路径，不依赖后端服务。

### 使用专属 Skill

阅读 [six-echo-ai-talk Skill](skills/six-echo-ai-talk/)，或者下载 [six-echo-ai-talk.skill](skills/six-echo-ai-talk.skill) 安装包。

调用示例：

> 使用 six-echo-ai-talk skill，把这份 AI 主题资料整理成一份可公开分享、可交互、可打印的中文演讲 HTML 页面。

---

## 质量检查

- 内容结构完整，不遗漏 Agent、Harness、Prompt、Skill 等关键模块
- 白色背景、色条、标题对比度与图片比例保持统一
- 头像翻转、标签切换、复制按钮和返回顶部均可操作
- 移动端无横向溢出，长文本不会遮挡
- 键盘焦点、图片替代文本和 reduced motion 状态可用
- 发布时只包含页面、图片和 Skill，不包含测试依赖、私密资料或草稿文件

---

## Credits

- 视觉方法与基础设计语言参考 [Esther 不二设计系统](https://github.com/esthersjw/esther-design-system)
- 本项目在其 CC BY-NC-SA 4.0 许可基础上进行六叔个人 IP 与演讲场景适配
- 内容、案例、页面实现和 `six-echo-ai-talk` 专属 Skill：Six-Echo

## License

本项目中的 Esther 设计系统适配部分遵循 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)：

- ✅ 可使用、修改和分享
- ✅ 必须保留 Esther 不二署名
- ❌ 禁止未经许可的商业使用
- 🔄 修改后的适配版本需以相同协议分享

六叔个人 IP、头像、社群二维码和个人内容素材归 Six-Echo 所有，未经许可请勿用于商业用途或冒充官方身份。
