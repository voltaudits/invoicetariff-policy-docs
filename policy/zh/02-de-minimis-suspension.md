# 800 美元 De Minimis 免税额及其暂停

> 信息截至 **2026-10-05**。关税政策时效性强，最新变化请见 [关税雷达（变更日志 + 邮件提醒）](https://invoicetariff.com/zh/radar)。
> Other language: [English](../en/02-de-minimis-suspension.md)

## De Minimis 是什么

De Minimis（法律依据：19 U.S.C. § 1321，俗称「§321 免税」）曾允许**单票货值不超过 800 美元**的包裹免关税、免规费进入美国，且手续极简。它是直邮电商（Shein、Temu 模式）得以低成本直发美国消费者的核心通道。

## 现状：对所有国家暂停，且已无限期化

**自 2025-08-29 起，800 美元 De Minimis 免税额对所有国家和地区暂停适用。** 无论货物来自中国还是任何其他国家，低值包裹都要按正常关税栈缴税：MFN 基础税率 +适用的 301/232 等加征层级（层级相加、不复利的计算规则见[关税计算详解](01-us-tariff-calculation.md)）。

暂停的后续演进（截至 2026-10-05）：

- **2026-02-25**：总统公告确认对所有国家继续暂停（FR 2026-03829）——IEEPA 判决收尾时免税并未恢复。
- **2026-06-24**：暂停**无限期化**（FR 2026-12670，非邮政渠道当日生效；FR 2026-12669，邮政/邮件渠道 2026-07-24 生效，并启用新的邮政非正式报关流程）——目前**没有恢复时间表**。
- **司法审查进行中**：de minimis 相关问题已诉至国际贸易法院（*Axle of Dearborn, Inc. v. Department of Commerce*），法院在 IEEPA 退款命令中明确未处理 de minimis 问题（91 FR 63299）。判决前，**暂停照常执行**——按应税栈做成本计划。

对低值货物意味着三件事：

1. **不再有「免税直邮」**。$500 的包裹如果落在 7.5% + 12.5% 的栈里，就要按 20% 缴税，外加规费。
2. **合规义务下沉到小包裹**。原来可以不管 HTS 编码、不管原产国的卖家，现在必须逐单申报准确的编码与原产地——编码查错，整条税栈就错。
3. **邮路与非正式报关仍有特殊安排**。邮政渠道的非正式报关（≤ $2,500）缴纳固定规费而非从价 MPF，但关税本身照缴。

## 谁受影响最大

- **直邮电商卖家**：原本按「免税小包」定价的 SKU，到岸成本结构整个变了；不重算落地成本就可能在售价里倒贴关税。
- **小额样品/退换货**：寄回美国的替换件同样不再免税，发补发件前先算税。
- **消费者直购**：海外直购包裹可能被要求缴税后才能清关放行，体验上多一道「税到付」环节。

## 卖家现在应该做什么

1. **给每个 SKU 定准 HTS 编码**：用 [HTS 编码查询](https://invoicetariff.com/zh/hts)确认 8/10 位编码——这是税额的第一决定因素。
2. **按新规则重算落地成本**：用[关税计算器](https://invoicetariff.com/zh)或[落地成本计算器](https://invoicetariff.com/zh/landed-cost-calculator)把关税、MPF/HMF 摊进单件成本，再决定涨价或改物流方案。
3. **整目录批量重算**：SKU 多的卖家直接用 [SKU 批量测算](https://invoicetariff.com/zh/batch)上传 XLSX/CSV，一次算完整表（单文件 200 行，全部在浏览器本机完成）。
4. **订阅政策变化提醒**：De Minimis 相关规则仍在演进（如邮路细则），[关税雷达](https://invoicetariff.com/zh/radar)每 12 小时扫描官方来源、可邮件订阅提醒。

---

**相关文章**：[美国关税怎么算](01-us-tariff-calculation.md) · [对华 301 关税](04-section-301-china.md) · [全球 301 计划](05-global-section-301.md)

**相关工具**：[关税计算器](https://invoicetariff.com/zh) · [SKU 批量测算](https://invoicetariff.com/zh/batch) · [落地成本计算器](https://invoicetariff.com/zh/landed-cost-calculator) · [站内专题：De Minimis](https://invoicetariff.com/zh/de-minimis)

> 本文为一般性政策解读，仅供参考，不构成报关或法律意见。申报请以 HTSUS、Federal Register 与 CBP 指引为准。
