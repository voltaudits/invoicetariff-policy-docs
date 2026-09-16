# 订阅与关税动态常见问题（关税雷达 / Waitlist / API）

> 信息截至 **2026-09-16**。以[关税雷达](https://invoicetariff.com/zh/radar)页面为准。
> Other language: [English](../en/subscription-updates-faq.md)

关税规则几乎是「月更」：301 排除窗口、全球 301 分层、232 新行业、MPF 年度调整……本页说明怎么**订阅变更提醒**、怎么跟进动态、以及怎么获得更高额度与 API。

## 关税雷达（Tariff Radar）

**Q：关税雷达是什么？**
[关税雷达](https://invoicetariff.com/zh/radar)是本站的关税变更追踪器：**每 12 小时扫描官方来源**（Federal Register、CBP、USTR 等），检测到变更立即在[变更日志](https://invoicetariff.com/zh/radar/changelog)发布增量记录，每条都带法源出处（如 FR 文号），与站内计算引擎的规则集同步。

**Q：能邮件订阅吗？怎么退订？**
能。在[雷达页面](https://invoicetariff.com/zh/radar)顶部的订阅卡片输入邮箱即可订阅变更提醒；每封提醒邮件底部都带退订链接，点击即退。

**Q：订阅要付费吗？会拿我邮箱做什么？**
免费。邮箱仅用于发送变更提醒（与[隐私政策](https://invoicetariff.com/zh/privacy)一致：不用追踪 cookie、不做广告画像）。

**Q：为什么要在意这些变更？**
税率与**报关日期**绑定：全球 301 于 2026-07-24 生效、232 药品关税 2026-09-29 启动、MPF 上下限 2026-10-01 调整、178 项对华排除 **2026-11-10 到期**——每一个都直接影响下一票的到岸成本（背景见[全球 301](../../policy/zh/05-global-section-301.md) 与[对华 301](../../policy/zh/04-section-301-china.md)）。

## Waitlist 与更高额度

**Q：批量测算的每日额度用完了怎么办？**
[批量测算](https://invoicetariff.com/zh/batch)限额为单文件 200 行、每日 5 个文件（浏览器本地计数）。额度不够时，在批量页或 [API waitlist 页](https://invoicetariff.com/zh/api-waitlist)留下邮箱，我们会按序开放更高额度。

**Q：waitlist 和雷达订阅是同一个名单吗？**
是同一套 waitlist 系统，但按「主题」区分：雷达页订阅的是「关税变更提醒」，API waitlist 页登记的是「更高批量额度 / API」意向，互不混淆，都可以随时退订。

## API

**Q：会提供 API 吗？**
在计划中。ERP / SaaS 把关税试算嵌进自家流程的需求已经在 waitlist 里收集——到 [API waitlist 页](https://invoicetariff.com/zh/api-waitlist)登记使用场景与规模，上线时会按登记顺序通知。

**Q：不想订阅，怎么自己盯变化？**
直接收藏[变更日志](https://invoicetariff.com/zh/radar/changelog)定期查看；或用 RSS（雷达提供 feed）。也可以先看本库的政策文章了解规则框架：[美国关税怎么算](../../policy/zh/01-us-tariff-calculation.md)。

---

**直达工具**：[关税雷达](https://invoicetariff.com/zh/radar) · [变更日志](https://invoicetariff.com/zh/radar/changelog) · [API / 更高额度 waitlist](https://invoicetariff.com/zh/api-waitlist) · [SKU 批量测算](https://invoicetariff.com/zh/batch)

> 本文为产品功能说明与一般性解读，不构成报关或法律意见。
