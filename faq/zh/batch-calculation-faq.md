# 批量测算（SKU Batch Calculator）常见问题

> 信息截至 **2026-09-16**。功能与额度如有调整，以[批量测算页面](https://invoicetariff.com/zh/batch)为准。
> Other language: [English](../en/batch-calculation-faq.md)

[SKU 批量测算](https://invoicetariff.com/zh/batch)面向「整目录重算关税 / 结算到岸成本」的场景：上传 XLSX/CSV，整表逐行试算，导出带税费的结果表。以下是最常见的问题。

## 基本用法

**Q：一次能算多少行？**
单文件最多 **200 行**，超出部分不会被解析（可拆分文件后重试）；每日最多上传 **5 个文件**（浏览器本地计数，清除站点数据即重置）。额度不够用可以[加入 waitlist](https://invoicetariff.com/zh/api-waitlist) 获取更高额度。

**Q：模板有哪些列？**
模板列：**SKU、品名、HTS、申报价值 USD、净重 kg、数量、运费分摊 USD**。可在页面直接下载 CSV / XLSX 模板，按列填好即可。

**Q：支持什么进口国和运输方式？**
批量测算按「**进口国 = 美国**」全口径计算；运输方式（海运/空运）整票统一选择，影响 HMF 是否计收。

**Q：数据会被上传到服务器吗？**
不会。解析与计算**全部在浏览器完成，数据不出本机**——这是产品的设计原则，也是你敢把整份价目表丢进去算的原因。语言偏好等少量偏好数据仅存于浏览器 localStorage。

## 口径与结果

**Q：「整票口径」是什么意思？**
MPF/HMF 是按报关票数计收的规费，两种口径结果不同：

- **所有 SKU 同一票报关**：MPF/HMF 只收一次，按全部货值合计计算（拼票成本更低）；
- **每个 SKU 单独报关**：各行独立计 MPF（含每票最低 $33.58）。

结果页会明确标注所选口径，规费单列在合计行。

**Q：为什么有的行提示「HTS 未命中本地税则库」？**
该 8/10 位编码不在本地税则库中。先到 [HTS 编码查询](https://invoicetariff.com/zh/hts)确认编码是否正确，再修正表格重传。

**Q：为什么有的行提示「净重必填」？**
该编码的 MFN 税率为**从量税或复合税**（按千克计价），必须有净重才能算准。补齐净重列即可。

**Q：结果是什么口径的？**
结果为**估算**，并自带规则集版本号；异常行会在行内红字提示、可在线修正后重算。批量结果仅供参考，**不构成报关意见**——正式申报以报关行核算为准。

**Q：怎么导出结果？**
计算完成后可**导出 XLSX 结果表**，包含每行税费与单件落地成本，可直接用于成本核算与定价。

## 典型场景

- **政策变动后整目录重算**：例如 [De Minimis 暂停](../../policy/zh/02-de-minimis-suspension.md)、[全球 301 分层生效](../../policy/zh/05-global-section-301.md)后，把全量 SKU 丢进去重算一遍落地成本，再决定涨价与换源。
- **多国询价比价**：同一张表分别按中国、越南原产各算一次，对比实际税率差（原理见[对华 301](../../policy/zh/04-section-301-china.md) 与[全球 301](../../policy/zh/05-global-section-301.md)）。
- **整票 vs 分票的成本对比**：切换「整票口径」两种选项各算一次，比较 MPF/HMF 节省。

---

**直达工具**：[SKU 批量测算](https://invoicetariff.com/zh/batch) · [单票关税计算器](https://invoicetariff.com/zh) · [HTS 编码查询](https://invoicetariff.com/zh/hts) · [更高额度 / API waitlist](https://invoicetariff.com/zh/api-waitlist) · [订阅政策变更提醒](https://invoicetariff.com/zh/radar)

> 本文为产品功能说明与一般性解读，不构成报关或法律意见。
