# 🔄 Gap Translator · 代沟翻译机

> 不站队——不骂父母封建，也不骂孩子不懂事。只是两套操作系统不兼容，我们负责翻译。

## 这是什么

一个 AI 代际沟通工具。选个年代，把你想跟父母/孩子说但怕吵起来的话输进去，AI 帮你翻译成对方那代人能接受的版本。

灵感来自：
- [GenSync](https://arxiv.org/abs/2604.19276)（学术研究：AI 介导的代际语言翻译）
- 抖音/小红书评论区真实的代际沟通吐槽

## 为什么做这个

每次跟我妈打电话，说不到三句就吵起来。
不是不爱，是她说的我听不懂，我说的她觉得我在造反。
后来发现这不是我一个人的问题——抖音上"报喜不报忧"的视频有121万赞。

## 功能

- **双向翻译**：你可以帮孩子说话，也可以帮父母理解孩子
- **年代感知**：60后~10后，AI自动切换说话方式
- **问题库**：100+ 真实代际困惑，点一下就问
- **模拟对话**：选个家长类型（唠叨型/控制型/打击型/情绪型），AI 扮演你妈跟你练吵架
- **真实评论**：抖音小红书高赞评论，不是AI编的

## 项目结构

```
gap-translator/
├── data/
│   ├── personas.json       # 60后~10后人格设定
│   ├── slang.json          # 00后黑话词典（24个词）
│   ├── questions.json      # 代际问题种子库
│   └── real_comments.json  # 抖音/小红书真实高赞评论
├── prompts/
│   ├── translate.txt        # 翻译模式 prompt
│   ├── understand.txt       # 解释模式 prompt
│   ├── roleplay.txt         # 模拟对话 prompt
│   └── safety.txt           # 安全检测 prompt
└── index.html               # 极简 demo
```

## 快速开始

1. clone 本仓库
2. 打开 `index.html`
3. 在 JS 里填入你的 OpenAI 兼容 API Key
4. 开始翻译

## 数据说明

- `real_comments.json` 里的评论来自抖音、小红书公开评论区，已标注来源和点赞数
- `personas.json` 的代际特征基于公开调研和真实评论整理
- 欢迎 PR 补充更多真实问题和评论

## 参考文献

- [GenSync: Transparent AI-Mediated Language Support for Intergenerational Family Communication](https://arxiv.org/abs/2604.19276) - 研究发现：同时展示原文和翻译，比只给翻译效果好得多

## License

MIT
