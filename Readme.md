# Bioprocess Data Analysis in Excel

An Excel workbook that simulates **Continued Process Verification (CPV)** for monoclonal antibody (mAb) production batches. Each batch is checked automatically against product-specific specification limits. The results are then summarized as KPIs and shown on a dashboard.

> **Disclaimer:** All batch data and specification limits are fictional and were created for training and portfolio purposes. They are not validated manufacturing specifications.

---

## Project Objective

In biopharmaceutical manufacturing, every batch must be checked against predefined limits for process conditions and quality attributes. The aim of this project was to build a simple, formula-driven tool that:

- Stores batch records in a structured table
- Flags each parameter as **PASS** or **FAIL** against its specification
- Gives every batch an **overall release status**
- Calculates KPIs by product, production line and parameter
- Shows batch performance on a dashboard that updates automatically

---

## Batch Data

Each batch record contains:

`Batch ID` · `Product` · `Production Line` · `Start Date` · `End Date` · `Shift` · `Temperature (°C)` · `pH` · `DO (% air saturation)` · `Yield (%)` · `Purity (%)` · `Potency (% relative activity)`

The data covers 15 batches across 3 products (5 batches each), 2 production lines (Line_A, Line_B) and 2 shifts (Day, Night).

---

## Results

### Overall

| KPI | Value |
|---|---|
| Total batches | 15 |
| Passing batches | 11 |
| Failing batches | 4 |
| Overall pass rate | 73.3 % |

### By Product

| Product | Total | Passing | Failing | Pass rate |
|---|---:|---:|---:|---:|
| mAb_X | 5 | 3 | 2 | 60.0 % |
| mAb_Y | 5 | 5 | 0 | 100.0 % |
| mAb_Z | 5 | 3 | 2 | 60.0 % |

### By Production Line

| Line | Total | Passing | Failing | Pass rate |
|---|---:|---:|---:|---:|
| Line_A | 8 | 6 | 2 | 75.0 % |
| Line_B | 7 | 5 | 2 | 71.4 % |

### Out-of-Specification Batches

| Batch | Product | Failed parameter |
|---|---|---|
| BATCH-006 | mAb_Z | Temperature |
| BATCH-010 | mAb_X | Purity |
| BATCH-013 | mAb_X | pH |
| BATCH-015 | mAb_Z | Yield |

### Average Results (all batches)

| Parameter | Average |
|---|---|
| Temperature | 36.9 °C |
| pH | 7.08 |
| DO | 45.9 % air saturation |
| Yield | 84.8 % |
| Purity | 95.9 % |
| Potency | 92.3 % relative activity |

## Key Insights

- **mAb_Y** was the most consistent product, with a 100 % pass rate.
- **mAb_X** and **mAb_Z** each had 2 out-of-specification batches (60 % pass rate).
- Failures were spread across four different parameters (Temperature, pH, Yield, Purity), each failing once. No single parameter was a systematic problem.
- **DO** and **Potency** stayed within specification in every batch.
- The two production lines performed similarly (75.0 % vs. 71.4 %).

## Author

**Angel HK**, biotechnology / bioprocess engineering student
