# natural-expression · 清楚表达

一个中文写作与说话表达 skill。先整理材料、读者和目的，再处理内容衔接与语言，让表达清楚、连贯、自然，同时保留事实、观点、确定程度和作者声音。

## 能做什么

| 模式 | 用途 |
|---|---|
| 新写 | 根据材料写文章、说明或发言 |
| 改稿 | 润色、压缩、去套话，保留原意 |
| 口播与对话 | 整理演讲、逐字稿和回复，检查听一遍能否理解 |
| 审稿 | 定位逻辑缺口、冗余和衔接问题，给出修改建议 |

词语、句式、标点和比喻按语境检查，不设统一禁词表或句长门槛。现实内容不补造经历、数据与引用；改稿后核对否定、条件、时间、范围、归因和完成状态。默认只交可直接使用的成稿，用户要求检查时提供诊断。

## 调用示例

```text
使用 natural-expression，把下面的材料写成一篇面向普通读者的说明。

使用 natural-expression，润色下面这段话，保留事实和我的语气，只给最终稿。

使用 natural-expression，把下面的稿子改成两分钟口播。

使用 natural-expression，只检查哪里不顺和哪里缺论据，先不要重写。
```

在这些提示后附上材料或原稿即可。

## 在 Codex Cloud 使用

1. 把本仓库加入云端环境，在本仓库目录中开始任务，确认任务能读取 `.agents/skills/natural-expression/SKILL.md`。
2. 使用上面的自然语言提示。若未识别 skill，可明确要求：`请先读取 .agents/skills/natural-expression/SKILL.md，并按需读取其 references，再处理下面的材料。`
3. 在其他项目使用时，把完整的 `.agents/skills/natural-expression/` 目录复制到目标仓库的 `.agents/skills/` 下，提交到云端任务使用的分支，并确认任务能看到这些文件。

本机个人 skill 不会自动同步到云端；云端任务可以使用仓库内的 skill。见 [OpenAI 官方云端环境说明](https://learn.chatgpt.com/docs/environments/cloud-environments#current-limitations)。仓库 skill 的发现路径见 [Build skills](https://learn.chatgpt.com/docs/build-skills)。

## 目录

skill 位于 `.agents/skills/natural-expression/`，复制时保留整个目录。

| 文件 | 用途 |
|---|---|
| [SKILL.md](.agents/skills/natural-expression/SKILL.md) | 入口、任务分流、保真边界与交付方式 |
| [references/writing.md](.agents/skills/natural-expression/references/writing.md) | 材料、结构与新写方法 |
| [references/editing.md](.agents/skills/natural-expression/references/editing.md) | 改稿与审稿检查 |
| [references/spoken.md](.agents/skills/natural-expression/references/spoken.md) | 口播、演讲与对话 |
| [references/sources.md](.agents/skills/natural-expression/references/sources.md) | 四个来源的总结、固定版本与整合取舍 |
| [agents/openai.yaml](.agents/skills/natural-expression/agents/openai.yaml) | skill 的界面名称与描述 |

## 来源与许可

整合 human-writing、dbs-script-flow、Humanizer-zh 与 humanizer 的方法。详细出处见 [来源总结](.agents/skills/natural-expression/references/sources.md)。

本整合包按 [CC BY-NC 4.0](.agents/skills/natural-expression/LICENSE) 分发，使用和改编时保留署名，不用于商业用途；上游 MIT 声明及署名见 [THIRD_PARTY_NOTICES.md](.agents/skills/natural-expression/THIRD_PARTY_NOTICES.md)。
