# Discussion Preparation Skill

一个面向中国留学生的 Codex skill：核对课程阅读材料，完整翻译学术英语，并基于原文准备 discussion 分析笔记。

它特别适合英语能力一般、阅读量较大，同时又不希望 AI 用“总结”代替原文翻译的学生。

## 它能做什么

- 先确认本周指定阅读清单，不擅自加入其他材料。
- 核对作者、版本、章节、印刷页码和 PDF 页码。
- 检查缺页、扫描质量、OCR 错误和跨页断句。
- 将指定范围完整翻译成自然中文，不总结、不删节。
- 保留重要英文人名、书名、引文和学术术语，方便回到原文定位。
- 用清晰中文解释难懂的 academic English 和概念。
- 在全部译文完成后，再制作摘要、术语表、文本比较和 discussion questions。
- 默认生成分析笔记，不生成需要背诵的“课堂发言稿”。

## 安装

将仓库中的 `skills/discussion-preparation` 文件夹复制到 Codex skills 目录：

```text
Windows: %USERPROFILE%\.codex\skills\discussion-preparation
macOS/Linux: ~/.codex/skills/discussion-preparation
```

重新打开 Codex 后，即可在提示词中调用：

```text
$discussion-preparation 帮我准备这周的 discussion。
```

第一次调用时，skill 会要求你确认课程主题、完整阅读清单、页码范围、文件位置和期望输出。提供材料并确认清单后，它才会开始处理。

## 推荐用法

```text
$discussion-preparation
课程：HIST 201，第 6 周
指定阅读：作者、标题、版本、章节、印刷页码
文件：附上的 PDF
输出：完整中文翻译、术语表、两道 discussion questions 的中英双语分析
```

如果你只需要翻译，可以明确写：

```text
只生成完整中文译文，不要摘要、讨论题答案或课堂发言稿。
```

## 工作原则

这个 skill 将“逐句翻译”理解为：原文的每一句话和每个重要细节都必须得到忠实呈现，而不是把译文机械地拆成一句一句编号。译文应保持自然段落和连续阅读体验。

如果材料缺页、无法辨认或版本不符，skill 会指出具体问题并等待补充，而不会凭记忆补写。它也不会绕过付费墙、登录限制或 DRM。请仅上传和处理你有权使用的课程材料；本仓库不包含任何课程阅读原文或译文。

## English overview

This Codex skill helps Chinese international students prepare for academic discussion sections. It verifies the assigned source set, produces complete Chinese translations without condensation, explains difficult academic English, and creates source-grounded analytical notes only after translation coverage is complete.

The skill preserves useful English names and terminology so students can locate evidence in the original reading. It defaults to analytical notes rather than ready-made classroom scripts.

## Plugin package

This repository is also packaged as a skills-only Codex plugin. The plugin manifest is in `.codex-plugin/plugin.json`, and the distributable ZIP is produced from the repository's plugin files without course readings or student work.

Public directory publication is subject to OpenAI review. Until the directory listing is approved, install the standalone skill from `skills/discussion-preparation`.

## License

MIT License. See [LICENSE](LICENSE).
