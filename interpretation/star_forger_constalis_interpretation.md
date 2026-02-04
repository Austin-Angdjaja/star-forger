# DISCLAIMER
The issue with the base Star Forger index is that it only provides us with the historical context of speculation. Markets, however, evolve. The market of today is vastly different from the market of 2020, and the market of 2020 is vastly different from the market of 1990. It is imperative then we anchor to the regime of today, and possibly even, the regime of tomorrow.

Constalis, then, for that purpose is not a signal generator, a predictor, or some pseudo-valuation tool. It is simply a n overlay of the Star Forger base index itself, that which allows us to examine speculation with more "up to date" context.

# LOGIC AND RATIONALE
Markets do not move in absolutes. They move in regimes. This is the core behind Constalis. Raw levels and historical prices are meaningless without context:
- Correlation reading is only alarming if it is extreme relative to itself.
- Speculative drawdown only matters if it is abnormal for that specific environment.
- Stress is subjective. Base "stress" levels differ between sectors and companies.

Most people make the mistake of looking at numbers in isolation and derive hallucinated meaning. Constalis exists precisely to solve this issue. It is not enough to consider the base Star Forger index's reading and related correlation measures. We need to anchor these findings to the current day market regime, which is what Constalis intends to do.

The premise is simple: behavior only starts mattering relative to its own historical context.

<img width="1742" height="748" alt="image" src="https://github.com/user-attachments/assets/8a58255d-95f9-44a6-b5a3-662af1693b55" />

# MECHANICS
A recap of Constalis' mechanics:
1. Fixed-length historical window is defined (90 days).
2. Within that window, values are ranked. Minima and maxima is established.
3. The current observation is expressed as a percentile ranking of past behavior.
4. The window rolls forward continuously, allowing regime change to manifest as information.

Constalis adapts to current regimes without fully rewriting history or anchoring to outdated baselines. Essentially, the system seeks to answer: "is what we are observing normal, elevated, or extreme?"

# INTERPRETATION
## PERCENTILE REGIMES
1. Low Percentiles (Normal / Benign)
   - Behavior is well within historical norms.
   - Speculation is functioning as expected.
   - Noise is dominant.
   - Systemic inference is not possible.
2. Middle Percentiles (Elevated / Watchful)
   - Behavior is becoming less common.
   - Stress or enthusiasm is building.
   - Context begins mattering.
   - Signals should be observed, not acted upon.
3. High Percentiles (Extreme / Constrained)
   - Behavior is rare historically.
   - Regime conditions dominate outcomes.
   - Probability distributions distorted.
   - Discretion dominates modeling.
## MEASUREMENTS
- Constalis at 1.00 indicates elevated levels of greed, relative to recent activity.
- Constalis at 0.00 indicates elevated levels of fear, relative to recent activity.
- Constalis at 0.50 indicates neutrality.
- Constalis plateauing at 1.00 for extended duration indicates maximum / euphoria levels of greed, relative to recent activity.
- Constalis plateauing at 0.00 for extended duration indicates maximum / euphoria levels of fear, relative to recent activity.
## ADDITIONAL NOTES
- Prima, Constalis, and the base Star Forger index is to be used in tandem.
- As always, Constalis is contextual; judgement is mandatory.
