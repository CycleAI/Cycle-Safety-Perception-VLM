# Notebooks

Notebooks are numbered in the order they should be run. Each stage's
outputs feed into the next.

| Notebook | Description |
|---|---|
| `01_gpt_voting_25k_validated_set__nokeys.ipynb` | Collects GPT-5.2 synthetic votes on the 25,560-pair validated set, used for human-AI alignment analysis (Stage 1). |
| `02_gpt_voting_200k_extended_set_nokeys.ipynb` | Collects the additional ~200,000 GPT-5.2 votes used to build the extended safety ranking for Stage 2 prediction. |
| `03_prompt_configuration.ipynb` | Evaluates alternative prompt designs and documents the final prompt configuration used for GPT-5.2 voting. |
| `04_stage1_trueskill_ranking_and_agreement.ipynb` | Filters human votes, computes TrueSkill rankings for both sources, and evaluates human-AI agreement (Agreement Analyses A and B). |
| `05_feature_extraction_and_cleaning_nokeys.ipynb` | Extracts panoptic segmentation, object detection and image statistics features, and applies the cleaning pipeline (validation pass; full pipeline re-run in Notebook 06). |
| `06_stage2_prediction_models_main_results.ipynb` | Full feature cleaning and composite construction, Pearson filtering, and main cross-validated safety score prediction models (MLP, XGBoost, LightGBM, CatBoost), including SHAP feature importance. |
| `07_stage2_vote_scaling_analysis.ipynb` | Evaluates how prediction performance changes as the number of GPT-5.2 votes used to build the ranking increases. |
| `08_complementary_analysis_and_diagnostics_nokeys.ipynb` | Additional diagnostics and exploratory analysis supporting the main results. |
| `09_spatial_maps_and_borough_choropleth_nokeys.ipynb` | Generates spatial visualisations of perceived safety scores across London, including the borough-level choropleth map. |

## Requirements

See each notebook's first cell for required packages. Notebooks were run on
[Kaggle / your environment — specify].

## Note on credentials

Notebooks that access Azure Blob Storage or CARTO basemaps read credentials
from environment variables (`AZURE_CONN_STR`, `AZURE_OPENAI_API_KEY`,
`CARTO_API_KEY`). No credentials are stored in these files. You will need
your own credentials to re-run notebooks that fetch images or maps.
