# btc-risk-off
Strategy Description: BTC risk-Off based on Equity and Credit market signals, and BTC trend.
This strategy dynamically reduces exposure to Bitcoin during periods of elevated macro risk, combining two types of signals:

Cross-Market Risk Signal (Equity-Based)
We use a composite model originally designed for the S&P 500, which combines:

Breadth indicators (e.g., Advance-Decline, New High–New Low, VIX z-score)
High-yield credit spread stress, detected via a Thomas Count-like approach
When this model flags a risk-off regime in equities, we interpret it as a signal to reduce exposure in BTC as well — reflecting the increasing correlation between crypto and traditional markets during periods of stress.

BTC Trend Signal
In parallel, we monitor a simple trend-following indicator on BTC itself (e.g., moving average slope or price below long-term average).
If the trend is negative, we also move to a defensive stance, regardless of equity market conditions.

The strategy enters risk-off mode if either:

The equity-based model turns risk-off
The BTC trend is negative
This dual-layer logic helps manage downside exposure while staying aligned with broader market conditions.
