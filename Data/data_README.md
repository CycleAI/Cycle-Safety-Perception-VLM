# Data

The public data files contain synthetic GPT votes and image-level rankings.
Raw human poll records, including participant UUIDs and voting times, are withheld.

| File | Content |
| --- | --- |
| `gpt52_votes_25k_20_06_26.csv` | 25,560 synthetic GPT-5.2 pairwise votes; user IDs in this file are synthetic and do not match poll participant IDs. |
| `human_trueskill_rankings_final_20_06_26.csv` | Aggregate human TrueSkill ranking for 17,246 images. |
| `gpt_trueskill_rankings_200k_20_06_26.csv` | GPT-5.2 ranking for 19,988 images, used as the main Stage 2 GPT prediction target. |

## Inputs not bundled

- Participant-level human votes. Notebooks reading these require authorized local access.
- The full extracted image-feature matrix, image metadata, raw imagery and full
  200k+ synthetic vote logs. Notebook 06 references
  `processed_features_merged_02_06_26.csv`, which is not included here.
- A combined 225k ranking is referenced in earlier documentation but is not
  included in this release.

No public archive link for the missing files is supplied. The available files
support inspection of rankings and saved results, but do not by themselves
reproduce every analysis. See [PUBLIC_RELEASE.md](../PUBLIC_RELEASE.md).
