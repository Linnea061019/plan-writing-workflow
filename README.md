# 计划书协作写作

`plan-writing-workflow` 是用于协作撰写和迭代计划书的 Codex Skill，支持从构想起草、逐章共创、现稿修订与文件交付。适用于项目、建设、运营、活动及创业计划书。

## 协作方式

按当前任务进入流程，已有信息不重复询问。需要梳理时，围绕八个阶段选择问题：

1. 用途与任务边界。
2. 服务对象、具体痛点与现有资源。
3. 目标、服务边界与规模。
4. 方案与资源配置。
5. 运营机制与责任。
6. 预算、资金与可行性。
7. 进度、风险与成效。
8. 正文、修订与交付。

每阶段提供首问、根据回答选择的追问及起草条件。模糊回答追实例，数字补口径，未知事实列待核实，冲突先分清范围；不套用固定问卷。

正文按章节判断是否可以起草，并区分章节草稿、完整讨论稿和正式用途成稿。预算未齐不妨碍先写概况，讨论稿中的建议与备选方案保持可见。完整方法见 [计划书写作方法](references/workflow.md)。

## 安装与调用

下载 [plan-writing-workflow.zip](plan-writing-workflow.zip)，将其中的 `plan-writing-workflow` 文件夹解压到本地 `~/.codex/skills/`，形成：

```text
~/.codex/skills/plan-writing-workflow/SKILL.md
```

调用示例：

```text
使用 $plan-writing-workflow，帮我把以下构想整理成计划书。
先利用已有信息，只问影响当前方案的关键问题。
```

也可以指定阶段或修改范围：

```text
使用 $plan-writing-workflow，按现有底稿只修改预算，并同步相关段落。
```

## 文件

| 文件 | 内容 |
| --- | --- |
| [SKILL.md](SKILL.md) | 入口、协作规则与起草条件 |
| [references/workflow.md](references/workflow.md) | 完整流程、阶段提问与追问分支 |
| [references/decision-checks.md](references/decision-checks.md) | 十五类易错情境与检查标准 |
| [agents/openai.yaml](agents/openai.yaml) | 界面名称与默认调用提示 |
| [plan-writing-workflow.zip](plan-writing-workflow.zip) | 包含上述四个 Skill 文件的安装包 |

Skill 复用写作方法，不带入特定项目的地址、金额、公益定位或审批流程。仅做局部修订、格式转换或打包时，不重启完整访谈。
