# BookFlow 工作流映射

## 阶段与交付物

| 阶段 | BookFlow 入口 | 主要交付物 | 出场标准 |
| --- | --- | --- | --- |
| 选题 | 选题 | 标题、卖点、主分类、情节标签、评分 | 有明确冲突，达到项目线或进入备选池 |
| 立项 | 选题中的进项目 | 项目记录 | 标题、赛道、目标读者已锁定 |
| 前期方案 | 项目详情 | README、角色设定 | README 完成，角色设定人工确认 |
| 结构 | 项目详情 | 章节大纲、爆点节奏 | 每章有事件、情绪和章尾钩子 |
| 正文 | 进入写作 | 分章节正文 | 人物、时间线和字数通过检查 |
| 发布准备 | 项目详情 | 全书汇总、配套素材、配图、ZIP | 发布稿、简介、标题和素材齐全 |
| 发布 | 待发 / 已发 | 状态和平台链接 | 用户人工完成平台发布 |
| 复盘 | 复盘 | 24h/72h/7d 数据和结论 | 有数据、有判断、有下一步 |

## 推荐执行顺序

1. 先选一个题，不要同时生成几十个完整项目。
2. 用 4 维评分卡筛选：标题点击欲、冲突明确度、赛道辨识度、差异化。
3. 进入项目后，先生成 README，再生成角色设定。
4. 角色设定必须人工确认。改名或改关系后，重新生成大纲。
5. 先生成章节 beat，再逐章写正文；每章写完立即检查。
6. 正文完成后再生成汇总、配套素材和封面，不要让配套素材反过来决定正文。
7. 发布前保留原始 Markdown、最终稿和 ZIP。
8. 发布后按时间窗口录入真实数据，不能用总曝光代替阅读、完读和互动。

## 推荐 Skill 组合

### 核心

- `bookflow-skill`：总流程、阶段门禁和素材路由。
- BookFlow prompts：README、角色、大纲、beat、正文、汇总、配套和发布 QA。

### 内容质量

- `stop-slop`：去模板化表达、降低 AI 味、调整节奏。
- `ai`：提示词版本管理、输入输出验证、成本与效果平衡。

### 发布复用

- `x-mastery-mentor`：把实操经历整理成 X Article、Thread 或发布说明。
- `visual-imprint` 或 `lany-cover`：需要统一个人 IP 封面和正文视觉时使用。

## 关键提示词模块

| 目标 | 文件 |
| --- | --- |
| 选题生成 | `seed_generator.system.md` |
| 选题评分 | `seed_scorer.system.md` |
| 项目说明 | `project_readme.system.md` |
| 角色设定 | `project_character_setup.system.md` |
| 章节大纲 | `project_outline.system.md` |
| beat 拆分 | `chapter_beats.system.md` |
| 正文生成 | `chapter_write.system.md` / `chapter_write_full.system.md` |
| 去 AI 味 | `anti_ai_rules.md` / `project_book_polish.system.md` |
| 全书汇总 | `project_book_summary.system.md` |
| 发布配套 | `project_side_dishes.system.md` |
| 发布检查 | `publish_qa.system.md` |
| 复盘分析 | `review_analyze.system.md` |
