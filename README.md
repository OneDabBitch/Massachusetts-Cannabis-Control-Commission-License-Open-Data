# Massachusetts Cannabis Control Commission — Self-Reported Licensee Data

This repository publishes the dataset catalog from the **Cannabis Control Commission (CCC) of Massachusetts** Open Data Platform. All information on the platform is **self-reported by licensees**.

- **Source:** https://masscannabiscontrol.com/open-data/data-catalog/
- **Publisher:** Commonwealth of Massachusetts, Cannabis Control Commission
- **Catalog captured:** 2026-11-12

Each dataset below is served directly by the Commission as CSV and as a JSON API endpoint. The files are not mirrored here; this repository is a machine-readable index pointing at the authoritative source. A `datasets.csv` manifest in this repo lists the same entries for programmatic use.

## Applications and Licenses

| Type | Dataset | CSV | JSON API |
| --- | --- | --- | --- |
| Adult Use | Marijuana Establishment License Application DBE Totals | [csv](https://masscannabiscontrol.com/resource/a_applications_dbe.csv) | [json](https://masscannabiscontrol.com/resource/a_applications_dbe.json) |
| Adult Use | Marijuana Establishment License Applications — Approved, Pending, Re-Opened | [csv](https://masscannabiscontrol.com/resource/l_applications_all_details.csv) | [json](https://masscannabiscontrol.com/resource/l_applications_all_details.json) |
| Adult Use | Total Adult-use Marijuana Establishment License Applications Submitted | [csv](https://masscannabiscontrol.com/resource/a_applications_all.csv) | [json](https://masscannabiscontrol.com/resource/a_applications_all.json) |
| Adult Use | Adult-Use Marijuana Establishment Licenses — Commence Ops | [csv](https://masscannabiscontrol.com/resource/l_licenses_commence_ops.csv) | [json](https://masscannabiscontrol.com/resource/l_licenses_commence_ops.json) |
| Medical | Medical Marijuana Establishments (MMEs) | [csv](https://masscannabiscontrol.com/resource/l_licenses_mtc.csv) | [json](https://masscannabiscontrol.com/resource/l_licenses_mtc.json) |
| Medical and Adult-Use | All Licenses / Licensing Tracker for Adult-Use and Medical Marijuana Establishments | [csv](https://masscannabiscontrol.com/resource/l_licenses_all_details_public.csv) | [json](https://masscannabiscontrol.com/resource/l_licenses_all_details_public.json) |

## Sales and Product Distribution

| Type | Dataset | CSV | JSON API |
| --- | --- | --- | --- |
| Adult Use | Marijuana Establishment Facility Sales and Statistics (by day and product type, 2018–current) | [csv](https://masscannabiscontrol.com/resource/a_sales_au_gross.csv) | [json](https://masscannabiscontrol.com/resource/a_sales_au_gross.json) |
| Adult Use | Marijuana Retail and Delivery Weekly Sales Report Total | [csv](https://masscannabiscontrol.com/resource/a_sales_au_deliveries.csv) | [json](https://masscannabiscontrol.com/resource/a_sales_au_deliveries.json) |
| Adult Use | Average Monthly Price per Ounce for Adult-Use Cannabis | [csv](https://masscannabiscontrol.com/resource/a_sales_au_price_per_gram.csv) | [json](https://masscannabiscontrol.com/resource/a_sales_au_price_per_gram.json) |
| Medical | Medical Marijuana Establishments (MMEs) — Facility Sales | [csv](https://masscannabiscontrol.com/resource/a_sales_mtc_gross.csv) | [json](https://masscannabiscontrol.com/resource/a_sales_mtc_gross.json) |
| Adult Use and Medical | Marijuana Establishment Adult-use and MMEs Plant Activity and Volume | [csv](https://masscannabiscontrol.com/resource/a_sales_au_activityvolume.csv) | [json](https://masscannabiscontrol.com/resource/a_sales_au_activityvolume.json) |

## Agent Registration and Ownership

| Type | Dataset | CSV | JSON API |
| --- | --- | --- | --- |
| Adult Use | Active Marijuana Establishment Agents Gender Totals | [csv](https://masscannabiscontrol.com/resource/a_agents_gender.csv) | [json](https://masscannabiscontrol.com/resource/a_agents_gender.json) |
| Adult Use | Marijuana Establishment Agent Race / Ethnicity Totals | [csv](https://masscannabiscontrol.com/resource/a_agents_raceethnicity.csv) | [json](https://masscannabiscontrol.com/resource/a_agents_raceethnicity.json) |

## Testing Results

Testing results are entered into Metrc by Independent Testing Laboratories. The Commission releases testing data on a six-month lag.

| Dataset | Dates included | CSV | JSON | Last updated |
| --- | --- | --- | --- | --- |
| Test results: THC, THCA, arsenic, cadmium, lead, mercury, total yeast and mold | 2025-01-01 – 2025-11-30 | [csv, 67 MB](https://masscannabiscontrol.com/resource/CCC_Testing_Results_2025.csv) | [json, 147 MB](https://masscannabiscontrol.com/resource/CCC_Testing_Results_2025.json) | 2026-03-19 |
| Test results: THC, THCA, microbials | 2024-01-01 – 2024-12-31 | [csv, 99 MB](https://masscannabiscontrol.com/resource/Testing_Results_2024_20260415_OpenData.csv) | [json, 269 MB](https://masscannabiscontrol.com/resource/Testing_Results_2024_20260415_OpenData.json) | 2026-04-15 |

A data clarification note for the 2025 file is published at https://masscannabiscontrol.com/2026/03/3-19-2026-testing-data-update/

## 2025 Industry Report files

Data files and the matching R processing scripts released alongside the Commission's industry report.

| File type | Title | Link |
| --- | --- | --- |
| Data | Adult Market Data, Including Counties | [csv](https://masscannabiscontrol.com/resource/Research-IndustryReport/20240513_adultMarketData_plus%20counties.csv) |
| Data | Marijuana Establishment Facility Sales and Statistics | [csv](https://masscannabiscontrol.com/resource/Research-IndustryReport/fren-z7jq.csv) |
| Data | Medical Treatment Centers — Facility Statistics | [csv](https://masscannabiscontrol.com/resource/Research-IndustryReport/g5mj-5pg3%20(11).csv) |
| Data | Average Monthly Price per Ounce for Adult-Use Cannabis | [csv](https://masscannabiscontrol.com/resource/Research-IndustryReport/rqtv-uenj.csv) |
| Data | Testing data: THC, THCA, yeast and mold, 2021–2023 | [csv](https://masscannabiscontrol.com/resource/Research-IndustryReport/Testing_Data_THC_THCA_Y&M-2021-2023.csv) |
| R Script | Adult-Use and Medical Establishments | [Rmd](https://masscannabiscontrol.com/resource/Research-IndustryReport/adultMedical_MEs_processing.Rmd) |
| R Script | Production | [Rmd](https://masscannabiscontrol.com/resource/Research-IndustryReport/facilitySales_processing.Rmd) |
| R Script | Medical-Use Market | [Rmd](https://masscannabiscontrol.com/resource/Research-IndustryReport/medical_market_data_processing.Rmd) |
| R Script | Price per Gram | [Rmd](https://masscannabiscontrol.com/resource/Research-IndustryReport/monthlyPrice_processing.Rmd) |
| R Script | Testing | [Rmd](https://masscannabiscontrol.com/resource/Research-IndustryReport/testing_processing.Rmd) |

## Using the JSON API

Every dataset has a `.json` endpoint that mirrors its CSV, so you can pull data without downloading files:

```bash
curl -s https://masscannabiscontrol.com/resource/l_licenses_all_details_public.json -o licenses.json
```

```python
import pandas as pd
url = "https://masscannabiscontrol.com/resource/a_sales_au_gross.csv"
sales = pd.read_csv(url)
```

## Important caveats

Data on the Open Data Platform is supplied by licensees themselves, not independently verified by the Commission. The Commission notes that it works toward completeness and accuracy but cannot guarantee it, that it is not responsible for licensee errors, and that it reserves the right to correct, remove, or amend published data. Each file carries its own "Last Updated" column, so check that column rather than assuming the capture date above. Always treat the Commission's site as the source of truth and re-pull before publishing analysis.

## Attribution and license

Datasets are published by the Commonwealth of Massachusetts Cannabis Control Commission as public open data. This repository adds only the index and documentation, and is not affiliated with or endorsed by the Commission. Please credit the Commission as the data source in any derived work.
# ma-ccc-licensee-open-data
Catalog of self-reported licensee datasets from the Massachusetts Cannabis Control Commission Open Data Platform
