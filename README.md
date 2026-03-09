# Data Preprocessing Pipeline – CSV Normalization Utility

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Category](https://img.shields.io/badge/Category-Data%20Engineering-purple)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

## Overview

This project demonstrates a lightweight CSV normalization tool designed to simulate a preprocessing stage in a data engineering pipeline.

It converts whitespace-separated structured datasets into properly formatted comma-delimited CSV files suitable for analytics ingestion.

The tool was tested using a subset of the UCI Bike Sharing dataset.

---

## Problem

Real-world datasets are often exported with inconsistent delimiters (spaces, tabs, mixed formatting).  
Downstream systems such as SQL databases, BI tools, and ML frameworks require strict comma-delimited CSV structure.

---

## Solution

This utility:

- Converts whitespace-separated data to comma-delimited CSV
- Preserves column structure
- Ensures consistent formatting
- Prepares structured datasets for ingestion into analytics systems

---

## Example Dataset

Dataset used: UCI Bike Sharing Dataset (subset)

### Raw Format (Whitespace-Separated)
1 1/1/2011 1 0 1 0 0 6 0 1 0.24 0.2879 0.81 0 3 13 16

### Cleaned Output (Comma-Delimited)
1,1/1/2011,1,0,1,0,0,6,0,1,0.24,0.2879,0.81,0,3,13,16

---

## Project Structure
python-csv-cleaner/
│
├── csv_cleaner.py
├── README.md
├── LICENSE
│
└── examples/
├── bike_raw_sample.csv
└── bike_cleaned_sample.csv

---

## How To Run

```bash
python csv_cleaner.py input_file.csv output_file.csv

```

## Use Case
This tool simulates the transformation layer in a simple ETL workflow:

Raw Dataset
↓
Normalization
↓
Ready for:

Pandas

SQL ingestion

Azure ML

Power BI

Analytics pipelines
