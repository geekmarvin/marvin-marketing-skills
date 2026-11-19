# 安装 Marvin 营销 Skills

使用支持 `codex plugin` 命令的 Codex CLI。插件的 9 个 Skill 和共享参考随同一个包安装，共用你的正常 Codex 登录。项目可以只使用自己的 Brief 和附件。

## 从 ZIP 或克隆目录安装

1. 从仓库下载 ZIP 并解压，或将仓库克隆到本机。选择一个可以保留的目录。本地市场登记会指向该目录。
2. 从含 `README.md`、`.agents` 和 `plugins` 的仓库根目录打开终端。
3. 登记本地市场并安装插件。

```sh
codex plugin marketplace add .
codex plugin add marketing-skills@marvin-skills
codex plugin list
```

在列表中查找 `marketing-skills@marvin-skills`。然后用同一 Codex 配置开一个新对话，在 Skill 选择器里搜索 `marketing-project-orchestrator`，或选择[任意专业 Skill](README.md#9-个可用-skill)。

## 在新电脑上用同一版

在新电脑上安装 Codex，下载同一个版本的仓库文件，再执行上面的安装步骤。9 个 Skill 与共享资源会随同这个插件安装，已有 Brief 和业务资料按项目需要单独提供。

也可以直接用本仓库的 GitHub HTTPS 地址登记来源。把下例中的 `OWNER/REPO` 替换为 GitHub 页面的实际路径。若安装指定发行版，可在登记命令末尾加 `--ref` 和对应 Git 标签。

```sh
codex plugin marketplace add https://github.com/OWNER/REPO
codex plugin add marketing-skills@marvin-skills
```

## 安装排查

- **终端找不到 `codex` 或不识别 `plugin`。** 安装或更新到支持该命令的 Codex CLI。 [Codex CLI 安装指引](https://learn.chatgpt.com/docs/codex/cli)
- **找不到本地市场。** 回到同时包含 `.agents/plugins/marketplace.json` 与 `plugins/marketing-skills/plugin.json` 的目录，确保解压时保留了 `.agents`。
- **已安装但 Skill 列表没刷新。** 确认 Codex 客户端和终端使用同一配置，重开对话。若同名 Skill 来源不同，选择本插件提供的版本。 [Codex Skill 发现说明](https://learn.chatgpt.com/docs/build-skills)
- **更新或换下载来源。** 先用 `codex plugin marketplace list` 确认登记路径。若需替换本地旧版，可从新版本目录重新登记。遇到同名旧市场时，可以先用下方命令移除本插件和它的专用市场条目，再按上面的步骤安装新版本。 [插件命令参考](https://learn.chatgpt.com/docs/cli/reference#codex-plugin)

## 卸载

```sh
codex plugin remove marketing-skills@marvin-skills
codex plugin marketplace remove marvin-skills
```
