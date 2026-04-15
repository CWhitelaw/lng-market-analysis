# How the Ukraine War Rewired Global LNG Markets
An empirical analysis of the structural shift in U.S. LNG export flows following 
the Russian invasion of Ukraine, including a market structure case study of the 
Venture Global contract dispute.

## Key Findings
- U.S. LNG exports to Europe increased **268%** on a monthly aggregate basis 
  following the February 2022 invasion
- Pre-invasion monthly average: ~59,572 MMCF | Post-invasion: ~218,975 MMCF
- Germany received **zero** U.S. LNG imports before the invasion and took 
  **10 months** to receive its first meaningful cargo, constrained by a complete 
  absence of regasification infrastructure
- Spot LNG prices to Europe peaked at ~$17/MCF during 2022-2023, approximately 
  3x the pre-war baseline of ~$5-6/MCF
- The Venture Global arbitration reveals a structural flaw in long-term LNG 
  contracts: commissioning exemptions create legal incentives to withhold supply 
  during price spikes

## Project Structure
```
lng-market-analysis/
│
├── 01_us_lng_exports.ipynb              # U.S. LNG exports to Europe by destination
├── 02_pre_post_invasion_analysis.ipynb  # Pre/post invasion aggregate comparison
├── 03_germany_case_study.ipynb          # Germany: zero to major importer
├── 04_venture_global_lng_price_analysis.ipynb  # Price spike + contract dispute analysis
│
├── europe_lng_volumes.csv               # Monthly LNG export volumes by destination
├── europe_lng_prices.csv                # Monthly LNG export prices by destination
```

## Data Sources
- **U.S. Energy Information Administration (EIA)** — LNG export volumes and prices 
  by destination via the EIA Open Data API
- **Arbitration case research** — Venture Global dispute outcomes current as of 
  March 2026

## Setup & Usage
1. Clone this repository
2. Install dependencies: `pip install requests pandas matplotlib jupyter`
3. Get a free EIA API key at [eia.gov/opendata](https://www.eia.gov/opendata/)
4. In `01_us_lng_exports.ipynb`, replace `YOUR_EIA_API_KEY_HERE` with your key
5. Run notebooks in order — notebooks 02 through 04 load from saved CSV files 
   and do not require an API key

## Further Analysis
The following extensions are planned:
- **Seasonality-adjusted pre-invasion signal** — year-over-year volume change 
  analysis to isolate geopolitical risk pricing from winter heating demand in 
  late 2021
- **Asian market displacement analysis** — did the European demand surge divert 
  cargoes from traditional Asian buyers (Japan, South Korea, China)?
- **Interactive dashboard** — Plotly/Streamlit visualization of key findings

## Author
Callum Whitelaw  
B.A. Economics, University of Nevada, Reno (August 2026)  
[GitHub](https://github.com/CWhitelaw) | callumjwhitelaw@gmail.com
