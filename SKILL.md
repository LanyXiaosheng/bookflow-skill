---
name: bookflow-skill
description: "Run a human-led AI short-fiction workflow from topic selection through outline, chapter drafting, anti-AI editing, platform packaging, and post-publication review. Use for BookFlow, 番茄短篇, AI-assisted novel writing, or requests to turn a story idea into a repeatable production project."
---

# BookFlow AI 小说生产 Skill

把一个故事脑洞推进成可检查、可发布、可复盘的短篇项目。AI 负责候选生成、结构化和草稿加速，人负责题材判断、人物取舍、事实核验、最终改稿和发布决定。

## 适用边界

- 适用于番茄短篇、女性情感、婚恋火葬场、古言反转、悬疑规则怪谈等短篇生产。
- 默认先做短篇验证，不把 6000 字或任何平台门槛写成永久保证；发布前以平台当前规则为准。
- 不把 AI 初稿直接当成最终稿。保留原稿、提示词版本、人工修改记录和平台数据。
- 不自动发布、签约、付款或提交敏感身份资料；这些动作由用户在目标平台完成。

## 标准链路

1. **选题**：确定主分类和情节标签，生成 5 个以上候选标题。
2. **筛选**：按标题点击欲、冲突明确度、赛道辨识度、差异化评分；低于项目线的题进入备选或淘汰。
3. **立项**：建立项目 README，写清目标读者、核心卖点、情绪曲线、文风和禁区。
4. **角色**：生成角色总表、关系图、欲望/恐惧、秘密、说话方式和成长弧线；人工确认后再继续。
5. **大纲**：生成章节标题、主要冲突、情绪目标和章尾钩子。角色设定改变后，先重生大纲。
6. **正文**：按章节和 beat 分段生成，保存上下文；逐章检查字数、连续性、人物声音和钩子。
7. **去 AI 味**：用具体动作、场景和对话替代总结句；删除模板化形容词、重复转折和万能金句。
8. **发布包**：生成全书汇总、平台简介、导语、标题变体、推送语、标签、引流选段和封面提示词。
9. **QA 与打包**：做敏感词、角色名、时间线、逻辑、平台格式和原创性检查，下载可回滚的 ZIP。
10. **发布复盘**：发布后按 24h/72h/7d 录入数据，判断爆/平/扑，回写成功原因、失败原因和下一步。

## BookFlow 对应入口

- `选题`：主分类、情节标签、AI 试评、四维评分和候选池。
- `项目`：项目 Kanban、状态迁移和项目详情。
- `项目详情`：README、角色设定、大纲、正文、全书汇总、配套素材、配图和 ZIP。
- `写作`：章节、beat、AI 写章、局部修改和字数底线。
- `待发 / 已发 / 复盘`：发布前检查、状态记录和数据回收。
- `设置`：配置 Anthropic Messages 或 OpenAI-compatible API；API Key 只保存掩码。

## 读取 supporting references

- 先读 [workflow-map.md](references/workflow-map.md) 了解阶段、入口和出场标准。
- 需要选题、标题、冲突或试读结构时，读 `references/factory/02-资产库/` 下对应资料。
- 需要完整内容治理时，读 `references/factory/04-完整链路SOP.md`。
- 需要对照 BookFlow 的实际模型提示词时，读 `references/bookflow-prompts/` 中对应的 `.system.md` 文件。

## 每次交付前检查

- 是否明确题材、目标读者、开局死局、反杀动作和结局方向？
- 是否在正文前确认角色设定和大纲？
- 是否保留原稿和可回滚版本？
- 是否区分 AI 生成、人工修改、平台审核和真实发布状态？
- 是否把收入、流量和签约条件标成个人实测或平台当前页面信息，而不是固定承诺？
