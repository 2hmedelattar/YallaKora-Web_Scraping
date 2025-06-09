# 🏆 Football Match Scraper

This repository contains data scraped from an online source displaying recent football match results. The data is organized in a structured CSV file format and includes:

- Championship name
- Competing teams (Team A and Team B)
- Final match score
- Match time

---

## 📁 Files

| File Name     | Description                                      |
|---------------|--------------------------------------------------|
| `Scraper.csv` | Cleaned and structured football match data in CSV format |

---

## 🧾 CSV Format

The `Scraper.csv` file contains the following columns:

| Championship Name                 | Team A         | Team B         | Score  | Time  |
|----------------------------------|----------------|----------------|--------|-------|
| تصفيات كأس العالم - أمريكا الجنوبية | الأرجنتين       | البرازيل        | 4 - 1  | 02:00 |
| دوري القسم الثاني-أ               | القناة         | طنطا‏           | 0 - 1  | 21:30 |
| ...                              | ...            | ...            | ...    | ...   |

All text is encoded in UTF-8 to support Arabic content.

---

## 🚀 How the Data Was Collected

The data was scraped using **Python** with the following tools:

- `requests` – to fetch the web page
- `BeautifulSoup (bs4)` – for parsing HTML
- `csv` and `pandas` – to write and display data

The scraper extracts all match cards from the page, organizes the data, and saves it to `Scraper.csv`.

---

## 🧠 How to Use

If you'd like to use this data:

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git

import pandas as pd
df = pd.read_csv('Scraper.csv')
df.head()
