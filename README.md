# Extinction Risk ML

Machine learning prediction of animal threatened-status risk and
Data-Deficient reassessment prioritization from integrated IUCN
Red List and GBIF occurrence data.

## Associated Paper
Dhungana RC, Satyal D (2025). Machine learning prediction of animal
threatened-status risk and Data-Deficient reassessment prioritization
from integrated IUCN Red List and GBIF occurrence data.

## Key Results
- Primary model: LightGBM (selected through transparent benchmarking)
- Test PR-AUC = 0.635 (95% CI: 0.616–0.656)
- Test ROC-AUC = 0.858 (95% CI: 0.851–0.866)
- 95,898 animal taxa from IUCN Red List integrated with GBIF
- 16,293 Data-Deficient taxa scored for reassessment prioritization
- 10,497 taxa (64.4%) exceeded the F2-optimal triage threshold

## Repository Contents

| File | Description |
|------|-------------|
| `animal_extinction_risk_analysis.ipynb` | Full analysis notebook — data integration, feature engineering, model training, calibration, SHAP explainability, and Data-Deficient prioritization |

## Data
- IUCN Red List: https://www.iucnredlist.org
- GBIF occurrence data: https://www.gbif.org
- Model outputs archived at Zenodo: https://doi.org/10.5281/zenodo.20633953

## Requirements
See Cell 1 of the notebook for all required Python packages
(numpy, pandas, scikit-learn, lightgbm, xgboost, catboost, shap, cartopy).
