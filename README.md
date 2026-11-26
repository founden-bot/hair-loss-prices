# US hair loss treatment prices online

What US online clinics, pharmacies and stores charge for hair-loss treatment, one row per price: finasteride, minoxidil (topical and oral), finasteride and minoxidil formulas, dutasteride and spironolactone, at Hims, Keeps, Ro, Hers, Happy Head, Strut Health, Maximus, Lemonaid, Oak, RedBox Rx, Mark Cuban Cost Plus Drugs and others.

Every row is the provider's own price in its own words, read on the provider's own page (`source_url`) on the day in `checked_on`, by [HairLossCompare](https://hairlosscompare.com), a US price comparison site for hair-loss treatment. This file is a dated snapshot, also on Hugging Face (huggingface.co/datasets/hairlosscompare/hair-loss-prices). The current file is always at [hairlosscompare.com/data](https://hairlosscompare.com/data), where it is rebuilt from the same records as every price on the site.

## What a row holds

| Column | Meaning |
|---|---|
| `quote_id` | Stable id of the price (provider, product, plan length). |
| `product` | The product as the provider names it. |
| `ingredient` | The medicine: Finasteride, Minoxidil, Finasteride and minoxidil, Dutasteride, Spironolactone. |
| `brand` | The FDA-approved brand, when the price is for one. |
| `form` | `tablet` (a pill) or `topical` (on the scalp). |
| `seller` | The online clinic, pharmacy or store. |
| `seller_type` | Online clinic, compounded, pharmacy cash price or store. |
| `compounded` | `yes` for a compounded formula (not FDA-approved). |
| `price_kind` | What the price buys. |
| `membership_fee` | `none`, `separate`, or empty when the page does not say. |
| `advertised_price` | The price as published, with its period ("$22/month", "$120 for 3 months"). |
| `price_usd` | The advertised amount in US dollars. |
| `price_terms` | The provider's own words the price depends on. |
| `supply_days`, `upfront_months` | The supply the price buys and the months paid up front, when stated. |
| `cost_per_30_days_usd` | The price per 30 days, only where the supply is stated. |
| `checked_on` | The day (UTC) the price was read. |
| `review_status` | `current` within the review window, `overdue` after it. |
| `source_url` | The provider's own page the price was read on. |
| `referral_program` | `yes` when HairLossCompare may earn a referral fee from this provider. |
| `hairlosscompare_page` | The provider's page on HairLossCompare, with every price in context. |
| `notes` | Conditions, fees and caveats from the provider's terms. |

An empty cell means the provider's page does not state that fact. Nothing is estimated to fill it.

## Read it live

The same prices answer live, with no key:

- MCP server for AI assistants: `https://hairlosscompare.com/api/mcp` (streamable HTTP), tools `find_hair_loss_prices`, `find_provider_hair_loss_prices`, `list_hair_loss_medications`.
- Web API: `https://hairlosscompare.com/api/v1/prices?medication=finasteride`, described at `https://hairlosscompare.com/openapi.json`.

## Licence and citation

CC BY 4.0: reuse it, commercially too, naming HairLossCompare as the source with a link to https://hairlosscompare.com/data.

> HairLossCompare. US hair loss treatment prices online. https://hairlosscompare.com/data. Licensed under CC BY 4.0.

Dated snapshots with a DOI are archived on Zenodo: [10.5281/zenodo.24548073](https://doi.org/10.5281/zenodo.24548073) always resolves to the newest one.

Not medical advice. Every medicine here needs a prescription except over-the-counter minoxidil, and a compounded formula is not FDA-approved.
