# bookflow-skill

把 AI 辅助写小说从“一次性生成”变成可复用的短篇生产流程。

这套 Skill 来自两部分真实资料：

- `references/factory/`：AI 小说批量生产工厂，包含选题、对标、冲突、人物、试读、项目生产、发布和复盘资料；
- `references/bookflow-prompts/`：BookFlow 当前使用的实际提示词模块。

## 适用场景

- 番茄短篇选题与项目化生产；
- 女性情感、婚恋火葬场、古言反转、悬疑短篇；
- README → 角色 → 大纲 → beat → 正文 → 配套素材 → QA → 复盘；
- 用 Codex、Claude 或兼容 API 做人机协作写作。

## 使用方式

在支持 Codex Skill 的环境中，将仓库作为一个 Skill 目录使用，并显式调用：

```text
Use $bookflow-skill to turn this story idea into a scored short-fiction project.
```

如果配合本地 BookFlow 使用，先启动 BookFlow，再从“选题”进入；具体阶段映射见 [references/workflow-map.md](references/workflow-map.md)。

## 设计原则

- 人控制题材、人物、方向和发布决定；
- AI 加速拆解、结构化、草稿和检查；
- 每一步都有输入、输出和人工确认点；
- 不把平台门槛、流量和收益写成永久保证；
- 发布前保留原稿和可回滚版本。

## License

MIT，见 [LICENSE](LICENSE)。
