# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-11-12 06:37 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-11-11, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Thu 12 Nov | d+1 | 131.7 | 95.3 to 182.0 | 142.5 | 207 | Very Unhealthy | drizzle, 15 to 25C |
| Fri 13 Nov | d+2 | 131.4 | 89.2 to 193.4 | 142.0 | 207 | Very Unhealthy | drizzle, 17 to 27C, 2mm |
| Sat 14 Nov | d+3 | 131.2 | 88.1 to 195.5 | 141.8 | 207 | Very Unhealthy | cloudy, 14 to 27C |
| Sun 15 Nov | d+4 | 131.1 | 87.3 to 196.9 | 141.6 | 207 | Very Unhealthy | drizzle, 12 to 24C |
| Mon 16 Nov | d+5 | 131.1 | 86.7 to 198.1 | 141.5 | 206 | Very Unhealthy | clear, 9 to 23C |
| Tue 17 Nov | d+6 | 131.0 | 86.6 to 198.4 | 141.5 | 206 | Very Unhealthy | cloudy, 10 to 23C |
| Wed 18 Nov | d+7 | 131.0 | 86.0 to 199.6 | 141.4 | 206 | Very Unhealthy | clear, 10 to 23C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 79 | 13% | 17% | -8% | 90% | 70% | 99% |
| d+2 | 78 | 17% | 20% | -11% | 83% | 68% | 99% |
| d+3 | 77 | 19% | 22% | -12% | 82% | 70% | 99% |
| d+4 | 76 | 18% | 23% | -14% | 79% | 68% | 99% |
| d+5 | 75 | 21% | 24% | -15% | 77% | 67% | 99% |
| d+6 | 74 | 23% | 25% | -16% | 77% | 66% | 99% |
| d+7 | 73 | 23% | 26% | -17% | 73% | 62% | 99% |

Across all lead times the 80% range contained the truth **80%** of the time on **532** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-11-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 12 Nov | d+1 | 131.7 | 95.3 to 182.0 | 207 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+2 | 131.4 | 89.2 to 193.4 | 207 | pending | pending | n/a | n/a |
| Sat 14 Nov | d+3 | 131.2 | 88.1 to 195.5 | 207 | pending | pending | n/a | n/a |
| Sun 15 Nov | d+4 | 131.1 | 87.3 to 196.9 | 207 | pending | pending | n/a | n/a |
| Mon 16 Nov | d+5 | 131.1 | 86.7 to 198.1 | 207 | pending | pending | n/a | n/a |
| Tue 17 Nov | d+6 | 131.0 | 86.6 to 198.4 | 206 | pending | pending | n/a | n/a |
| Wed 18 Nov | d+7 | 131.0 | 86.0 to 199.6 | 206 | pending | pending | n/a | n/a |

### Issued 2026-11-11

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 11 Nov | d+1 | 124.0 | 89.7 to 171.5 | 199 | 132.1 | 208 | -6% | yes |
| Thu 12 Nov | d+2 | 124.4 | 84.5 to 183.4 | 199 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+3 | 124.7 | 83.6 to 186.0 | 200 | pending | pending | n/a | n/a |
| Sat 14 Nov | d+4 | 124.8 | 83.1 to 187.6 | 200 | pending | pending | n/a | n/a |
| Sun 15 Nov | d+5 | 124.9 | 82.6 to 189.0 | 200 | pending | pending | n/a | n/a |
| Mon 16 Nov | d+6 | 125.0 | 82.5 to 189.3 | 200 | pending | pending | n/a | n/a |
| Tue 17 Nov | d+7 | 125.0 | 82.0 to 190.5 | 200 | pending | pending | n/a | n/a |

### Issued 2026-11-10

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 10 Nov | d+1 | 137.5 | 99.3 to 190.3 | 213 | 123.3 | 198 | +12% | yes |
| Wed 11 Nov | d+2 | 130.6 | 88.6 to 192.6 | 206 | 132.1 | 208 | -1% | yes |
| Thu 12 Nov | d+3 | 126.7 | 84.9 to 189.1 | 202 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+4 | 124.5 | 82.8 to 187.2 | 199 | pending | pending | n/a | n/a |
| Sat 14 Nov | d+5 | 123.2 | 81.4 to 186.4 | 198 | pending | pending | n/a | n/a |
| Sun 15 Nov | d+6 | 122.4 | 80.8 to 185.6 | 198 | pending | pending | n/a | n/a |
| Mon 16 Nov | d+7 | 122.0 | 80.0 to 186.0 | 198 | pending | pending | n/a | n/a |

### Issued 2026-11-09

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 09 Nov | d+1 | 155.8 | 112.5 to 215.7 | 231 | 150.0 | 225 | +4% | yes |
| Tue 10 Nov | d+2 | 137.9 | 93.5 to 203.4 | 213 | 123.3 | 198 | +12% | yes |
| Wed 11 Nov | d+3 | 128.4 | 86.0 to 191.5 | 204 | 132.1 | 208 | -3% | yes |
| Thu 12 Nov | d+4 | 123.0 | 81.8 to 185.0 | 198 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+5 | 120.0 | 79.3 to 181.6 | 196 | pending | pending | n/a | n/a |
| Sat 14 Nov | d+6 | 118.3 | 78.1 to 179.3 | 195 | pending | pending | n/a | n/a |
| Sun 15 Nov | d+7 | 117.3 | 76.9 to 178.8 | 194 | pending | pending | n/a | n/a |

### Issued 2026-11-08

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 08 Nov | d+1 | 116.1 | 84.0 to 160.5 | 193 | 191.8 | 267 | -39% | **no** |
| Mon 09 Nov | d+2 | 112.2 | 76.2 to 165.1 | 191 | 150.0 | 225 | -25% | yes |
| Tue 10 Nov | d+3 | 110.0 | 73.8 to 163.7 | 189 | 123.3 | 198 | -11% | yes |
| Wed 11 Nov | d+4 | 108.7 | 72.4 to 163.0 | 188 | 132.1 | 208 | -18% | yes |
| Thu 12 Nov | d+5 | 107.9 | 71.5 to 162.9 | 188 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+6 | 107.5 | 71.1 to 162.4 | 187 | pending | pending | n/a | n/a |
| Sat 14 Nov | d+7 | 107.2 | 70.6 to 162.9 | 187 | pending | pending | n/a | n/a |

### Issued 2026-11-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 07 Nov | d+1 | 105.5 | 76.3 to 145.9 | 186 | 123.1 | 198 | -14% | yes |
| Sun 08 Nov | d+2 | 103.3 | 70.2 to 152.1 | 185 | 191.8 | 267 | -46% | **no** |
| Mon 09 Nov | d+3 | 102.0 | 68.5 to 152.0 | 184 | 150.0 | 225 | -32% | yes |
| Tue 10 Nov | d+4 | 101.3 | 67.5 to 152.0 | 183 | 123.3 | 198 | -18% | yes |
| Wed 11 Nov | d+5 | 100.8 | 66.8 to 152.3 | 183 | 132.1 | 208 | -24% | yes |
| Thu 12 Nov | d+6 | 100.6 | 66.5 to 152.0 | 183 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+7 | 100.4 | 66.1 to 152.5 | 182 | pending | pending | n/a | n/a |

### Issued 2026-11-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 06 Nov | d+1 | 105.9 | 76.5 to 146.6 | 186 | 109.5 | 189 | -3% | yes |
| Sat 07 Nov | d+2 | 103.5 | 70.2 to 152.5 | 185 | 123.1 | 198 | -16% | yes |
| Sun 08 Nov | d+3 | 102.1 | 68.5 to 152.3 | 184 | 191.8 | 267 | -47% | **no** |
| Mon 09 Nov | d+4 | 101.3 | 67.4 to 152.2 | 183 | 150.0 | 225 | -32% | yes |
| Tue 10 Nov | d+5 | 100.8 | 66.7 to 152.4 | 183 | 123.3 | 198 | -18% | yes |
| Wed 11 Nov | d+6 | 100.6 | 66.5 to 152.1 | 183 | 132.1 | 208 | -24% | yes |
| Thu 12 Nov | d+7 | 100.4 | 66.1 to 152.5 | 182 | pending | pending | n/a | n/a |

### Issued 2026-11-05

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 05 Nov | d+1 | 111.0 | 80.1 to 153.7 | 190 | 110.3 | 189 | +1% | yes |
| Fri 06 Nov | d+2 | 105.8 | 71.8 to 156.1 | 186 | 109.5 | 189 | -3% | yes |
| Sat 07 Nov | d+3 | 102.9 | 69.0 to 153.6 | 184 | 123.1 | 198 | -16% | yes |
| Sun 08 Nov | d+4 | 101.2 | 67.3 to 152.2 | 183 | 191.8 | 267 | -47% | **no** |
| Mon 09 Nov | d+5 | 100.3 | 66.3 to 151.6 | 182 | 150.0 | 225 | -33% | yes |
| Tue 10 Nov | d+6 | 99.7 | 65.9 to 150.7 | 182 | 123.3 | 198 | -19% | yes |
| Wed 11 Nov | d+7 | 99.3 | 65.4 to 150.8 | 182 | 132.1 | 208 | -25% | yes |

### Issued 2026-11-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 04 Nov | d+1 | 110.7 | 79.9 to 153.5 | 190 | 120.4 | 196 | -8% | yes |
| Thu 05 Nov | d+2 | 104.3 | 70.7 to 154.0 | 185 | 110.3 | 189 | -5% | yes |
| Fri 06 Nov | d+3 | 100.7 | 67.5 to 150.4 | 183 | 109.5 | 189 | -8% | yes |
| Sat 07 Nov | d+4 | 98.7 | 65.6 to 148.4 | 181 | 123.1 | 198 | -20% | yes |
| Sun 08 Nov | d+5 | 97.5 | 64.5 to 147.3 | 180 | 191.8 | 267 | -49% | **no** |
| Mon 09 Nov | d+6 | 96.8 | 64.1 to 146.2 | 180 | 150.0 | 225 | -35% | **no** |
| Tue 10 Nov | d+7 | 96.4 | 63.6 to 146.1 | 180 | 123.3 | 198 | -22% | yes |

### Issued 2026-11-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 03 Nov | d+1 | 126.3 | 91.1 to 175.1 | 202 | 122.8 | 198 | +3% | yes |
| Wed 04 Nov | d+2 | 111.0 | 75.2 to 164.0 | 190 | 120.4 | 196 | -8% | yes |
| Thu 05 Nov | d+3 | 102.9 | 68.9 to 153.8 | 184 | 110.3 | 189 | -7% | yes |
| Fri 06 Nov | d+4 | 98.5 | 65.5 to 148.0 | 181 | 109.5 | 189 | -10% | yes |
| Sat 07 Nov | d+5 | 96.0 | 63.6 to 144.8 | 179 | 123.1 | 198 | -22% | yes |
| Sun 08 Nov | d+6 | 94.5 | 62.7 to 142.4 | 178 | 191.8 | 267 | -51% | **no** |
| Mon 09 Nov | d+7 | 93.7 | 61.9 to 141.6 | 178 | 150.0 | 225 | -38% | **no** |

_70 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

