# About the Dataset

> **Official Release Date:** June 1, 2026

## Overview
The MetroAT dataset is a newly introduced open-source benchmark dataset designed for research and development in data-driven maintenance of metro pneumatic systems. It comprises 105 variables and approximately 25 million observations collected continuously over a one-year period, capturing the operational behavior of multiple pneumatic system components.


## Dataset Structure

- **Collection Period:** June 2024 – June 2025  
- **Sampling Frequency:** 1 Hz  
- **Data Organization:** Files are structured hierarchically by year, month, and day for efficient storage and retrieval.
  
```text  
MetroAT/
├── 2024/
│   ├── 06/
│   │   ├── 01.parquet
│   │   ├── 02.parquet
│   │   ├── 03.parquet
│   │   └── ...
│   ├── 07/
│   │   ├── 01.parquet
│   │   ├── 02.parquet
│   │   ├── 03.parquet
│   │   └── ...
│   ├── 08/
│   │   ├── 01.parquet
│   │   ├── 02.parquet
│   │   └── ...
│   └── ...
│
├── 2025/
│   ├── 01/
│   │   ├── 01.parquet
│   │   ├── 02.parquet
│   │   ├── 03.parquet
│   │   └── ...
│   ├── 02/
│   │   ├── 01.parquet
│   │   ├── 02.parquet
│   │   └── ...
│   ├── 03/
│   │   └── ...
│   └── ...
```

## Variables

The dataset contains 105 variables, excluding timestamp-related fields (`timestamp`, `day`, `month`, and `year`), categorized as follows:

- **72 continuous sensor variables**
- **20 binary sensor variables**
- **7 operational state variables**
- **4 failure and maintenance variables**
- **2 aggregated sensor variables**

## Sample Data (Excerpt)

> The table below shows a simplified preview of the dataset. The full dataset contains 105 variables sampled at 1 Hz.

| timestamp           | TRAIN_FA | TRAIN_MA   | CW1_PNE | MW2_PRC | MW4_BRA | CW1_BRA | CW2_CON | MW4_SPR | MW3_SPR | MW4_PRC | MW1_SPR |
|--------------------|----------|-------------|--------:|--------:|--------:|--------:|--------:|--------:|--------:|--------:|--------:|
| 2025-04-05 01:58:08 | FALSCH   | No Failure  | 1 | 0,528198 | 0,002869 | 0,003723 | 0 | 0,515564 | 0,52533 | 0,515991 | 0,513733 |
| 2025-04-05 01:58:09 | FALSCH   | No Failure  | 1 | 0,528625 | 0,002869 | 0,003723 | 0 | 0,515991 | 0,524536 | 0,515991 | 0,51416  |
| 2025-04-05 01:58:10 | FALSCH   | No Failure  | 1 | 0,528992 | 0,002869 | 0,004089 | 0 | 0,516357 | 0,52533  | 0,518005 | 0,513733 |
| 2025-04-05 01:58:11 | FALSCH   | No Failure  | 1 | 0,527405 | 0,002869 | 0,003723 | 0 | 0,515137 | 0,524109 | 0,515991 | 0,513733 |
| 2025-04-05 01:58:12 | FALSCH   | No Failure  | 1 | 0,527771 | 0,002869 | 0,003723 | 0 | 0,514771 | 0,52533  | 0,516357 | 0,513733 |

