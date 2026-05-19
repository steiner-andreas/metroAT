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

