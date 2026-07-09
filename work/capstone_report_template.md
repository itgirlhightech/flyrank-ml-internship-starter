# Capstone Report — <your lane>

- **Author:** Antonia Evilyn de Morais Feitosa
- **Lane:** Lane 2 - Refresh/Opportunity Scoring 
- **Repo:** https://github.com/itgirlhightech/flyrank-ml-internship-starter
- **Date:** 2026/07/09

> Copy this file to `work/capstone_report.md` and fill it in as you build. The eight
> sections mirror the Pass / Needs-Work rubric axes, so nothing here is optional.

## 1. Problem framing

There are thousands of pages and various metrics (CTR, position, content age, impressions, trend...). Analysing everything manualli is difficult. Data and Machine Learning can identify patterns and help prioritize which pages should be reviewed first.


## 2. Data safety

I used position_tier, ctr, content_age_days, and trend_direction for the exploratory analysis because they describe page performance and content characteristics relevant to the research question. I excluded content_id and client_id as features because they are pseudonymous identifiers and do not provide predictive information. I also considered the risk of data leakage: fields such as trend_direction and trend_pct may reveal information related to the target in a future predictive model, so they were only used for exploratory analysis and not as candidate features. Finally, I confirmed that no client-identifying information is included in the work/ directory.


## 3. Baseline

The baseline has not been built yet. As a first step, I performed exploratory analyses to understand the dataset and identify useful patterns. These observations will guide the design of a simple and transparent scoring rule that can later be compared with a machine learning model using the same evaluation metric.

## 4. Model / analysis

I will start with exploratory analysis to understand the relationships between the variables. Then I plan to build a simples scoring rule to prioritize pages before comparing it with a machine learning model.

## 5. Evaluation

Your split (grouped by client? time-aware?) and why. Metrics, model vs baseline **on the same
split**. What the errors look like — a short error analysis beats a big metric table.

## 6. Interpretation

What the model/clusters actually found. Feature importances or cluster profiles in plain
words. Surprises and negative results — a well-understood "no effect" is a valid result.

## 7. Recommendation

The initial results are based on exploratory data analysis and provide useful insights that will support the next stages of the project. The selected Lane aims to produce a practical ranking that helps prioritize which pages should be reviewed first. A FlyRank editor could use this ranking to focus on pages that are more likely to benefit from content updates instead of reviewing every page manually.

At this stage, my confidence is moderate because the conclusions are based on observed patterns rather than a trained machine learning model. The current analyses identify relationships in the data but do not establish causation. The ranking, features, and methodology may be refined as new analyses and models are developed throughout the following weeks.

## 8. Reproducibility

The exact commands to re-run everything from a fresh clone, your random seeds, and your
environment (`pip freeze` highlights or `requirements.txt` deltas).

---

> **Claims checklist before submitting:** observed / measured / directional / decision-support
> **Metrics vs. base rate:** report your task's base rate (majority-class %) next to any
> precision@K or accuracy — a high score can just be a high base rate. AUC / lift over
> baseline are the honest discrimination numbers.
> language everywhere · no causal claims without an experiment or causal design · no
> "predicted Google's algorithm" · no client-identifying details · numbers in this report
> match a fresh re-run.
