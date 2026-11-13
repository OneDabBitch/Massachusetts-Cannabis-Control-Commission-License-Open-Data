# Manifest schema

This file documents the two machine-readable files in the repository: `datasets.csv` with one row per dataset and `fields.csv` with one row per column per dataset.

The Commission does not publish a data dictionary for the Open Data Platform. Column descriptions in `fields.csv` are inferred from the published headers and sample rows, so treat them as documentation of this index rather than as official Commission definitions. Column names, order and spelling are copied exactly from the source files.

## datasets.csv

UTF-8, comma delimited, header row required. Values are quoted only where they contain a comma.

| column | type | required | description |
| --- | --- | --- | --- |
| dataset_id | string | yes | Stable identifier taken from the Commission resource name without its extension. Join key to `fields.csv`. |
| category | string | yes | Catalog section as published by the Commission. |
| type | enum | yes | Normalized market segment used for filtering. One of `adult_use`, `medical`, `both`. |
| type_label | string | yes | The Commission wording for the segment preserved as published. |
| name | string | yes | Dataset title as published in the catalog. |
| column_count | integer | yes | Number of columns observed in the CSV header on the capture date. |
| source_last_updated | date | no | Last update reported by the source. Taken from the CCCLastUpdated value inside the file or from the catalog note for the testing files. ISO 8601. |
| csv_url | url | yes | Direct CSV endpoint at masscannabiscontrol.com. |
| json_url | url | yes | JSON endpoint mirroring the CSV. |

### type vocabulary

| type | source wording mapped into it | meaning |
| --- | --- | --- |
| adult_use | Adult Use | Adult-use establishments only |
| medical | Medical | Medical treatment centers only |
| both | Medical and Adult-Use, Adult Use and Medical, All | Covers both segments |

Example filter on the manifest: awk -F, '$3=="medical"' datasets.csv

## fields.csv

UTF-8, comma delimited, header row required. 415 rows covering the 15 datasets listed in `datasets.csv`.

| column | type | required | description |
| --- | --- | --- | --- |
| dataset_id | string | yes | Matches `dataset_id` in `datasets.csv`. |
| column_name | string | yes | Column header exactly as published including source spelling spacing and case. |
| position | integer | yes | One-based ordinal position of the column in the source header. |
| data_type | enum | yes | Inferred type. One of `string`, `integer`, `decimal`, `date`. |
| description | string | yes | Plain-language description inferred from the header and sample values. |

## Known quirks at the source

- CULTIVATION_ENVIRONMNET is misspelled in the Commission files and is documented with the source spelling.
- The catalog titles a_sales_au_price_per_gram as price per ounce while the resource name and the AVERAGERETAILPRICEPERGM column are per gram.
- l_licenses_commence_ops and l_licenses_mtc share an identical 86 column schema.
- The two testing files differ from each other. The 2024 file has 14 columns and the 2025 file has 8 with different capitalisation.
- Every recurring file carries its own CCCLastUpdated column. Prefer that value over source_last_updated in this repository.

## Maintenance

column_count and source_last_updated are a snapshot taken on 2026-11-12. The Commission can republish a file at any time, so re-read the headers before relying on either field. Treat masscannabiscontrol.com as the source of truth.
