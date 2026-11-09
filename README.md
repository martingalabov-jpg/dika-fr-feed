# DiKa FR - Google Merchant Center feed

`feed.tsv` is rebuilt daily by GitHub Actions from DiKa's French catalogue CSV
(`images.dika.com/catalogues/5000/meta-pixel/general-fr.csv`) and fetched by Merchant Center (Dika.com, account 5889610493) from:

https://raw.githubusercontent.com/martingalabov-jpg/dika-fr-feed/main/feed.tsv

Changes vs. source: Google-format prices, `sale_price` only when lower than `price`, `internal_label` -> `custom_label_3`,
`gender` = female and `age_group` = adult (required for apparel in France), and per-item `shipping`
(15 EUR to France, free from 200 EUR, per dika.com/fr/terms/delivery; delivery 7-10 business days).
Run manually: Actions -> Update DiKa FR feed -> Run workflow.
