network-intrusion-detection-analytics/
│
├── data/
│   ├── raw/              # Original CICIDS2017 CSV files (not committed — see .gitignore)
│   └── processed/        # Cleaned data ready for loading
│
├── src/
│   ├── extract.py        # Reads and consolidates raw CSVs
│   ├── transform.py       # Cleans data, handles nulls/infinities, engineers features
│   └── load.py            # Loads cleaned data into PostgreSQL
│
├── sql/
│   └── schema.sql          # DDL for fact and dimension tables
│
├── notebooks/
│   └── exploration.ipynb  # Initial data exploration and quality checks
│
├── dashboard/
│   └── network_intrusion_dashboard.pbix   # Power BI file
│
├── main.py                # Runs extract → transform → load in sequence
├── requirements.txt        # Python dependencies
├── .gitignore
└── README.md
