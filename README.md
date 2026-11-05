# 管理学综述写作 · Management Review Writing

一个面向 Codex 的中文 skill，帮助研究者完成管理学综述的选题定位、文献编码、证据综合、理论框架、研究议程、正文修改与质量评估。

它从 **13 篇中英文主题综述和 2 篇写作指南**中提炼论证方法：英文主题范文来自 UTD24 名单内期刊，中文来自《管理世界》《外国经济与管理》《南开管理评论》。每篇都有书目、来源链接、结构分析、可迁移规则和使用限制。

## 可以用来做什么

- 把宽泛主题收窄为可回答的综述问题，并说明相对已有综述的增量。
- 选择综述路线，设计纳排标准、编码字段和证据矩阵。
- 按概念、机制、过程或分析层次组织文献，处理矛盾与反例。
- 检查框架中的节点与箭头是否得到证据支持。
- 把研究缺口转成有机制、数据与设计的研究议程。
- 评估已有综述，并给出具体修订方案。

## 安装到 Codex

在 Codex 中调用自带的 skill-installer，并发送：

```text
请使用 $skill-installer，从 https://github.com/kyyf4z59y4-pixel/management-review-writing
安装 skills/management-review-writing。
```

也可以下载本仓库，将 `skills/management-review-writing` 文件夹复制到 `~/.codex/skills/`。如果同名 skill 已存在，先保留备份，再决定是否替换。安装后重启 Codex，再新建对话使用。

## 使用示例

```text
请使用 $management-review-writing。
我想写“生成式人工智能与员工创新”的独立综述。
目前只有初步文献清单，请先比较已有综述，提出 2–3 个可回答的问题，
说明各自的贡献目标、证据方法和整合主轴，不要直接编写研究结论。
```

```text
请使用 $management-review-writing，评估我上传的综述草稿。
重点检查概念边界、文献综合、框架的证据依据和研究议程。
请按“原文位置—问题—影响—修订建议”反馈。
```

```text
请使用 $management-review-writing，根据已经全文阅读的材料设计证据矩阵，
区分研究结果、作者解释和我的待检验推论，保留相反结果及方法差异。
```

## 内容结构

```text
skills/management-review-writing/
├── SKILL.md                        # 入口与核心工作流程
├── agents/openai.yaml              # Codex 显示名称与默认提示
└── references/
    ├── planning-and-synthesis.md   # 规划、编码、综合、框架与议程
    ├── writing-and-review.md       # 写作、审读与评价标准
    ├── exemplar-index.md          # 15 篇文献索引与使用边界
    └── exemplars/                  # 逐篇原创阅读分析
```

从 [SKILL.md](skills/management-review-writing/SKILL.md) 查看操作流程，从 [范文索引](skills/management-review-writing/references/exemplar-index.md) 查看完整书目。执行具体任务时按需读取相关笔记。

## 范文与评价原则

英文主题范文涉及代理理论、社会资本、知识管理、信息技术与战略优势、文化价值观、团队文化多样性；中文主题范文涉及创业学习、动态能力、价值共创、品牌意义、动态 QCA、机器学习与分类理论。

评价优先考虑理论贡献、文献综合、证据处理与表达。引用量、下载量、奖项和人大复印资料转载是辅助信号，需要记录来源、日期及口径。范文的期刊范围用于挑选学习材料；新研究的证据范围由研究问题和方法决定。

## 使用边界

- 本仓库包含原创写作分析、书目与稳定链接，不附论文原文、原始图表或数据库会话信息。
- 阅读综述全文不等于逐一核验其引用的全部原始研究；各篇笔记保留实际阅读范围和版本限制。
- 经典范文用于学习论证方式。新的主题事实、技术方法和期刊政策仍需更新检索与核验。
- skill 不会把“已下载”视为“已读”，也不允许虚构文献、筛选流程、效应量或因果证据。

文献整理日期：2026-11-05。

## English overview

A Codex skill for planning, synthesizing, writing, and reviewing management literature reviews. It includes original analyses of 13 review exemplars and two writing guides. Instructions and reading notes are primarily in Chinese; the workflow also supports English manuscripts. Original papers are not redistributed.
