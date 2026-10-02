# my-workspace

ZCode（Claude Code 类编码代理）工作区已安装的**第三方插件与 Skills 清单**。官方自带插件不在本清单内。

- Skills 安装位置：`~/.zcode/skills/`
- 插件安装位置：`~/.zcode/cli/plugins/cache/`
- Skills 统一用 Vercel 的 skills CLI 安装：`npx skills add <owner>/<repo> -a zcode -g --copy -y`（下表「来源」即该命令的包标识，非 npm 运行时依赖）

## 第三方插件（1 个）

| 名称 | 仓库 | 用处 | 特点 | 安装时间 |
|---|---|---|---|---|
| **taste-skill** | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 前端设计品味/审美插件，一套 13 个 skill | 覆盖多种风格流派（极简、工业粗野主义、高端视觉等）、品牌工具箱（brandkit）、截图转代码（image-to-code）、现有项目重设计、图像生成风格前端、GSAP 动效预设；v1.0.0 | 2026-09-08 |

## 第三方 Skills（17 个，来自 9 个仓库）

### 动效 / 视频类

| 名称 | 仓库 | 用处 | 特点 |
|---|---|---|---|
| **gsap-core / gsap-frameworks / gsap-performance / gsap-plugins / gsap-react / gsap-scrolltrigger / gsap-timeline / gsap-utils**（8 个） | [greensock/gsap-skills](https://github.com/greensock/gsap-skills) | GSAP 动画开发全流程 | GreenSock 官方出品，按主题拆成 8 个 skill：核心、框架集成、性能、插件、React、ScrollTrigger、时间轴、工具函数 |
| **onetake** | [feitangyuan/onetake](https://github.com/feitangyuan/onetake) | 「一镜到底」动效短片：产品发布片、teaser、功能演示 | 单 HTML 合成、每个数值都是时间的纯函数；内置约 38 种实测动效、真实快门运动模糊（1080p30 草稿 / 4K60 成片）、同一房间感的合成音效、自动 oracle 验收（拒绝 PPT 式节奏）；PolyForm Noncommercial 许可，**仅限非商用** |
| **morphicons** | 自制 skill（封装 [morphicons](https://www.npmjs.com/package/morphicons) npm 包） | 图标 morph 动画：menu↔X、play↔pause 等切换 | 唯一自写条目，非第三方；弹簧物理驱动 SVG 描边变形，支持 React/Vue/Svelte/vanilla，可跨图标库（Lucide/Tabler/Heroicons）转换数据 |

### 设计 / UI-UX 类

| 名称 | 仓库 | 用处 | 特点 |
|---|---|---|---|
| **frontend-design** | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/frontend-design) | 前端视觉设计指导：审美方向、排版、配色 | Anthropic 官方；主打「反模板化」——像设计工作室主创一样做有态度的、贴合主题的视觉决策 |
| **ui-ux-pro-max** | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | UI/UX 设计综合辅助 | 自带**本地设计数据库**：配色系统、字体搭配、UX 准则、GSAP 动效预设，离线可查 |
| **vercel-react-best-practices** | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) | React / Next.js 性能优化准则 | Vercel Engineering 官方，MIT；触发于写/审/重构 React 代码、数据获取、bundle 优化等场景 |

### 文本 / 流程类

| 名称 | 仓库 | 用处 | 特点 |
|---|---|---|---|
| **humanizer-zh** | [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) | 去除中文文本的 AI 生成痕迹 | 翻译自 blader/humanizer，基于维基百科「AI 写作特征」指南；按模式检测：夸大象征、宣传腔、三段式、破折号滥用、AI 词汇等 |
| **to-spec** | [mattpocock/skills](https://github.com/mattpocock/skills) | 把模糊想法变成可执行的 spec | Matt Pocock 出品；前身 to-prd 已退役改名 |
| **tdd** | [mattpocock/skills](https://github.com/mattpocock/skills) | 测试驱动开发（红→绿→重构） | 同上仓库；强调「值得保留的测试」，含反模式清单，skills.sh 下载量百万级 |
| **grilling** | [mattpocock/skills](https://github.com/mattpocock/skills) | 用尖锐追问拷问/澄清需求 | 同上仓库 |
| **grill-me** | [mattpocock/skills](https://github.com/mattpocock/skills) | 触发 grilling 的快捷入口 | 同上仓库；本身只是 stub，实际逻辑在 grilling |
| **find-skills** | [vercel-labs/skills](https://github.com/vercel-labs/skills) | 发现与安装 agent skills 的元技能 | `npx skills` CLI 的配套技能，检索 skills.sh 开放生态 |

## 备注

- 官方插件（github、documents、pdf、pptx、xlsx、browser-use、computer-use、obsidian、video-agent-kit、video2code、wecom-cli、tencent-meeting-cli 等）来自 `zcode-plugins-official` 市场，不属于第三方，未列入。
- 曾装过但已移除：`open-kimi-ppt`（导出接口失效）、`android-emulator`（工具名超长致 MCP 400 报错）。
- 统计口径：插件 1 个；skills 目录共 19 个，除自制 morphicons 外 18 个第三方 skill，来自 9 个第三方仓库。
