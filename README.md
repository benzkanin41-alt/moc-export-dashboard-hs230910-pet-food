# Thailand Export Monitor: อาหารสุนัขและแมว HS 230910

Static dashboard for Thailand export data from Thailand's Trade Statistic, Ministry of Commerce.

## Dashboard

- Product: อาหารสุนัขและแมว
- HS code used: `230910`
- HS source name: `230910 : อาหารสุนัขหรือแมว จัดทำขึ้นเพื่อการขายปลีก (เช่น ปลาบรรจุภาชนะอัดลม เป็นต้น)`
- Source page: https://tradereport.moc.go.th/th/stat/reporthscodeexport01
- API endpoint: https://tradereport.moc.go.th/stat/reporthscodeexport01/result
- Coverage: `2021-01` to `2026-04`
- Latest source month: `เม.ย. 2569`
- Currency: THB

## Validation

- Months fetched: `64`
- Country-month rows: `5,054`
- Reconciliation max value diff: `0.0`
- Reconciliation max quantity diff: `0.0`
- Missing continent mappings: `0`

The dashboard includes monthly, quarterly, and yearly views; total, country, and continent views; value and quantity metrics; MoM, QoQ, and YoY growth; clickable chart points; sortable tables; and CSV export from the current filtered table.

## Files

- `index.html`, `styles.css`, `app.js`, `data.js`: static dashboard runtime.
- `data/dataset.json`: full dashboard dataset.
- `data/monthly_country_hs230910.csv`: monthly country data.
- `data/monthly_continent_hs230910.csv`: monthly continent aggregates.
- `data/monthly_total_hs230910.csv`: monthly world totals.
- `data/validation_reconciliation.csv`: reconciliation output.
- `scripts/fetch_moc_hs230910.py`: reproducible MOC fetch script.
- `dashboard-smoke.png`, `dashboard-mobile-smoke.png`, `dashboard-mobile-full-smoke.png`: local QA screenshots.

## Local Run

```powershell
python -m http.server 8776 --bind 127.0.0.1
```

Then open:

```text
http://127.0.0.1:8776/
```
