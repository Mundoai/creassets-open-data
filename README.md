# CRE Assets open data: syndication software pricing and a waterfall model

Free data and models for commercial real estate syndication, published by
[CRE Assets](https://creassets.com) under [CC BY 4.0](LICENSE).

| File | What it is | Page with context |
|---|---|---|
| [`syndication-software-pricing.csv`](syndication-software-pricing.csv) | What 9 sponsor/syndication software platforms publish about their prices, contract terms and migration fees, sourced row by row | [creassets.com/resources/syndication-software-pricing](https://creassets.com/resources/syndication-software-pricing) |
| [`creassets-real-estate-waterfall-model.xlsx`](creassets-real-estate-waterfall-model.xlsx) | A three-tier IRR-hurdle distribution waterfall in Excel with live formulas (return of capital and pref, then two GP promote tiers) | [creassets.com/tools/real-estate-waterfall-model-excel](https://creassets.com/tools/real-estate-waterfall-model-excel) |

**Disclosure:** CRE Assets sells software in the category this pricing dataset covers, so treat it as a
vendor's work. Every competitor value cites the vendor page it came from, so each row can be checked.

## Pricing dataset

Checked **2026-10-27**. One row per platform:

| Column | Meaning |
|---|---|
| `vendor` | Platform name |
| `website` | Vendor home page |
| `prices_published` | `Yes`, `Floor only`, `Tier names only` or `Not published` |
| `lowest_paid_plan_usd_per_month` | Lowest paid plan in USD per month, only when the vendor publishes it; empty otherwise |
| `price_as_published` | The price as the vendor states it; third-party estimates are labelled "third-party" |
| `pricing_basis` | How the price scales (per firm, per entity, by deals, by equity under management…) |
| `contract_terms` | Contract length and renewal, as stated |
| `migration_and_onboarding` | Migration or onboarding fees, as stated |
| `checked_on` | Date the row was last read from the vendor's site |
| `sources` | Space-separated source URLs |

**Method.** We read each vendor's own pricing, product and help pages and recorded what they list. Where a
vendor publishes nothing and a third party reports a figure, the text says "third-party" and the number
column stays empty. We never fill a blank with a guess.

**Updates.** The canonical, most recent copy is always at
<https://creassets.com/data/syndication-software-pricing.csv>. This repository is a versioned mirror;
outdated prices can be reported through an issue or at <https://creassets.com/contact> with the vendor's URL.

## Waterfall model

One workbook, two sheets: *Read me* explains the tiers and limits; *Waterfall* holds the inputs (yellow
cells), a ten-year timeline and the results (LP IRR, LP equity multiple, GP IRR, total promote and a check
row that must read $0 every year). Annual periods, all equity in at year 0, no GP catch-up. Opens in
Excel, Google Sheets, Numbers and LibreOffice. The example uses illustrative sample data only.

It is for illustration and education, not investment, legal or tax advice.

## How to cite

> CRE Assets (creassets.com), "Real estate syndication software pricing dataset", checked October 2, 2026.
> https://creassets.com/resources/syndication-software-pricing

GitHub's "Cite this repository" button reads [`CITATION.cff`](CITATION.cff).

## License

[Creative Commons Attribution 4.0 International](LICENSE) — reuse, adapt and redistribute with attribution.
