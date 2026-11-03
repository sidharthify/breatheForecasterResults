# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-11-04 05:14 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-11-03, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Wed 04 Nov | d+1 | 110.7 | 79.9 to 153.5 | 120.5 | 190 | Unhealthy | cloudy, 14 to 27C |
| Thu 05 Nov | d+2 | 104.3 | 70.7 to 154.0 | 114.2 | 185 | Unhealthy | cloudy, 14 to 26C |
| Fri 06 Nov | d+3 | 100.7 | 67.5 to 150.4 | 110.7 | 183 | Unhealthy | cloudy, 14 to 27C |
| Sat 07 Nov | d+4 | 98.7 | 65.6 to 148.4 | 108.8 | 181 | Unhealthy | clear, 14 to 26C |
| Sun 08 Nov | d+5 | 97.5 | 64.5 to 147.3 | 107.7 | 180 | Unhealthy | cloudy, 14 to 26C |
| Mon 09 Nov | d+6 | 96.8 | 64.1 to 146.2 | 107.1 | 180 | Unhealthy | cloudy, 14 to 27C |
| Tue 10 Nov | d+7 | 96.4 | 63.6 to 146.1 | 106.8 | 180 | Unhealthy | clear, 13 to 27C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 71 | 14% | 17% | -7% | 90% | 73% | 99% |
| d+2 | 70 | 18% | 20% | -10% | 83% | 69% | 99% |
| d+3 | 69 | 20% | 22% | -11% | 83% | 71% | 99% |
| d+4 | 68 | 19% | 23% | -11% | 78% | 69% | 99% |
| d+5 | 67 | 20% | 23% | -12% | 78% | 67% | 99% |
| d+6 | 66 | 18% | 24% | -13% | 77% | 67% | 98% |
| d+7 | 65 | 18% | 24% | -14% | 78% | 65% | 98% |

Across all lead times the 80% range contained the truth **81%** of the time on **476** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-11-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 04 Nov | d+1 | 110.7 | 79.9 to 153.5 | 190 | pending | pending | n/a | n/a |
| Thu 05 Nov | d+2 | 104.3 | 70.7 to 154.0 | 185 | pending | pending | n/a | n/a |
| Fri 06 Nov | d+3 | 100.7 | 67.5 to 150.4 | 183 | pending | pending | n/a | n/a |
| Sat 07 Nov | d+4 | 98.7 | 65.6 to 148.4 | 181 | pending | pending | n/a | n/a |
| Sun 08 Nov | d+5 | 97.5 | 64.5 to 147.3 | 180 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+6 | 96.8 | 64.1 to 146.2 | 180 | pending | pending | n/a | n/a |
| Tue 10 Nov | d+7 | 96.4 | 63.6 to 146.1 | 180 | pending | pending | n/a | n/a |

### Issued 2026-11-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 03 Nov | d+1 | 126.3 | 91.1 to 175.1 | 202 | 122.6 | 198 | +3% | yes |
| Wed 04 Nov | d+2 | 111.0 | 75.2 to 164.0 | 190 | pending | pending | n/a | n/a |
| Thu 05 Nov | d+3 | 102.9 | 68.9 to 153.8 | 184 | pending | pending | n/a | n/a |
| Fri 06 Nov | d+4 | 98.5 | 65.5 to 148.0 | 181 | pending | pending | n/a | n/a |
| Sat 07 Nov | d+5 | 96.0 | 63.6 to 144.8 | 179 | pending | pending | n/a | n/a |
| Sun 08 Nov | d+6 | 94.5 | 62.7 to 142.4 | 178 | pending | pending | n/a | n/a |
| Mon 09 Nov | d+7 | 93.7 | 61.9 to 141.6 | 178 | pending | pending | n/a | n/a |

### Issued 2026-11-02

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 02 Nov | d+1 | 129.5 | 93.4 to 179.7 | 205 | 157.3 | 233 | -18% | yes |
| Tue 03 Nov | d+2 | 109.6 | 74.2 to 161.8 | 189 | 122.6 | 198 | -11% | yes |
| Wed 04 Nov | d+3 | 99.5 | 66.7 to 148.2 | 182 | pending | pending | n/a | n/a |
| Thu 05 Nov | d+4 | 94.0 | 62.8 to 140.6 | 178 | pending | pending | n/a | n/a |
| Fri 06 Nov | d+5 | 91.0 | 60.6 to 136.5 | 176 | pending | pending | n/a | n/a |
| Sat 07 Nov | d+6 | 89.2 | 59.5 to 133.8 | 175 | pending | pending | n/a | n/a |
| Sun 08 Nov | d+7 | 88.3 | 58.7 to 132.7 | 174 | pending | pending | n/a | n/a |

### Issued 2026-11-01

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 01 Nov | d+1 | 125.7 | 90.6 to 174.3 | 201 | 172.9 | 248 | -27% | yes |
| Mon 02 Nov | d+2 | 103.8 | 70.5 to 152.8 | 185 | 157.3 | 233 | -34% | **no** |
| Tue 03 Nov | d+3 | 93.1 | 62.8 to 137.8 | 177 | 122.6 | 198 | -24% | yes |
| Wed 04 Nov | d+4 | 87.4 | 58.8 to 129.9 | 173 | pending | pending | n/a | n/a |
| Thu 05 Nov | d+5 | 84.3 | 56.6 to 125.7 | 171 | pending | pending | n/a | n/a |
| Fri 06 Nov | d+6 | 82.6 | 55.5 to 122.9 | 170 | pending | pending | n/a | n/a |
| Sat 07 Nov | d+7 | 81.6 | 54.8 to 121.7 | 169 | pending | pending | n/a | n/a |

### Issued 2026-10-31

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 31 Oct | d+1 | 98.8 | 71.4 to 136.6 | 181 | 175.6 | 251 | -44% | **no** |
| Sun 01 Nov | d+2 | 87.4 | 59.8 to 127.7 | 173 | 172.9 | 248 | -49% | **no** |
| Mon 02 Nov | d+3 | 81.5 | 55.5 to 119.8 | 169 | 157.3 | 233 | -48% | **no** |
| Tue 03 Nov | d+4 | 78.4 | 53.1 to 115.5 | 167 | 122.6 | 198 | -36% | **no** |
| Wed 04 Nov | d+5 | 76.6 | 51.8 to 113.3 | 166 | pending | pending | n/a | n/a |
| Thu 05 Nov | d+6 | 75.7 | 51.3 to 111.6 | 165 | pending | pending | n/a | n/a |
| Fri 06 Nov | d+7 | 75.1 | 50.8 to 111.0 | 165 | pending | pending | n/a | n/a |

### Issued 2026-10-30

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 30 Oct | d+1 | 70.7 | 51.3 to 97.6 | 162 | 122.6 | 198 | -42% | **no** |
| Sat 31 Oct | d+2 | 70.2 | 48.1 to 102.3 | 161 | 175.6 | 251 | -60% | **no** |
| Sun 01 Nov | d+3 | 69.8 | 47.6 to 102.4 | 161 | 172.9 | 248 | -60% | **no** |
| Mon 02 Nov | d+4 | 69.7 | 47.4 to 102.4 | 161 | 157.3 | 233 | -56% | **no** |
| Tue 03 Nov | d+5 | 69.5 | 47.2 to 102.5 | 161 | 122.6 | 198 | -43% | **no** |
| Wed 04 Nov | d+6 | 69.5 | 47.3 to 102.1 | 161 | pending | pending | n/a | n/a |
| Thu 05 Nov | d+7 | 69.5 | 47.1 to 102.3 | 161 | pending | pending | n/a | n/a |

### Issued 2026-10-29

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 29 Oct | d+1 | 67.4 | 48.8 to 93.0 | 159 | 71.7 | 162 | -6% | yes |
| Fri 30 Oct | d+2 | 66.6 | 45.7 to 97.2 | 159 | 122.6 | 198 | -46% | **no** |
| Sat 31 Oct | d+3 | 66.2 | 45.1 to 97.2 | 159 | 175.6 | 251 | -62% | **no** |
| Sun 01 Nov | d+4 | 66.0 | 44.8 to 97.1 | 158 | 172.9 | 248 | -62% | **no** |
| Mon 02 Nov | d+5 | 65.9 | 44.7 to 97.1 | 158 | 157.3 | 233 | -58% | **no** |
| Tue 03 Nov | d+6 | 65.8 | 44.7 to 96.7 | 158 | 122.6 | 198 | -46% | **no** |
| Wed 04 Nov | d+7 | 65.7 | 44.6 to 96.9 | 158 | pending | pending | n/a | n/a |

### Issued 2026-10-28

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 28 Oct | d+1 | 73.6 | 53.3 to 101.7 | 164 | 68.7 | 160 | +7% | yes |
| Thu 29 Oct | d+2 | 69.7 | 47.8 to 101.9 | 161 | 71.7 | 162 | -3% | yes |
| Fri 30 Oct | d+3 | 67.6 | 46.1 to 99.3 | 159 | 122.6 | 198 | -45% | **no** |
| Sat 31 Oct | d+4 | 66.5 | 45.1 to 97.9 | 159 | 175.6 | 251 | -62% | **no** |
| Sun 01 Nov | d+5 | 65.8 | 44.6 to 97.1 | 158 | 172.9 | 248 | -62% | **no** |
| Mon 02 Nov | d+6 | 65.4 | 44.5 to 96.3 | 158 | 157.3 | 233 | -58% | **no** |
| Tue 03 Nov | d+7 | 65.2 | 44.2 to 96.2 | 158 | 122.6 | 198 | -47% | **no** |

### Issued 2026-10-27

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 27 Oct | d+1 | 71.7 | 51.9 to 99.2 | 162 | 81.0 | 169 | -11% | yes |
| Wed 28 Oct | d+2 | 67.9 | 46.5 to 99.2 | 160 | 68.7 | 160 | -1% | yes |
| Thu 29 Oct | d+3 | 65.8 | 44.8 to 96.6 | 158 | 71.7 | 162 | -8% | yes |
| Fri 30 Oct | d+4 | 64.6 | 43.9 to 95.2 | 157 | 122.6 | 198 | -47% | **no** |
| Sat 31 Oct | d+5 | 64.0 | 43.3 to 94.5 | 157 | 175.6 | 251 | -64% | **no** |
| Sun 01 Nov | d+6 | 63.6 | 43.2 to 93.6 | 157 | 172.9 | 248 | -63% | **no** |
| Mon 02 Nov | d+7 | 63.4 | 43.0 to 93.5 | 157 | 157.3 | 233 | -60% | **no** |

### Issued 2026-10-26

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 26 Oct | d+1 | 61.3 | 44.4 to 84.7 | 155 | 79.0 | 167 | -22% | yes |
| Tue 27 Oct | d+2 | 61.3 | 41.9 to 89.5 | 155 | 81.0 | 169 | -24% | yes |
| Wed 28 Oct | d+3 | 61.2 | 41.7 to 90.0 | 155 | 68.7 | 160 | -11% | yes |
| Thu 29 Oct | d+4 | 61.2 | 41.5 to 90.3 | 155 | 71.7 | 162 | -15% | yes |
| Fri 30 Oct | d+5 | 61.2 | 41.5 to 90.4 | 155 | 122.6 | 198 | -50% | **no** |
| Sat 31 Oct | d+6 | 61.2 | 41.6 to 90.1 | 155 | 175.6 | 251 | -65% | **no** |
| Sun 01 Nov | d+7 | 61.2 | 41.5 to 90.3 | 155 | 172.9 | 248 | -65% | **no** |

_62 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

