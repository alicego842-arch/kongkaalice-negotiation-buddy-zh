# 控卡Alice·谈判专家（negotiation-buddy-zh）

作者：**控卡Alice（kongkaAlice）**  
版本：0.2.1  
Skill 名称：`negotiation-buddy-zh`  
命名空间：`kongkaalice/negotiation-buddy-zh`

一个中文的谈判参谋和陪练 Agent Skill，帮你处理工作和生活里需要谈条件、又不好开口的事：领导临时加活、谈薪、房东扣押金、甲方拖款、亲戚借钱、合租分账、网购维权、不知道怎么拒绝别人。

## 仓库地址（完整，可复制）

https://github.com/alicego842-arch/negotiation-buddy-zh

GitHub 标准短路径（owner/repo）：

```
alicego842-arch/negotiation-buddy-zh
```

ZIP 下载：

https://github.com/alicego842-arch/negotiation-buddy-zh/archive/refs/heads/main.zip

## 一键安装（推荐）

本仓库遵循 Agent Skills 标准目录：`skills/kongkaalice/negotiation-buddy-zh/SKILL.md`。

用 GitHub CLI：

```bash
gh skill install alicego842-arch/negotiation-buddy-zh kongkaalice/negotiation-buddy-zh
```

或安装本仓库全部 skill：

```bash
gh skill install alicego842-arch/negotiation-buddy-zh --all
```

预览：

```bash
gh skill preview alicego842-arch/negotiation-buddy-zh
```

## 手动安装

把目录 `skills/kongkaalice/negotiation-buddy-zh/` 整夹复制到你所用工具的 skills 目录（例如 `.agents/skills/negotiation-buddy-zh/`），保持文件夹内 `SKILL.md` 与 `references/` 相对位置不变。

## 给谁用

| 你是谁 | 你可能卡在哪 |
|---|---|
| 刚工作几年的上班族 | 被加活不敢说，谈薪不知道怎么开口 |
| 租房的人 | 退押金、修东西、涨房租，和房东、中介反复沟通没结果 |
| 接单的自由职业者 | 尾款拖着不给，需求一点点加 |
| 不好意思拒绝的人 | 借钱、帮忙、人情，不想答应，又不知道怎么拒绝 |
| 消费者 | 网购退货、预付卡退款被拖 |

## 适用场景

按关系分六类：职场与工作、租房与居住、钱与生意、消费维权、亲友与人情、日常拒绝与边界。

## 不适用 / 边界

不做的事：送礼行贿、违法违纪、PUA 与情感操控、主动教人使阴招、替你发消息。劳动仲裁、诉讼、人身安全等建议走专业渠道。

## 四种用法

1. 出主意  
2. 陪练加复盘  
3. 改消息  
4. 急用版  

默认中国大陆语境，回复用口语，不露谈判术语。

## 目录

```
skills/kongkaalice/negotiation-buddy-zh/
  SKILL.md
  references/knowledge-base.md
  tests/scenarios.md
LICENSE
README.md
```

## 来源与致谢

- 谈判思路参考罗杰·道森《优势谈判》（迩东晨译，北京联合出版公司，2022，ISBN 9787559657091）。本项目是非官方的学习整理，不含书中原文。
- 陪练与复盘做法参考了 https://github.com/bh52/voss 的思路。
- README 结构参考了 https://github.com/Ssupercoder/Salary-Negotiation-Skill 。

Copyright (c) 2026 kongkaAlice · MIT License
