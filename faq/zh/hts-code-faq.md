# HTS 编码常见问题

> 信息截至 **2026-09-16**。以[HTS 编码查询页](https://invoicetariff.com/zh/hts)与 USITC 官方税则为准。
> Other language: [English](../en/hts-code-faq.md)

## 基础问题

**Q：HTS 编码是什么？**
HTS（Harmonized Tariff Schedule of the United States）是美国进口货物的分类编码体系：前 6 位是国际通行的 HS 编码，美国层面细化到 **8 位**（统计口径到 **10 位**）。你缴多少关税，第一决定因素就是这个编码——它决定 MFN 基础税率，也决定是否落入[对华 301 清单](../../policy/zh/04-section-301-china.md)、[全球 301 分层](../../policy/zh/05-global-section-301.md)、232 范围或 AD/CVD 案件。

**Q：申报到几位数？**
正式报关一般报到 **10 位**（8 位税率 + 后 2 位统计后缀）；电商与发票场景至少要锁定正确的 8 位。编码错一位，税栈可能完全不同。

**Q：怎么找到我的编码？**
三种路径：

1. 用[HTS 编码查询](https://invoicetariff.com/zh/hts)按品名/关键词检索，点进编码页看税率与适用层级；
2. 对照 USITC 官方 HTS 税则逐级确认；
3. 拿不准时查海关裁定（CBP CROSS 数据库）或问报关行——先在编码页把候选编码的税率跑一遍，再让专业人士拍板。

## 核对与纠错

**Q：编码页上的「核实状态」是什么意思？**
[编码页](https://invoicetariff.com/zh/hts/61091000)列出该编码适用的每一层级（MFN、对华 301、全球 301、232）及其税率、生效窗口与 **Federal Register 来源**；部分豁免清单条目官方仅以图片附件公布、仍在转录核实的，页面会明确标注——这就是核实状态的意义：让你知道哪些数字有法源、哪些待核实。

**Q：为什么从量税/复合税还要填净重？**
部分 MFN 税率按千克计价（如大米 2.1¢/kg）或「百分比 + 千克」复合（如钢螺栓 9% + 0.5¢/kg）。没有净重就算不准——[批量测算](https://invoicetariff.com/zh/batch)遇到这类行会提示「净重必填」。

**Q：编码报错了有什么风险？**
少缴：海关追补税款 + 罚金；多缴：白交钱。另外，把高税率编码「故意报成」低税率编码属于违规行为，与[转口洗产地](../../policy/zh/05-global-section-301.md)一样是 CBP 重点执法对象。

**Q：301 排除怎么和编码配合用？**
[产品排除](../../policy/zh/04-section-301-china.md)是按 8/10 位编码豁免的：排除有效期内（现行 178 项至 **2026-11-10**），对应编码免掉对华 301 那一层，但 MFN、232、全球 301 档照常。报关前让报关行逐码确认排除状态。

---

**直达工具**：[HTS 编码查询](https://invoicetariff.com/zh/hts) · [编码示例页](https://invoicetariff.com/zh/hts/61091000) · [关税计算器](https://invoicetariff.com/zh) · [SKU 批量测算](https://invoicetariff.com/zh/batch)

> 本文为产品功能说明与一般性解读，不构成报关或法律意见。编码归类请以 USITC 税则与海关裁定为准。
