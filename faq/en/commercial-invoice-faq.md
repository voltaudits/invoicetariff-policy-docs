# Commercial Invoice FAQ

> As of **2026-09-16**. If features change, the [invoice generator page](https://invoicetariff.com/en/invoice) is authoritative.
> 其他语言：[中文](../zh/commercial-invoice-faq.md)

## Basics

**Q: What is a commercial invoice, and how is it different from a regular invoice?**
A commercial invoice is the **core customs document for cross-border shipments**: customs uses it to assess the customs value and verify HTS codes and origin. It is not a tax invoice — its job is to tell customs plainly what the goods are, what they are worth, and where they were made.

**Q: When do I need one?**
International couriers (DHL/FedEx/UPS etc.) and freight forwarders normally require a commercial invoice with every shipment; since the [de minimis suspension](../../policy/en/02-de-minimis-suspension.md) on 2025-08-29, low-value parcels need a proper commercial invoice and accurate declarations too.

**Q: What must a commercial invoice include?**
The usual elements: seller and buyer details, invoice number and date, per-line description, **HTS code**, country of origin, quantity, unit price and total, currency, Incoterms (e.g. FOB / DDP), transport mode, and signature.

## Getting the details right

**Q: Do I declare the DDP price?**
**No.** U.S. customs value is the transaction value — in practice the **FOB / EXW price** of the goods; international freight and insurance are excluded when shown separately. Even on DDP terms you declare the goods value, and the duty is your cost (background: [how U.S. tariffs are calculated](../../policy/en/01-us-tariff-calculation.md)).

**Q: How should descriptions be written?**
State material and use; avoid bare "parts", "gift" or "sample". Description + HTS code + origin must agree — that is the baseline for smooth clearance. If the code is uncertain, verify it first in the [HTS code lookup](https://invoicetariff.com/en/hts).

**Q: Do free samples still need a declared value?**
Yes. Declare samples at their true value even when provided free; "no commercial value" no longer means duty-free — since the de minimis suspension, samples can attract duty too.

## Using the site's tools

**Q: How do I generate a compliant invoice quickly?**
Use the [commercial invoice generator](https://invoicetariff.com/en/invoice): enter seller/buyer details and line items (description + HTS + origin + amounts), and print or export the invoice as PDF. Form content is saved only in your own browser (localStorage) — **data never leaves your machine**.

**Q: Is there a ready-made template?**
Yes — the [commercial invoice template page](https://invoicetariff.com/en/commercial-invoice-template) has a template you can adopt directly, with filling instructions.

**Q: How does the invoice connect to tariff calculation?**
Before invoicing, price the duty for the same HTS code and origin in the [tariff calculator](https://invoicetariff.com/en), then set your FOB/DDP price with the duty folded in; for many SKUs, run the whole sheet through the [batch calculator](https://invoicetariff.com/en/batch).

---

**Go straight to**: [Commercial Invoice Generator](https://invoicetariff.com/en/invoice) · [Commercial Invoice Template](https://invoicetariff.com/en/commercial-invoice-template) · [Tariff Calculator](https://invoicetariff.com/en) · [SKU Batch Calculator](https://invoicetariff.com/en/batch)

> This document describes product features and general policy context — it is not customs or legal advice. Document requirements follow your carrier's and CBP's rules.
