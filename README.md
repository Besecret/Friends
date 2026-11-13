# Friends

一个私人日记仓库：记录每天的学习、工作与生活。

## 结构

```
日记/
├── 模板.md            # 日记模板
└── YYYY-MM-DD.md      # 一天一篇，按日期命名
```

## 怎么写

1. 复制 `日记/模板.md` 为 `日记/YYYY-MM-DD.md`
2. 按模板填写 —— 用不上的小节**整段删掉**，不用为了填满而硬凑内容
3. 提交并推送

```sh
git add 日记/YYYY-MM-DD.md
git commit -m "日记: YYYY-MM-DD"
git push
```

## 约定

- **文件名**：`YYYY-MM-DD.md`，一天一篇；同一天只保留一个文件
- **内容**：以真实记录为主，不修饰、不编造；只记得一句话就写一句话
- **提交信息**：`日记: YYYY-MM-DD`

## 常用

| 操作 | 命令 |
| --- | --- |
| 看最近写了什么 | `git log --oneline` |
| 看某天内容 | `cat 日记/2026-11-13.md` |
| 批量列出所有日记 | `ls 日记/` |

## 关于自动化

日常通过 [DeepSeek Harness](https://deepseek-harness.github.io/) 的 `diary` 技能完成：说一句「记日记」并给出当天内容，会自动按模板写入 `日记/YYYY-MM-DD.md`、提交并推送到本仓库。
