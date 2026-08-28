# Data

This folder contains the processed vote and ranking datasets needed to
reproduce the analyses in this study.

| File | Description |
|---|---|
| `human_votes_05_06_26.csv` | Raw human pairwise votes collected via the perception poll, before behaviour-based filtering. |
| `gpt52_votes_25k_final.csv` | GPT-5.2 synthetic votes on the 25,560-pair validated set, used for human-AI alignment analysis (Stage 1). |
| `human_trueskill_rankings_final_20_06_26.csv` | Final human TrueSkill safety score ranking, used as the human prediction target in Stage 2. |
| `gpt_trueskill_rankings_200k_20_06_26.csv` | GPT-5.2 TrueSkill ranking built from ~200,000 votes. **This is the ranking used as the GPT-5.2 prediction target in the paper's main Stage 2 results.** |
| `gpt_trueskill_rankings_final_20_06_26.csv` | GPT-5.2 TrueSkill ranking built from the combined 225k vote set (25k validated + 200k extended). Provided for completeness; not the ranking used in the paper's main reported results. |
| `metadata_images_mapping.csv` | Mapping between image filenames and sampled point locations. |

**Note:** two GPT-5.2 rankings are included above. The paper's headline
results (Section 4.2) use `gpt_trueskill_rankings_200k_20_06_26.csv`. See
Notebook 06 for the exact data loading configuration.

Larger datasets not included directly in this repository, including the full
extracted feature matrix (785 features × ~20,000 images) and the full raw
GPT-5.2 vote logs (200k+ votes), will be archived and made available via
Zenodo upon publication.
