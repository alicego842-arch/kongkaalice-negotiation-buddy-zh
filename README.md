# 谈判专家 negotiation-buddy-zh

一个中文的谈判参谋和陪练 skill，帮你处理工作和生活里需要谈条件、又不好开口的事：领导临时加活、谈薪、房东扣押金、甲方拖款、亲戚借钱、合租分账、网购维权、不知道怎么拒绝别人。

作者：kongkaAlice
版本：0.2.1

## 给谁用

| 你是谁 | 你可能卡在哪 |
|---|---|
| 刚工作几年的上班族 | 被加活不敢说，谈薪不知道怎么开口 |
| 租房的人 | 退押金、修东西、涨房租，和房东、中介反复沟通没结果 |
| 接单的自由职业者 | 尾款拖着不给，需求一点点加 |
| 不好意思拒绝的人 | 借钱、帮忙、人情，不想答应，又不知道怎么拒绝 |
| 消费者 | 网购退货、预付卡退款被拖 |

## 适用场景

本 skill 处理日常生活和工作里需要跟人谈条件、争取利益或守住边界的事，按关系分六类：

| 类别 | 谁跟谁 | 常见矛盾 |
|---|---|---|
| 职场与工作 | 员工与上级、同事、跨部门协作方、人事部门 | 工作量分配、范围加码、功劳归属、责任推诿、薪酬待遇、调岗转岗 |
| 租房与居住 | 租客与房东、中介、物业、室友、邻居 | 押金退还、损耗认定、维修责任、费用分摊、租金调整 |
| 钱与生意 | 自由职业者、小商家与客户、合作方、供应商 | 报价定价、付款拖延、需求加码、验收标准、口头承诺不兑现 |
| 消费维权 | 消费者与商家、平台、服务机构 | 退换货、质量争议、预付费退款、未经同意的扣费、处理拖延 |
| 亲友与人情 | 自己与家人、亲戚、朋友、伴侣 | 借钱还钱、人情往来、开销与家务分担、期望落差、边界被越过 |
| 日常拒绝与边界 | 自己与反复提要求的熟人或同事 | 难以开口拒绝、请求一再升级、时间被占用、帮忙被当成义务 |

## 不适用 / 边界

不做的事：
- 送礼、行贿、走关系。
- 违法违纪的事。
- PUA 和任何形式的情感操控。
- 主动教人对别人使阴招。对方的手段只帮你识别和应对。
- 替你发消息。要发给别人的话只给草稿，发不发由你决定。

需要专业渠道的事：劳动仲裁、合同纠纷、诉讼、人身安全受到威胁，会建议你找律师、工会或走正规途径，不建议自己硬谈。长期焦虑、抑郁等心理困扰不在范围内，建议找专业心理咨询。

其他说明：
- 不提供法律意见。涉及地方规定时，只引用政府部门发布的官方原文并附链接；查不到会直说，并提示你去当地政府网站核对。
- 情感关系只处理三件事：把需求说清楚，判断对方是否在逐步加码、空头许诺或拖延，以及家务、开销、时间这类具体事务怎么谈。关系该不该继续，由你自己判断。

## 第一次用怎么开口

直接说清你想谈的事、对方是谁、你想要的结果，有聊天记录就贴原话或截图。不确定从哪开始，可以先问它能做什么，它会介绍能帮的几类事和四种用法。

## 它能做什么

1. **出主意**：先帮你把事情讲清楚，一次最多问三个问题，每个带例子；然后第一句就给明确结论（比如先找谁），再给能直接说出口或复制发送的话，以及对方答应、拖着、拒绝时各怎么接。你补充新顾虑时，它会先说结论变不变。
2. **陪练加复盘**：它扮演对方，心里藏着对方的底线，跟你一句一句过招。你说「暂停」就出戏复盘：这轮拿到什么、漏了什么，按轮次点评，给下次照念的话，最后揭开对方的底牌让你看差距。
3. **改消息**：把要发的微信贴进来，它给你改成强一点和软一点两版，并提醒文字沟通的规矩。
4. **急用版**：对方在等你回话时，只给一句准话和一句马上能发的话。

默认中国大陆语境，回复用口语，不用谈判术语。

## 安装

这是一个标准的 Agent Skill 文件夹，核心是 `SKILL.md`，知识库在 `references/` 里。

- 把整个文件夹放进你所用工具的 skills 目录即可。Claude Code、Cursor 等支持 Agent Skills 的工具，具体目录位置请看各自的官方文档。
- 保持文件夹结构不变，`SKILL.md` 会按相对路径读取 `references/knowledge-base.md`。
- 放好后，跟助手说「用谈判专家帮我看看这件事」或者直接描述你的处境，助手会自动调用本 skill。

## 目录

```
SKILL.md                    skill 本体
references/knowledge-base.md 谈判思路知识库（学习整理稿）
tests/scenarios.md          改完 skill 后自测用的场景
LICENSE
```

## 来源与致谢

- 谈判思路参考罗杰·道森《优势谈判》（迩东晨译，北京联合出版公司，2022，ISBN 9787559657091）。本项目是非官方的学习整理，不含书中原文，书的版权归原作者与出版方。
- 陪练与复盘的做法参考了 https://github.com/bh52/voss 的思路。
- README 结构参考了 https://github.com/Ssupercoder/Salary-Negotiation-Skill 。
- 国内场景、提问方式、复盘格式、红线等内容由作者结合自己的使用经验整理编写。

## 协议

本项目自己编写的部分以 MIT 协议发布，见 `LICENSE`。参考书的内容与版权归原作者与出版方所有。

---

## English

**negotiation-buddy-zh** is a Chinese-language Agent Skill that helps with everyday negotiations in a mainland-China context, in six areas: work and the workplace (workload, credit, pay, internal transfers), renting and housing (deposits, repairs, shared costs, neighbors), money and small business (pricing, late payments, scope creep), consumer rights (returns, prepaid-card refunds, unauthorized charges), family and friends (lending money, favors, shared expenses), and everyday refusals and boundaries. It has four modes: advice, role-play practice with a structured debrief, rewriting a chat message, and a quick-reply mode for urgent moments. It will not teach bribery, manipulation, or anything illegal. Ideas are partly drawn from Roger Dawson's *Secrets of Power Negotiating*; this is an unofficial study summary that contains no text from the book. Licensed under MIT.
