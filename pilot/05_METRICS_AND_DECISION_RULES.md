# Credible value measurement
Manual private reports first. **Attribution** asks where a job came from; **incrementality** asks what would have happened without the service; **profit** asks what remains after relevant costs. A confirmed source does not prove the other two.

## Evidence tiers
| Tier | Example / required evidence | May claim | May not claim |
|---|---|---|---|
| Hard source attribution | Unique introduction and job IDs, recipient confirmation, redacted paid invoice/receipt | Verified referred collected revenue; verified job gross profit if costs supplied | All revenue is incremental; group caused all profit |
| Strong inference | Tagged reactivation/follow-up cohort, baseline, timing, preferably comparable untreated holdout | Tracked campaign revenue; estimated incremental contribution with method and limits | Causal lift from simple before/after alone |
| Weak attribution | Member says advice helped; total revenue rose | Member-reported benefit, clearly labeled | Financial ROI caused by membership |
| Unverified | Self-reported value without supporting evidence | Self-reported amount shown separately | "Verified" or causal return |

No app transforms weaker evidence into stronger evidence.

## Rules and arithmetic
- Separate pipeline, signed work, invoiced revenue and collected revenue. Do not add them together.
- Count each unique paid invoice/job once across referral, campaign and advice categories; retain multiple tags but one financial total.
- Record tax/pass-through exclusions and refunds consistently; correction log preserves original claim.
- Job gross profit = collected attributable revenue less corresponding direct delivery costs, when supplied. Contribution further deducts incremental selling/coordination costs as appropriate.
- Estimated net incremental benefit = estimated incremental contribution − dues − success fees − incremental participation/implementation costs. Include member time using their chosen rate or show it separately.
- ROI ratio only when inputs support it: (estimated incremental contribution − total program costs) / total program costs. Label assumptions and time horizon. If costs or incrementality unknown, show no causal ROI.
- Dues coverage ratio from verified referred contribution is descriptive, not necessarily causal. Never use revenue/dues as "profit ROI."
- A member's $10,000 referred revenue is not a $10,000 membership benefit. At 30% gross margin it yields $3,000 gross profit before additional costs; at 50% assumed incrementality only $1,500 is estimated incremental gross profit. If dues/fees/time total $900, illustrative net benefit = $600 and estimated ROI = 66.7%, still dependent on assumptions.
- No annualizing one good month into verified annual gain. Annualized scenarios go in a separate estimate box.
- For repeat deals under E, log relationship ID plus individual job/payment IDs and eligible fee window. Do not turn all future activity into attributable income by default.

## Manual member dashboard
| Field | Format / source | Required? |
|---|---|---|
| Reporting dates and dues paid | Actual payments | Required |
| Success fees paid/due/disputed | E ledger; separate from dues | Required in E |
| Referrals sent/received | Unique qualified accepted IDs and counts | Required |
| Referred pipeline | Count + optional provider estimate, clearly unpaid | Count required; value optional in A |
| Referred closed work | Signed jobs count; optional signed value | Count/status required |
| Referred collected revenue | Exact/range/self-report/verified marked separately | Optional in A; verifiable eligible basis required in E |
| Direct costs/gross profit | Private member-supplied evidence | Optional; no profit claims if absent |
| Campaigns/implementation completed | Asset/action and date | Required if exercise offered |
| Attributable campaign revenue | Deduplicated collected jobs with tier | Optional |
| Business improvements | Specific measured change or member-reported narrative | Optional |
| Active opportunities | Count, next step, stale-age | Required |
| Commitments completed | Completed / due | Required |
| Participation time | Self-reported hours, rate optional | Ask, don't force |
| Net benefit/ROI | Only when enough evidence; otherwise "not established" | Never fabricate |

Show one member's report to that member, not the whole group. Aggregate counts can be shared; exact prices, margins, customer data and future commercial plans stay private.

## Cohort health
Report distribution: number with no accepted introductions, no wins, and no reported useful benefit; median member result; source concentration; attendance; response adherence; paid renewal; missing-data rate; total operator hours. A large win for one provider cannot compensate statistically for seven dissatisfied members.

Commercial thresholds are in pilot/04; evidence semantics are defined here. Do not reclassify a pipeline opportunity as a useful financial outcome to pass a gate.
