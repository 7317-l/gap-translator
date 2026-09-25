# 贡献指南

欢迎补充你家的真实吐槽！

## 怎么加问题

编辑 `data/questions.json`，在对应分类下加：
- `elder_asks`：长辈问年轻人的问题
- `young_asks`：年轻人问长辈的问题

问题要具体、有场景感，不要假大空。

## 怎么加真实评论

编辑 `data/real_comments.json`，加一条：
```json
{
  "text": "评论内容",
  "platform": "抖音/小红书/微博",
  "likes": 123,
  "topic": "话题分类"
}
```

## 怎么加黑话

编辑 `data/slang.json`，加一个词条，记得写"explain_to_parents"。

## 怎么加代际特征

编辑 `data/personas.json`，完善对应年代的特征。
