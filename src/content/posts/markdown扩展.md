---
title: Markdown 扩展功能
published: 2024-05-01
updated: 2024-11-29
description: '阅读更多关于 Fuwari 中的 Markdown 功能'
image: ''
tags: [Demo, Example, Markdown, Fuwari]
category: 'Examples'
draft: false 
---

## GitHub仓库卡片

你可以添加链接到 GitHub 仓库的动态卡片，在页面加载时，仓库信息会从 GitHub API 拉取。 

::github{repo="Fabrizz/MMM-OnSpotify"}

使用代码`::github{repo="<owner>/<repo>"}`创建GitHub仓库卡片。

```markdown
::github{repo="saicaca/fuwari"}
```

## 警告框

支持以下类型的警告框：`note` `tip` `important` `warning` `caution`

:::note
突出显示即使用户略读也应考虑的信息。
:::

:::tip
帮助用户更成功的可选信息。
:::

:::important
用户成功所必需的关键信息
:::

:::warning
由于潜在风险，需要用户立即关注的关键内容。
:::

:::caution
行动的潜在负面后果。
:::

### 基本语法

```markdown
:::note
突出显示即使用户略读也应考虑的信息。
:::

:::tip
帮助用户更成功的可选信息。
:::
```

### 自定义标题

警告框的标题可以自定义。

:::note[这是标题]
这是一个带有自定义标题的注释。
:::

```markdown
:::note[这是标题]
这是一个带有自定义标题的注释。
:::
```

### GitHub 语法

> [!TIP]
> [GitHub语法](https://github.com/orgs/community/discussions/16925)同样支持

```
> [!NOTE]
> GitBub语法同样支持

> [!TIP]
> GitBub语法同样支持
```

### 剧透

你可以向文本中添加剧透。文本也支持 Markdown 语法。

这个内容 :spoiler[是隐藏的！**嘻嘻**]!

```markdown
这个内容 :spoiler[是隐藏的！**嘻嘻**]!

```