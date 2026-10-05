# HTS Code FAQ

> As of **2026-10-05**. Defer to the [HTS lookup page](https://invoicetariff.com/en/hts) and the official USITC tariff schedule.
> 其他语言：[中文](../zh/hts-code-faq.md)

## Basics

**Q: What is an HTS code?**
The Harmonized Tariff Schedule of the United States (HTS) classifies imported goods: the first 6 digits are the international HS code, refined at the U.S. level to **8 digits** (10 for statistical suffixes). The code is the first determinant of what you pay — it sets the MFN base rate and decides whether the item falls on the [China 301 lists](../../policy/en/04-section-301-china.md), a [global 301 tier](../../policy/en/05-global-section-301.md), a Section 232 scope, or an AD/CVD case.

**Q: How many digits do I report?**
Formal entries are filed to **10 digits** (8-digit rate line + 2-digit statistical suffix); for e-commerce and invoicing, at minimum lock in the correct 8 digits. One wrong digit can change the whole stack.

**Q: How do I find my code?**
Three paths:

1. Search by product/keyword in the [HTS code lookup](https://invoicetariff.com/en/hts) and open the code page to see rates and applicable layers;
2. Confirm step by step against the official USITC HTS;
3. When in doubt, check a customs ruling (CBP CROSS) or ask your broker — price the candidate codes on their code pages first, then let a professional make the call.

## Verification and mistakes

**Q: What does "verification status" on a code page mean?**
A [code page](https://invoicetariff.com/en/hts/61091000) lists every layer applying to the code (MFN, China 301, global 301, 232) with its rate, effective window and **Federal Register source**. Some exemption-list entries are published only as picture attachments and are still being transcribed — the page flags those explicitly, so you know which numbers are sourced and which are pending verification.

**Q: Why do specific/compound rates need net weight?**
Some MFN rates are priced per kilogram (e.g. rice at 2.1¢/kg) or compound ("percent + cents/kg", e.g. steel bolts at 9% + 0.5¢/kg). Without net weight they cannot be computed — the [batch calculator](https://invoicetariff.com/en/batch) flags such rows as "weight required".

**Q: What are the risks of a wrong code?**
Under-declaring: CBP recovers the duty plus penalties. Over-declaring: you simply overpay. And deliberately filing a high-rate code as a low-rate one is a violation — same enforcement lane as [transshipment origin washing](../../policy/en/05-global-section-301.md), which CBP actively pursues.

**Q: How do exclusions interact with the code?**
[Product exclusions](../../policy/en/04-section-301-china.md) are granted per 8/10-digit code: while valid (the current round of 178 runs through **2026-11-10**; a truce extension to 2027-01-10 has been announced, pending FR confirmation), the code enters without the China 301 layer — MFN, 232 and the global 301 tier still apply. Have your broker confirm each code's exclusion status before filing.

---

**Go straight to**: [HTS Code Lookup](https://invoicetariff.com/en/hts) · [Example code page](https://invoicetariff.com/en/hts/61091000) · [Tariff Calculator](https://invoicetariff.com/en) · [SKU Batch Calculator](https://invoicetariff.com/en/batch)

> This document describes product features and general policy context — it is not customs or legal advice. Classification follows the USITC tariff schedule and customs rulings.
