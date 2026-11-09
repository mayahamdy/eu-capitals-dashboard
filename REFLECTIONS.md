# Reflections

## Before building anything
I would give weather a bit more weight than CO₂ for a holiday, but I would not ignore emissions completely. A trip is only good if it is comfortable and reasonably sustainable.

## Acquisition reliability
One batched API call is more reliable than 26 separate calls because there are fewer chances for timeout, throttling, or a partial failure. A single request is simpler and more stable for an automated workflow.

## Provenance
Before publishing it, I would check the factor against a trusted source such as a government or official emissions standard, and I would note the year and assumptions. I would also label it as an estimate, not the exact emissions of one specific flight.

## Relative vs. absolute
A city’s real temperature does not change, but its normalized KPI score can change when the comparison group changes. This shows the difference between a raw measurement and a KPI built for a specific set of cities.

## Predict, then check
I would predict Madrid because it seems to balance good weather with a moderate trip distance from Paris. The final score depends on both weather quality and CO₂, so a city with excellent weather but higher emissions may still lose.

## Was your prediction right?
My prediction was close to the real result: Madrid was still near the top. The 50/50 formula rewards a good balance, not just the best weather alone, which is why a very sunny but farther city can drop.

## Monitoring
The clearest signal is the “last updated” timestamp on the live page. If it is stale for too long, the data pipeline may have stopped or silently failed.

## The unguided step
I would change the origin coordinates and the exclusion logic in `scripts/fetch_and_score.py`, and I would also update any visible “from Paris” labels in the page. The best destination is not absolute; it depends on the starting city and the week’s data.
