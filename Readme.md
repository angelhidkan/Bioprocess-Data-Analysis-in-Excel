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

## Key Insights

- **mAb_Y** was the most consistent product, with a 100 % pass rate.
- **mAb_X** and **mAb_Z** each had 2 out-of-specification batches (60 % pass rate).
- Failures were spread across four different parameters (Temperature, pH, Yield, Purity), each failing once. No single parameter was a systematic problem.
- **DO** and **Potency** stayed within specification in every batch.
- The two production lines performed similarly (75.0 % vs. 71.4 %).

## Author

**Angel HK**
