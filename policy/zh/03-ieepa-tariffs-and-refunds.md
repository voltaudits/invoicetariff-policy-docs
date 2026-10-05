# IEEPA 关税终止与退税（CAPE 流程）

> 信息截至 **2026-10-05**。关税政策时效性强，最新变化请见 [关税雷达（变更日志 + 邮件提醒）](https://invoicetariff.com/zh/radar)。
> Other language: [English](../en/03-ieepa-tariffs-and-refunds.md)

## IEEPA 关税是什么

2025 年，美国政府依据《国际紧急经济权力法》（IEEPA）先后加征了两轮关税：

- **「芬太尼」关税**——以芬太尼问题为由对特定国家加征；
- **「对等关税」（reciprocal tariffs）**——按贸易伙伴分国别、分税率档加征。

两者在报关时通过 Chapter 99 税号 **9903.01 / 9903.02** 列报，与 MFN、301 等层级叠加。

## 2026-02-20：最高法院裁定违法

**2026 年 2 月 20 日，美国最高法院在 *Learning Resources, Inc. v. Trump* 案中裁定依 IEEPA 征收的全部关税违法**。CBP 对 IEEPA 层的评估至 **2026-02-24** 止，此后：

- 新报关**不再**适用 9903.01 / 9903.02 层级——这条税栈从新增报关中消失；
- **IEEPA 之外的其他关税完全不受影响**：对华 301（清单 1–4A）、2026-07-24 生效的[全球 301 计划](05-global-section-301.md)、232 条款、AD/CVD 照旧征收。

常见误读：以为「关税被推翻了 = 都不用交了」。实际上被推翻的只是 IEEPA 这一层；很多货物的 MFN + 301 + 232 负担依然存在，先算清楚再乐观。

## 谁可以退税

**2025-02-04 至 2026-02-24 期间**按 IEEPA 层级（9903.01 / 9903.02）缴纳的关税，可经 **CBP CAPE 流程**申请退还。这波退税量级史无前例——CBP 估算涉及约 **$1,660 亿**税款、**超过 5,300 万份** entry summary（91 FR 63299），为此专门开发了自动化退款工具（见下节）。

关键点：

- **退税只退 IEEPA 层**。同票货物里的 MFN、301、232、AD/CVD 以及 MPF/HMF 规费**不在退还范围**。
- 报关时是否列了 9903.01 / 9903.02 税号，是判断「缴没缴过 IEEPA 税」的直接依据——翻出报关单（entry summary，CBP 7501 表）逐行核对。
- 正式报关的进口商（importer of record）才是退税申请人；委托报关行的，由报关行协助发起。

## CAPE 是什么、怎么运作

**CAPE（Consolidated Administration and Processing of Entries）** 是 CBP 为处理这波退款专门开发的自动化工具，入口是 **ACE（Automated Commercial Environment）门户**：

- **CAPE Declaration 申报**：以 CSV 列出 entry summary 编号提交，**单份申报最多 9,999 票**；同一进口商的多份 entry summary 合并为一次提交、一笔退款，量大可分批多次提交。
- **提交资格**：只有 ACE 账户持有人能提交。委托报关行的，确认报关行已在你的 ACE 账户中被指定为 notify party。
- **退款走 ACH 直存**：款项直接打入 importer of record 的收款账户——CBP 原则上**不再签发纸质支票**（电子退款临时最终规则，91 FR 21）。ACE 未登记 ACH 收款账户的退款会被暂扣；确需支票的须书面申请豁免（frn-achrefundsupport@cbp.dhs.gov）。
- **计息与条目状态**：退款计息，CBP 按法院命令尽快发放。未结算（unliquidated）条目由法院命令直接按不含 IEEPA 税清算/重清算；已结算条目须走重清算窗口——7501 处于哪种状态决定路径与截止，站内估算工具会按条目状态给出对应提示。

## 操作步骤

1. **圈定时间段**：只核 2025-02-04 → 2026-02-24 之间的进口报关单。
2. **逐票找出 IEEPA 行**：在 7501 表上找 9903.01 / 9903.02 税号及其对应税额。
3. **经 ACE 提交 CAPE Declaration**：备好 entry summary 清单（CSV，单份 ≤9,999 票）、ACH 收款账户与 notify party 指定；走报关行的，确认由报关行代为提交并跟踪进度。
4. **留好凭证与时效**：退款计息、以清算为准，建议逐票登记申请日期与金额，跟踪到账。

估算你能退多少、核对资格与时效，用站内的 **[IEEPA 退税估算工具](https://invoicetariff.com/zh/ieepa-refund)**（免费、本机运算）。

## 之后还会变吗

退税机制仍在快速演进：2026-10-05 CBP 就「Court-Ordered Refunds under the IEEPA Worksheet」向 OMB 提交 PRA 延期复审（91 FR 63299，意见期至 2026-11-04），退款节奏与个案口径还可能有新变化——[关税雷达](https://invoicetariff.com/zh/radar)每 12 小时扫描官方来源，建议[订阅邮件提醒](https://invoicetariff.com/zh/radar)拿到第一手变更与 Federal Register 出处。

---

**相关文章**：[美国关税怎么算](01-us-tariff-calculation.md) · [对华 301 关税](04-section-301-china.md) · [全球 301 计划](05-global-section-301.md)

**相关工具**：[IEEPA 退税估算](https://invoicetariff.com/zh/ieepa-refund) · [关税计算器](https://invoicetariff.com/zh) · [订阅关税变更邮件提醒](https://invoicetariff.com/zh/radar)

> 本文为一般性政策解读，仅供参考，不构成报关或法律意见。退税资格与流程以 CBP 官方指引为准。
