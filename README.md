# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-11-08 03:54 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-11-07, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Sun 08 Nov | d+1 | 116.1 | 84.0 to 160.5 | 125.5 | 193 | Unhealthy | clear, 15 to 26C |
| Mon 09 Nov | d+2 | 112.2 | 76.2 to 165.1 | 121.8 | 191 | Unhealthy | cloudy, 15 to 26C |
| Tue 10 Nov | d+3 | 110.0 | 73.8 to 163.7 | 119.8 | 189 | Unhealthy | cloudy, 14 to 27C |
| Wed 11 Nov | d+4 | 108.7 | 72.4 to 163.0 | 118.6 | 188 | Unhealthy | cloudy, 15 to 27C |
| Thu 12 Nov | d+5 | 107.9 | 71.5 to 162.9 | 118.0 | 188 | Unhealthy | cloudy, 14 to 26C |
| Fri 13 Nov | d+6 | 107.5 | 71.1 to 162.4 | 117.6 | 187 | Unhealthy | cloudy, 14 to 27C |
| Sat 14 Nov | d+7 | 107.2 | 70.6 to 162.9 | 117.4 | 187 | Unhealthy | cloudy, 13 to 27C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 75 | 14% | 17% | -8% | 91% | 72% | 99% |
| d+2 | 74 | 17% | 20% | -10% | 84% | 70% | 99% |
| d+3 | 73 | 19% | 22% | -12% | 82% | 71% | 99% |
| d+4 | 72 | 18% | 23% | -12% | 79% | 71% | 99% |
| d+5 | 71 | 20% | 23% | -14% | 77% | 69% | 99% |
| d+6 | 70 | 21% | 24% | -15% | 77% | 69% | 99% |
| d+7 | 69 | 22% | 25% | -16% | 74% | 64% | 99% |

Across all lead times the 80% range contained the truth **81%** of the time on **504** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-11-08

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 08 Nov | d+1 | 116.1 | 84.0 to 160.5 | 193 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+2 | 112.2 | 76.2 to 165.1 | 191 | pending | pending | n/a | n/a |
| Tue 10 Nov | d+3 | 110.0 | 73.8 to 163.7 | 189 | pending | pending | n/a | n/a |
| Wed 11 Nov | d+4 | 108.7 | 72.4 to 163.0 | 188 | pending | pending | n/a | n/a |
| Thu 12 Nov | d+5 | 107.9 | 71.5 to 162.9 | 188 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+6 | 107.5 | 71.1 to 162.4 | 187 | pending | pending | n/a | n/a |
| Sat 14 Nov | d+7 | 107.2 | 70.6 to 162.9 | 187 | pending | pending | n/a | n/a |

### Issued 2026-11-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 07 Nov | d+1 | 105.5 | 76.3 to 145.9 | 186 | 123.1 | 198 | -14% | yes |
| Sun 08 Nov | d+2 | 103.3 | 70.2 to 152.1 | 185 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+3 | 102.0 | 68.5 to 152.0 | 184 | pending | pending | n/a | n/a |
| Tue 10 Nov | d+4 | 101.3 | 67.5 to 152.0 | 183 | pending | pending | n/a | n/a |
| Wed 11 Nov | d+5 | 100.8 | 66.8 to 152.3 | 183 | pending | pending | n/a | n/a |
| Thu 12 Nov | d+6 | 100.6 | 66.5 to 152.0 | 183 | pending | pending | n/a | n/a |
| Fri 13 Nov | d+7 | 100.4 | 66.1 to 152.5 | 182 | pending | pending | n/a | n/a |

### Issued 2026-11-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 06 Nov | d+1 | 105.9 | 76.5 to 146.6 | 186 | 109.4 | 189 | -3% | yes |
| Sat 07 Nov | d+2 | 103.5 | 70.2 to 152.5 | 185 | 123.1 | 198 | -16% | yes |
| Sun 08 Nov | d+3 | 102.1 | 68.5 to 152.3 | 184 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+4 | 101.3 | 67.4 to 152.2 | 183 | pending | pending | n/a | n/a |
| Tue 10 Nov | d+5 | 100.8 | 66.7 to 152.4 | 183 | pending | pending | n/a | n/a |
| Wed 11 Nov | d+6 | 100.6 | 66.5 to 152.1 | 183 | pending | pending | n/a | n/a |
| Thu 12 Nov | d+7 | 100.4 | 66.1 to 152.5 | 182 | pending | pending | n/a | n/a |

### Issued 2026-11-05

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 05 Nov | d+1 | 111.0 | 80.1 to 153.7 | 190 | 110.2 | 189 | +1% | yes |
| Fri 06 Nov | d+2 | 105.8 | 71.8 to 156.1 | 186 | 109.4 | 189 | -3% | yes |
| Sat 07 Nov | d+3 | 102.9 | 69.0 to 153.6 | 184 | 123.1 | 198 | -16% | yes |
| Sun 08 Nov | d+4 | 101.2 | 67.3 to 152.2 | 183 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+5 | 100.3 | 66.3 to 151.6 | 182 | pending | pending | n/a | n/a |
| Tue 10 Nov | d+6 | 99.7 | 65.9 to 150.7 | 182 | pending | pending | n/a | n/a |
| Wed 11 Nov | d+7 | 99.3 | 65.4 to 150.8 | 182 | pending | pending | n/a | n/a |

### Issued 2026-11-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 04 Nov | d+1 | 110.7 | 79.9 to 153.5 | 190 | 120.4 | 196 | -8% | yes |
| Thu 05 Nov | d+2 | 104.3 | 70.7 to 154.0 | 185 | 110.2 | 189 | -5% | yes |
| Fri 06 Nov | d+3 | 100.7 | 67.5 to 150.4 | 183 | 109.4 | 189 | -8% | yes |
| Sat 07 Nov | d+4 | 98.7 | 65.6 to 148.4 | 181 | 123.1 | 198 | -20% | yes |
| Sun 08 Nov | d+5 | 97.5 | 64.5 to 147.3 | 180 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+6 | 96.8 | 64.1 to 146.2 | 180 | pending | pending | n/a | n/a |
| Tue 10 Nov | d+7 | 96.4 | 63.6 to 146.1 | 180 | pending | pending | n/a | n/a |

### Issued 2026-11-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 03 Nov | d+1 | 126.3 | 91.1 to 175.1 | 202 | 122.7 | 198 | +3% | yes |
| Wed 04 Nov | d+2 | 111.0 | 75.2 to 164.0 | 190 | 120.4 | 196 | -8% | yes |
| Thu 05 Nov | d+3 | 102.9 | 68.9 to 153.8 | 184 | 110.2 | 189 | -7% | yes |
| Fri 06 Nov | d+4 | 98.5 | 65.5 to 148.0 | 181 | 109.4 | 189 | -10% | yes |
| Sat 07 Nov | d+5 | 96.0 | 63.6 to 144.8 | 179 | 123.1 | 198 | -22% | yes |
| Sun 08 Nov | d+6 | 94.5 | 62.7 to 142.4 | 178 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+7 | 93.7 | 61.9 to 141.6 | 178 | pending | pending | n/a | n/a |

### Issued 2026-11-02

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 02 Nov | d+1 | 129.5 | 93.4 to 179.7 | 205 | 157.5 | 233 | -18% | yes |
| Tue 03 Nov | d+2 | 109.6 | 74.2 to 161.8 | 189 | 122.7 | 198 | -11% | yes |
| Wed 04 Nov | d+3 | 99.5 | 66.7 to 148.2 | 182 | 120.4 | 196 | -17% | yes |
| Thu 05 Nov | d+4 | 94.0 | 62.8 to 140.6 | 178 | 110.2 | 189 | -15% | yes |
| Fri 06 Nov | d+5 | 91.0 | 60.6 to 136.5 | 176 | 109.4 | 189 | -17% | yes |
| Sat 07 Nov | d+6 | 89.2 | 59.5 to 133.8 | 175 | 123.1 | 198 | -28% | yes |
| Sun 08 Nov | d+7 | 88.3 | 58.7 to 132.7 | 174 | pending | pending | n/a | n/a |

### Issued 2026-11-01

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 01 Nov | d+1 | 125.7 | 90.6 to 174.3 | 201 | 173.3 | 248 | -27% | yes |
| Mon 02 Nov | d+2 | 103.8 | 70.5 to 152.8 | 185 | 157.5 | 233 | -34% | **no** |
| Tue 03 Nov | d+3 | 93.1 | 62.8 to 137.8 | 177 | 122.7 | 198 | -24% | yes |
| Wed 04 Nov | d+4 | 87.4 | 58.8 to 129.9 | 173 | 120.4 | 196 | -27% | yes |
| Thu 05 Nov | d+5 | 84.3 | 56.6 to 125.7 | 171 | 110.2 | 189 | -23% | yes |
| Fri 06 Nov | d+6 | 82.6 | 55.5 to 122.9 | 170 | 109.4 | 189 | -25% | yes |
| Sat 07 Nov | d+7 | 81.6 | 54.8 to 121.7 | 169 | 123.1 | 198 | -34% | **no** |

### Issued 2026-10-31

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 31 Oct | d+1 | 98.8 | 71.4 to 136.6 | 181 | 175.9 | 251 | -44% | **no** |
| Sun 01 Nov | d+2 | 87.4 | 59.8 to 127.7 | 173 | 173.3 | 248 | -50% | **no** |
| Mon 02 Nov | d+3 | 81.5 | 55.5 to 119.8 | 169 | 157.5 | 233 | -48% | **no** |
| Tue 03 Nov | d+4 | 78.4 | 53.1 to 115.5 | 167 | 122.7 | 198 | -36% | **no** |
| Wed 04 Nov | d+5 | 76.6 | 51.8 to 113.3 | 166 | 120.4 | 196 | -36% | **no** |
| Thu 05 Nov | d+6 | 75.7 | 51.3 to 111.6 | 165 | 110.2 | 189 | -31% | yes |
| Fri 06 Nov | d+7 | 75.1 | 50.8 to 111.0 | 165 | 109.4 | 189 | -31% | yes |

### Issued 2026-10-30

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 30 Oct | d+1 | 70.7 | 51.3 to 97.6 | 162 | 122.8 | 198 | -42% | **no** |
| Sat 31 Oct | d+2 | 70.2 | 48.1 to 102.3 | 161 | 175.9 | 251 | -60% | **no** |
| Sun 01 Nov | d+3 | 69.8 | 47.6 to 102.4 | 161 | 173.3 | 248 | -60% | **no** |
| Mon 02 Nov | d+4 | 69.7 | 47.4 to 102.4 | 161 | 157.5 | 233 | -56% | **no** |
| Tue 03 Nov | d+5 | 69.5 | 47.2 to 102.5 | 161 | 122.7 | 198 | -43% | **no** |
| Wed 04 Nov | d+6 | 69.5 | 47.3 to 102.1 | 161 | 120.4 | 196 | -42% | **no** |
| Thu 05 Nov | d+7 | 69.5 | 47.1 to 102.3 | 161 | 110.2 | 189 | -37% | **no** |

_66 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

