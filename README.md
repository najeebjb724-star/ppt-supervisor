# 猫猫来做PPT · ppt-supervisor

![WorkBuddy Expert](https://img.shields.io/badge/WorkBuddy-Expert-6C5CE7) ![Version](https://img.shields.io/badge/version-1.0.0-blue) ![License: MIT](https://img.shields.io/badge/License-MIT-green)

> WorkBuddy 专家：按五阶段 SOP 陪你做 PPT——**逻辑没磨出来，不让你往下走。**

名字很可爱，内核很严格。它不是"帮你一键生成 PPT"的工具，而是一位 PPT 制作监理：名字叫猫猫，做事像严师。

## 它解决什么问题

AI 直接生成 PPT 的通病：页数有了、模板很漂亮，但**逻辑不是你的**——汇报时讲不顺，被追问就露馅。

这个专家反着来。五阶段流程里最核心的一条铁律：

> **阶段二的 PPT 逻辑必须由你自己写出来。**它只陪练、质疑、补漏，绝不代写。逻辑没磨出来，不放行进入下一阶段。

以及一条评审金句：

> 如果某句话的作用只是防止被质疑，而不是推进论证，请删除。

## 五阶段流程

| 阶段 | 它做什么 | 门禁 |
|---|---|---|
| 1. 搜集资料 | 搜集整理资料、找模板和风格方向 | 等你拍板资料范围与风格 |
| 2. 磨 PPT 逻辑 | 陪练式对话引导你产出逻辑，质疑薄弱环节 | **逻辑未确认，禁止往下走** |
| 3. 拆分生成素材 | 逐页素材清单 + 风格样图 | 清单与样图均需你确认 |
| 4. 开始生成 | 指挥生成 PPT，逐页对照逻辑 | — |
| 5. 大师评审 | 切换大师人格：字体、论证推进、删防质疑句 | 输出按严重程度排序的问题清单 |

每次会话结束输出一份**交接小结**（当前阶段、关键决策、待办、下次入口），下次进来说"继续"就能接着干——让下一个会话接得住。

## 安装

**方式一（推荐，10 秒）**

WorkBuddy 客户端 → 左侧【专家·技能·连接器】→【专家】→ 搜索 **「猫猫来做PPT」** → 召唤专家。

**方式二（源码）**

从本仓库 [Releases](../../releases) 下载 `ppt-supervisor.zip`，解压到本地专家目录：

```
Windows: C:\Users\<你的用户名>\.workbuddy\plugins\marketplaces\my-experts\plugins\ppt-supervisor\
```

重启 WorkBuddy 后在【我的专家】中可见。

## 使用

开场一句话即可，它会先"对表"判断你在哪一步，从实际位置切入，不逼你从头走：

- 「新PPT项目：帮我从搜集资料开始走流程」
- 「资料已齐，现在开始磨PPT逻辑」
- 「PPT初稿完成，切换大师评审找问题」

## 设计原则

- **门禁是硬的**：跳过阶段必须警告 + 二次确认，绝不静默放行
- **不代写逻辑**：你亲自动脑是流程的核心价值
- **已完成的阶段不重来**：带着成果进来，直接从当前节点继续
- **交接优先**：所有产物按"下一个 AI 能接得住"的标准输出

## 定制

- 改行为/门禁/评审清单：编辑 [`agents/ppt-supervisor.md`](agents/ppt-supervisor.md)
- 改名称、标签、推荐提示词：编辑 [`.codebuddy-plugin/plugin.json`](.codebuddy-plugin/plugin.json)
- 头像：替换 `avatars/expert.png`（512×512，≤500KB）

改完后在本地重新校验注册即可生效（参考 WorkBuddy 官方专家开发规范）。

## 反馈

使用中遇到门禁太松/太紧、评审清单缺项，欢迎开 [Issue](../../issues)。

## License

[MIT](LICENSE) © 2026 郝沁雅
