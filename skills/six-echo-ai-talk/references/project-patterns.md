# Six-Echo 项目模式参考

本文件记录从 `ai-human-ai-talk.html` 提炼的可迁移模式，不复制具体演讲内容。

## 页面骨架

```html
<header class="topbar">章节锚点导航</header>
<main>
  <section class="hero">标题、身份标签、头像翻转卡</section>
  <section id="why">焦虑的分层与核心观点</section>
  <section id="history">技术跃迁时间线</section>
  <section id="agent">AI 术语与六角色系统</section>
  <section id="harness">生活化案例 + Harness 图示</section>
  <section id="practice">Prompt Flow + 完整模板 + 复制</section>
  <section id="skill-system">搭建 Skill</section>
  <section id="skills">Skill 样例分类切换</section>
  <section id="action">行动收束</section>
</main>
<footer>署名、参考链接、回到顶部</footer>
```

## 视觉结构

- `section-head` 统一处理英文小标签、大标题和导语。
- `sticky-layout` 适合左侧章节号固定、右侧内容滚动。
- `visual-node`、`visual-connector` 适合概念关系图。
- `speaker-note` 适合把开场稿、转场稿、解释稿降级为可展开辅助内容。
- `view-tabs`、`prompt-switch`、`skill-tabs` 适合分组内容，不让所有内容同时出现。
- `harness-comic-grid` 适合四格案例，图片与正文采用相同卡片边界。

## 文案层级

每个 section 依次使用：

1. 英文 kicker：短、全大写、红色，配蓝色横条。
2. 中文主标题：深色、高对比，不超过两行为佳。
3. 导语：解释观众为什么要关心。
4. 图示标题：直接说出关系，不用泛化口号。
5. 正文：每段一个观点，搭配编号、边界或检查结果。

## 常见修正

- 发现暖色背景铺满页面：恢复主区域为白色，只保留少量 `--milk` 作为内容卡片。
- 发现彩色方块过多：改为顶部角标或底部横条。
- 发现图文拥挤：缩小图片、扩大留白、把长文案拆成阶段卡。
- 发现标题发灰：标题回到 `--ink`，只让说明文字使用 `--muted`。
- 发现 Skill 条目太多：改为类别 tab，类别内保留完整条目。
- 发现 Harness 边框突兀：采用与全站相同的细线、浅色背景和横条，不用深色粗边框。
