# Hop Teaming Analysis: Nashville Referral Network

A Streamlit multi-page app analyzing how primary care physicians (PCPs) refer patients to hospitals in the Nashville area, with community detection and referral network insights.

## Deployment (Streamlit Cloud)

1. Push this repository to GitHub.
2. Go to [share.streamlit.io](https://share.streamlit.io) and sign in.
3. Click **New app**, select your repo and branch.
4. Set **Main file path** to `Introduction.py`.
5. Click **Deploy**.

## Local Development

```bash
pip install -r requirements.txt
streamlit run Introduction.py
```

## Project Structure

```
├── Introduction.py          # Main/landing page
├── pages/
│   ├── 1_Community_Detection.py
│   ├── 2_Map.py
│   ├── 3_Analysis.py
│   └── 4_Conclusion.py
├── utils.py                 # Shared data loading & preprocessing
├── data/
│   └── hop_team_nashville.csv
├── images/
│   └── *.png / *.jpg
├── requirements.txt
└── .streamlit/
    └── config.toml
```

## Tech Stack

- **Streamlit** — app framework
- **PostgreSQL** — original data source
- **Neo4j** — graph database & Louvain community detection
- **Folium** — interactive maps
- **Plotly / Seaborn / Matplotlib** — visualizations

## Team (Nashville Software School)

- Grant Alan
- Abigail Ezell
- Shannon Lee
- Micheal Major
