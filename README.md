# OS-tips – Vinter-OS 2026 (starter v2)

## Ladda upp i GitHub
Ladda upp hela mappen (inkl. `data/`).

## Kör lokalt
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Deploy på Streamlit Community Cloud
New app -> välj repo -> `app.py`.

## Datafiler
- `data/athletes.csv` (athlete_id,name,sport,event)
- `data/results.csv` (athlete_id,medal)

I denna version är **varje gren en egen rad** i `athletes.csv`.
Det gör att ni kan tippa medalj per gren (inkl. stafetterna i längd).

## Lagring
Repo-mappen kan vara read-only i Streamlit Cloud, därför sparas tips/resultat i:
`~/.streamlit/os_tips_state/`
Använd fliken **Backup / Restore** för säkerhetskopia.
