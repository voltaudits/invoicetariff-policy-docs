# 商业发票（Commercial Invoice）常见问题

> 信息截至 **2026-09-16**。如页面功能有更新，以[商业发票生成器](https://invoicetariff.com/zh/invoice)为准。
> Other language: [English](../en/commercial-invoice-faq.md)

## 基础问题

**Q：商业发票是什么？和普通发票有什么区别？**
商业发票（Commercial Invoice）是**跨境货物报关的核心单据**：海关据以核定完税价格、核对 HTS 编码与原产地。它不是税务发票——核心是让海关看得懂「这是什么货、值多少钱、哪里造的」。

**Q：什么时候需要商业发票？**
国际快递（DHL/FedEx/UPS 等）与货运代理通常要求随货附商业发票；自 2025-08-29 [De Minimis 免税额暂停](../../policy/zh/02-de-minimis-suspension.md)后，低值包裹同样需要规范的商业发票与准确申报。

**Q：商业发票必须包含哪些内容？**
常规要素：卖方与买方信息、发票号与日期、每行的品名、**HTS 编码**、原产国、数量、单价与总价、币种、贸易条款（Incoterms，如 FOB / DDP）、运输方式、签名。

## 填写要点

**Q：申报价值填 DDP 价格吗？**
**不。** 美国完税价格采用成交价格（transaction value），实务中即 **FOB / EXW 货值**——国际运费与保险单独列明时不计入。即使你按 DDP 报价，申报的仍是货物本身的价值，关税是你的成本（原理见[美国关税怎么算](../../policy/zh/01-us-tariff-calculation.md)）。

**Q：品名怎么写才合规？**
写清材质与用途，避免只写「parts」「gift」「sample」。品名 + HTS 编码 + 原产国三者对得上，是顺利清关的底线；编码拿不准就先用 [HTS 编码查询](https://invoicetariff.com/zh/hts)确认。

**Q：样品发货也要申报货值吗？**
要。样品按其真实货值申报（即使免费提供）；「no commercial value」已不再意味着免税——De Minimis 暂停后，样品同样可能产生关税。

## 用站内工具开发票

**Q：怎么快速生成一张合规发票？**
用[商业发票生成器](https://invoicetariff.com/zh/invoice)：填入卖方/买方、逐行品名 + HTS + 原产国 + 金额，即可生成可打印/导出 PDF 的商业发票。表单内容仅保存在你自己的浏览器（localStorage），**数据不出本机**。

**Q：有没有现成模板可以参考？**
有。[商业发票模板页](https://invoicetariff.com/zh/commercial-invoice-template)提供可直接套用的模板与填写说明。

**Q：发票和关税试算怎么衔接？**
开发票前先在[关税计算器](https://invoicetariff.com/zh)按同一 HTS 编码与原产国试算税费，把关税摊进报价再定 FOB/DDP 价格；SKU 多就直接用[批量测算](https://invoicetariff.com/zh/batch)整表算。

---

**直达工具**：[商业发票生成器](https://invoicetariff.com/zh/invoice) · [商业发票模板](https://invoicetariff.com/zh/commercial-invoice-template) · [关税计算器](https://invoicetariff.com/zh) · [SKU 批量测算](https://invoicetariff.com/zh/batch)

> 本文为产品功能说明与一般性解读，不构成报关或法律意见。单据要求以承运人与 CBP 规定为准。
