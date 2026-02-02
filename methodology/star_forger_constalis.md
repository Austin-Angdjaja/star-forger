# CORE LOGIC
Markets move in cycles — this is a well known fact. Perhaps a little lesser known fact is that market memory is short. People tend to forget historical context and anchor to the here and now — repeating otherwise obvious mistakes of the past. Exhibit A: the current silver rally. Twice, silver has made parabolic moves historically, and twice said parabolic moves have ended in a cascade of liquidation and margin calls.

Star Forger: Constalis exists to anchor speculation to its own history, not to narratives, headlines, or any such external benchmarks. Where:
- Star Forger measures whether speculation is supported.
- Prima measures whether speculation is failing systemically.

Constalis measures where current speculative behavior sits relative to its historical context. The premise is simple.
> Risk appetite is meaningful only with context.

A high level of speculation may be healthy or dangerous depending on where it occurs in the cycle.

# THE IMPORTANCE OF CONTEXT
Speculation itself does not exist in absolutes. A speculative index at elevated levels:
- May represent early-cycle risk-on appetite.
- May represent late-cycle crowding and exhaustion.

Without context, price strength is ambiguous at best. Constalis seeks to resolve said ambiguity by viewing the problem from a different lens altogether:
> Is current speculative behavior extreme relative to itself?

This simple change reframes risk appetite from binary to gradient.

# NORMALIZATION AS A INFORMATION
Constalis normalizes the Star Forger base index against its own historical behavior. This normalization essentially:
- Compresses long-term horizons into comparable scale.
- Removes reliance on a single, absolute price level.
- Allows regime identification independent of market growth, inflation, environment difference, and circumstance change.

Rather than a simple, "is speculation high right now?", Constalis asks:
- Is speculation historically elevated?
- Is it compressed?
- Is it reverting?
- Is it breaking normal bounds?

Reference and regime-awareness is key. 

Exhibit A: a sample snapshot of the Star Forger: Constalis index.

<img width="1919" height="937" alt="image" src="https://github.com/user-attachments/assets/71811b81-f45f-466c-86a6-2a4aabffb70a" />


# ROLLING WINDOWS, GLOBAL CONTEXTS
The Star Forger index itself operates within global contexts. It tracks the historical behavior of speculation itself, and this tracking dates back years. Constalis introduces a localized rolling context in addition to Star Forger's global historical framing. In essence, it localizes regime behavior and provides the operator with a more nuanced perspective on speculation. Constalis seeks to answer:
- Are we nearing upper / lower bounds of recent speculative behavior?
- Is risk appetite expanding / contracting relative to recent norms?
- Are we operating near historical extremes?
- Is the market repeating familiar speculative patterns?
- Are we still operating within expected assumptions?

This localization allows for more easy identification of regime shifts and transitional phases. Star Forger's global context provides us with historical context; Constalis provides us with context relevant today.

# MECHANICS
Whereas the base Star Forger index:
- Normalizes each speculative asset price.
- Weights constituents equally.
- Sums price changes into a single scalar time series.

Constalis, instead:
- Looks back 60 trading days.
- Identifies minimum Star Forger value in that window.
- Identifies maximum Star Forger value in that window.
- Linearly rescales the current value between those two bounds.
- Maps the results onto a -1 ~ +1 scale.
- Hard clips to prevent numerical blowups.

Furthermore, Constalis also alternatively makes some adjustments to the base index:
- Computes the mean of Star Forger.
- Compute the standard deviation.
- Z-score's the current value.
- Clip at ±3σ
- Normalizes results to -1 ~ +1, by dividing by 3.

In essence, Constalis' main purpose is to provide an alternative perspective into the base Star Forger index. Whereas Star Forger simply charts an equally-weighted basket of speculative asset's normalized price movements, Constalis provides a more "recent" view into the past 60 trading days. This provides us with insight into recent market behavior and allows for identifying short-term regime shifts. These two normalizations are maintained simultaneously to prevent local regime compression from being misinterpreted as the historical extremity.

The rolling window (local regime) answers: "Relative to **now**, is speculation high / low?"

The global context (structural regime) answers: "Relative to **history**, is speculation high / low?"

# DESIGN PHILOSOPHY
Constalis came to me when I realized Star Forger itself wasn't exactly useful on its own. It provides me with context as to what the market considers **historically** speculative or otherwise, but market conditions are never static. Regimes shift, circumstances change, environments update — I needed something to provide me with more relevant context. Constalis, in that regards, is the tool.

The tool was designed specifically to anchor speculation to its own history. Constalis does not exactly track macro, valuation, or narrative history per se. It tracks the behavioral history of speculative capital itself.
