# Cycling safety perception with vision-language models · Paper 1

Code, public data and figures for **Can a Vision-Language Model Approximate Human
Perceptions of Cycling Safety? Evidence from Pairwise London Streetscape Judgements**.
The accompanying research is submitted to *Accident Analysis and Prevention*.

The study compares GPT-5.2 and human pairwise judgements of London streetscapes,
builds image-level safety rankings with TrueSkill, and evaluates models that
predict perceived safety from visual features.

## Start here

| To explore… | Open… |
| --- | --- |
| Paper figures | [Outputs/](Outputs/README.md) |
| Public datasets and missing inputs | [Data/](Data/README.md) |
| Analysis sequence and notebook descriptions | [Notebooks/](Notebooks/README.md) |
| Human–AI agreement and TrueSkill ranking | [Notebook 04](Notebooks/04_stage1_trueskill_ranking_and_agreement.ipynb) |
| Main perceived-safety prediction models | [Notebook 06](Notebooks/06_stage2_prediction_models_main_results.ipynb) |
| Privacy and reproducibility boundary | [PUBLIC_RELEASE.md](PUBLIC_RELEASE.md) |

## Analysis workflow

1. **Synthetic voting and prompts:** notebooks 01–03.
2. **Ranking and human–AI agreement:** notebook 04.
3. **Visual features and prediction:** notebooks 05–06.
4. **Vote scaling, diagnostics and spatial maps:** notebooks 07–09.

These are analysis stages, not a complete one-command pipeline. Read the data
guide and each notebook's input configuration before running it. Some stages
require restricted or unbundled inputs, a suitable runtime and your own API access.

## Public data and reproducibility

The release contains 25,560 synthetic GPT votes, aggregate human TrueSkill
rankings for 17,246 images, GPT rankings for 19,988 images, nine notebooks and
the supplied paper figures. Raw participant-level human poll records are withheld
to preserve anonymity. The full feature matrix and several acquisition inputs
are not bundled. Notebook outputs and execution metadata have been cleared.

These scores describe **perceived cycling safety**. For injury severity conditional
on a recorded crash, see [Paper 2](https://github.com/CycleAI/London-Cyclist-Crash-Severity-Prediction).

## Citation and funding

A final bibliographic citation and DOI are not supplied in this repository.
Use the paper title above and record the repository commit for the code version
you used; update the citation when publication details are available.

This research was supported by the London School of Economics and Political
Science's inaugural Global Sustainability Research Fund.

[CycleAI research catalogue](https://github.com/CycleAI) · [Contribution guide](https://github.com/CycleAI/.github/blob/main/CONTRIBUTING.md)
