# Proxy-Diskriminierung und Substitutionseffekt

Bachelorarbeit: SHAP-basierte Analyse von Proxy-Diskriminierung in Klassifikationsmodellen
(Folktables `ACSEmploymentFiltered`, Kalifornien 2018).

Die gesamte Analyse liegt in `bachelorarbeit_analyse.ipynb`.

## Ausführen

Voraussetzung: Python 3.12. Auf macOS zusätzlich `brew install libomp` (für XGBoost).

```bash
python3.12 -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab bachelorarbeit_analyse.ipynb
```

Im Notebook "Run All" ausführen. Beim ersten Lauf werden die ACS-Rohdaten (~65 MB)
automatisch von census.gov nach `data/` geladen; Details in Abschnitt 2.1 des Notebooks.
