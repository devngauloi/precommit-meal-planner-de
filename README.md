# Pre-registered kill criteria: family meal-planning app, Germany

Published before any of these tests runs. I will report each result as a new issue in this repository, and I will not edit this text; the commit history shows any change. If I change a threshold, I will say so publicly and explain why.

**Terms.** C is the ad spend per new paying user. ρ is C divided by lifetime net revenue per paying user. k is the share of annual subscribers who renew after year one.

| Test | Deadline | Pass | Fail, stop |
|---|---|---|---|
| E1: ask 3 small developers in this category for their real numbers | 2026-12-04 | At least one reports numbers giving ρ ≤ 0.5 | Someone replies and all replies give ρ > 1. No replies is "unknown", not a pass |
| E2: buy cold users in Germany with Meta and Apple Search Ads, up to €1,500 | 3 months after a working build | C ≤ €12.18 over the first 30 paying users | C > €30.64, or the €1,500 runs out before 30 paying users |
| E3: "from your own family's recipes" vs "save on groceries", inside E2 | Same as E2 | Own-recipes cost per payer ≤ 1× savings | Own-recipes cost per payer > 1.5× savings: the positioning is wrong |
| E4: refunds | 60 days after E2 | ≤ 5 % | > 10 % |
| E5: first-year renewal | 12 months after E2 | k ≥ 25 % | k < 10 % |

If E2 lands between pass and fail, I may run one more round of up to €1,500 with the same thresholds, within 2 months. I will not change the screens and re-measure to rescue a failed result. E3 with few payers is noisy, so I will report the interval and not only the point estimate.
