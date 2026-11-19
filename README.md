# Marvin 营销 Skills

面向品牌、产品营销和代理商团队的中文 Codex 插件。安装一个插件即可使用 9 个 Skill，从诊断和定位到 Campaign、渠道、转化与证据审查。跨阶段任务可以从项目编排入口开始，也可以单独选择专业 Skill。

公开版使用你提供的 Brief、附件和可核验的公开资料。只有一份 Brief 也可以起步，输出会标明哪些是事实、试验假设和待核验项。

## 安装

1. 在本仓库选择 **Code → Download ZIP**，解压到便于保留的位置。也可以直接克隆本仓库。
2. 在解压后的仓库根目录打开终端，运行以下命令。

```sh
codex plugin marketplace add .
codex plugin add marketing-skills@marvin-skills
```

在 Codex 开一个新对话，从 Skill 选择器选择 `marketing-project-orchestrator` 开始。可用 `codex plugin list` 核对安装。 [详细安装、换机和排查说明](INSTALL.md)

## 第一次使用

在 Codex 中打开仓库目录，选择营销项目编排，使用这条提示。

> 读取 `examples/fictional-launch/brief.md`，给我一份可讨论的新品首发试投草案。请明确核心用户行为，写两种短视频开场，说明什么条件下可以追加预算，并审核会暗示产品性能的画面和文案。

也可以直接阅读[虚构新品 Brief](examples/fictional-launch/brief.md)和[完整演练稿](examples/fictional-launch/walkthrough.md)。案例的品牌、产品和业务数字均为虚构，展示了从 Campaign、内容渠道和交易实验到证据审稿的交接。

## 9 个可用 Skill

| 序号 | Skill | 能完成的工作 |
|---|---|---|
| 01 | [营销问题诊断](plugins/marketing-skills/skills/marketing-brief-diagnosis/SKILL.md) | 把模糊诉求拆成待决策的问题、假设和验证顺序。 |
| 02 | [市场与消费者洞察](plugins/marketing-skills/skills/market-audience-insight/SKILL.md) | 梳理人群、需求场景和证据边界，形成可验证的机会。 |
| 03 | [品牌策略与定位](plugins/marketing-skills/skills/brand-strategy-positioning/SKILL.md) | 比较定位选项、价值主张、支持理由和取舍。 |
| 04 | [整合 Campaign 策划](plugins/marketing-skills/skills/campaign-strategy-design/SKILL.md) | 从核心行为设计创意机制、触点和试点节奏。 |
| 05 | [内容与渠道策略](plugins/marketing-skills/skills/content-channel-strategy/SKILL.md) | 规划内容支柱、平台分工、分发衡量和可拍脚本。 |
| 06 | [电商与直播转化增长](plugins/marketing-skills/skills/commerce-conversion-growth/SKILL.md) | 梳理漏斗和交易承接，设计小额试验和复盘口径。 |
| 07 | [出海本地化策略](plugins/marketing-skills/skills/cross-border-localization/SKILL.md) | 整理市场进入假设、本地化约束和试点计划。 |
| 08 | [营销证据与方案审查](plugins/marketing-skills/skills/marketing-evidence-review/SKILL.md) | 逐条核查文字、数字、案例和画面暗示，提出可用替换。 |
| 09 | [营销项目编排](plugins/marketing-skills/skills/marketing-project-orchestrator/SKILL.md) | 按交付需求调配相关 Skill，衔接各阶段并汇总方案。 |

## v0.1.1 的两项改进

- [付费预算追加前的能力核验](plugins/marketing-skills/skills/_shared/paid-readiness.md)提示团队在开投、追加和正式对照试验前，核验账户权限、投放控制、归因与退款数据。
- [画面暗示的产品性能审查](plugins/marketing-skills/skills/marketing-evidence-review/references/visual-claims.md)帮助团队逐镜头审查剪辑、字幕和口播共同暗示的性能，并给出替换镜头。

## 许可

本项目采用 [MIT 许可证](LICENSE)。使用、修改或再分发时保留版权与许可声明。
