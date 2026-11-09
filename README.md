# London Bike Safety: AI-Driven Cycling Safety Risk Mapping

Code and analysis for "Can a Vision-Language Model Approximate Human
Perceptions of Cycling Safety? Evidence from Pairwise London Streetscape
Judgements," submitted to *Accident Analysis and Prevention*.

This project evaluates whether GPT-5.2 can approximate human perceptions of
cycling safety from street-level imagery, using pairwise comparisons and
TrueSkill ranking, and uses the resulting safety scores to train predictive
models for city-scale cycling safety mapping across London.

## Repository structure

- [Notebooks/](Notebooks/notebooks_README.md) — the nine analysis notebooks, in run order. See
  [the notebook guide](Notebooks/notebooks_README.md) for a description of each.
- [Data/](Data/data_README.md) — processed vote and ranking datasets used in this study. See
  [the data guide](Data/data_README.md) for details and for what is not included here.
- [Outputs/](Outputs/) — final figures and tables as they appear in the paper.

## Public data and reproducibility

Raw participant-level poll votes are withheld to preserve participant anonymity.
The release retains aggregate human rankings, synthetic GPT votes, analysis code
and figures. Notebook outputs are cleared; some workflows require restricted or
unbundled inputs. See [the public release notes](PUBLIC_RELEASE.md).

## Citation

If you use this code or data, please cite:

[Full citation — insert once accepted/published]

## Funding

This research was supported by the London School of Economics and
Political Science's inaugural Global Sustainability Research Fund.
