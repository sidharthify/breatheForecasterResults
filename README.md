# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-24 03:14 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-23, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Sat 24 Oct | d+1 | 86.2 | 62.5 to 118.9 | 93.3 | 172 | Unhealthy | drizzle, 15 to 27C |
| Sun 25 Oct | d+2 | 75.4 | 51.6 to 110.1 | 82.3 | 165 | Unhealthy | clear, 13 to 28C |
| Mon 26 Oct | d+3 | 69.8 | 47.4 to 102.7 | 76.7 | 161 | Unhealthy | clear, 12 to 27C |
| Tue 27 Oct | d+4 | 66.7 | 45.2 to 98.5 | 73.8 | 159 | Unhealthy | clear, 14 to 28C |
| Wed 28 Oct | d+5 | 65.0 | 44.0 to 96.2 | 72.3 | 158 | Unhealthy | clear, 12 to 28C |
| Thu 29 Oct | d+6 | 64.1 | 43.5 to 94.5 | 71.4 | 157 | Unhealthy | clear, 12 to 29C |
| Fri 30 Oct | d+7 | 63.5 | 43.0 to 93.9 | 71.0 | 157 | Unhealthy | clear, 16 to 28C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 60 | 13% | 15% | -6% | 93% | 75% | 98% |
| d+2 | 59 | 16% | 19% | -8% | 85% | 66% | 98% |
| d+3 | 58 | 19% | 20% | -8% | 86% | 69% | 98% |
| d+4 | 57 | 18% | 21% | -7% | 82% | 67% | 98% |
| d+5 | 56 | 18% | 21% | -8% | 82% | 64% | 98% |
| d+6 | 55 | 16% | 21% | -9% | 82% | 64% | 98% |
| d+7 | 54 | 17% | 22% | -10% | 83% | 61% | 98% |

Across all lead times the 80% range contained the truth **85%** of the time on **399** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-24

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 24 Oct | d+1 | 86.2 | 62.5 to 118.9 | 173 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+2 | 75.4 | 51.6 to 110.1 | 165 | pending | pending | n/a | n/a |
| Mon 26 Oct | d+3 | 69.8 | 47.4 to 102.7 | 161 | pending | pending | n/a | n/a |
| Tue 27 Oct | d+4 | 66.7 | 45.2 to 98.5 | 159 | pending | pending | n/a | n/a |
| Wed 28 Oct | d+5 | 65.0 | 44.0 to 96.2 | 158 | pending | pending | n/a | n/a |
| Thu 29 Oct | d+6 | 64.1 | 43.5 to 94.5 | 157 | pending | pending | n/a | n/a |
| Fri 30 Oct | d+7 | 63.5 | 43.0 to 93.9 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-23

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 23 Oct | d+1 | 76.4 | 55.4 to 105.3 | 166 | 108.7 | 188 | -30% | **no** |
| Sat 24 Oct | d+2 | 68.7 | 47.1 to 100.3 | 160 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+3 | 64.7 | 44.1 to 95.0 | 157 | pending | pending | n/a | n/a |
| Mon 26 Oct | d+4 | 62.5 | 42.5 to 92.1 | 156 | pending | pending | n/a | n/a |
| Tue 27 Oct | d+5 | 61.3 | 41.5 to 90.5 | 155 | pending | pending | n/a | n/a |
| Wed 28 Oct | d+6 | 60.6 | 41.2 to 89.2 | 155 | pending | pending | n/a | n/a |
| Thu 29 Oct | d+7 | 60.2 | 40.8 to 88.8 | 154 | pending | pending | n/a | n/a |

### Issued 2026-10-22

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 22 Oct | d+1 | 68.6 | 49.8 to 94.6 | 160 | 91.8 | 176 | -25% | yes |
| Fri 23 Oct | d+2 | 63.6 | 43.7 to 92.8 | 157 | 108.7 | 188 | -42% | **no** |
| Sat 24 Oct | d+3 | 61.0 | 41.6 to 89.5 | 155 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+4 | 59.5 | 40.5 to 87.6 | 154 | pending | pending | n/a | n/a |
| Mon 26 Oct | d+5 | 58.7 | 39.8 to 86.6 | 153 | pending | pending | n/a | n/a |
| Tue 27 Oct | d+6 | 58.2 | 39.6 to 85.6 | 153 | pending | pending | n/a | n/a |
| Wed 28 Oct | d+7 | 58.0 | 39.3 to 85.5 | 153 | pending | pending | n/a | n/a |

### Issued 2026-10-21

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 21 Oct | d+1 | 66.3 | 48.0 to 91.4 | 159 | 78.2 | 167 | -15% | yes |
| Thu 22 Oct | d+2 | 61.8 | 42.4 to 90.2 | 155 | 91.8 | 176 | -33% | **no** |
| Fri 23 Oct | d+3 | 59.4 | 40.5 to 87.2 | 154 | 108.7 | 188 | -45% | **no** |
| Sat 24 Oct | d+4 | 58.1 | 39.5 to 85.6 | 153 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+5 | 57.4 | 38.9 to 84.7 | 152 | pending | pending | n/a | n/a |
| Mon 26 Oct | d+6 | 57.0 | 38.7 to 83.8 | 152 | pending | pending | n/a | n/a |
| Tue 27 Oct | d+7 | 56.7 | 38.5 to 83.7 | 152 | pending | pending | n/a | n/a |

### Issued 2026-10-20

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 20 Oct | d+1 | 61.7 | 44.7 to 85.2 | 155 | 74.8 | 165 | -18% | yes |
| Wed 21 Oct | d+2 | 59.3 | 40.6 to 86.4 | 154 | 78.2 | 167 | -24% | yes |
| Thu 22 Oct | d+3 | 57.9 | 39.5 to 85.0 | 153 | 91.8 | 176 | -37% | **no** |
| Fri 23 Oct | d+4 | 57.2 | 38.8 to 84.1 | 152 | 108.7 | 188 | -47% | **no** |
| Sat 24 Oct | d+5 | 56.7 | 38.5 to 83.7 | 152 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+6 | 56.5 | 38.4 to 83.1 | 152 | pending | pending | n/a | n/a |
| Mon 26 Oct | d+7 | 56.4 | 38.2 to 83.2 | 152 | pending | pending | n/a | n/a |

### Issued 2026-10-19

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 19 Oct | d+1 | 57.3 | 41.5 to 79.1 | 152 | 66.2 | 158 | -13% | yes |
| Tue 20 Oct | d+2 | 57.3 | 39.2 to 83.6 | 152 | 74.8 | 165 | -23% | yes |
| Wed 21 Oct | d+3 | 57.3 | 39.0 to 84.1 | 152 | 78.2 | 167 | -27% | yes |
| Thu 22 Oct | d+4 | 57.3 | 38.9 to 84.3 | 152 | 91.8 | 176 | -38% | **no** |
| Fri 23 Oct | d+5 | 57.3 | 38.8 to 84.5 | 152 | 108.7 | 188 | -47% | **no** |
| Sat 24 Oct | d+6 | 57.3 | 38.9 to 84.3 | 152 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+7 | 57.3 | 38.8 to 84.5 | 152 | pending | pending | n/a | n/a |

### Issued 2026-10-18

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 18 Oct | d+1 | 59.2 | 42.9 to 81.9 | 154 | 57.4 | 152 | +3% | yes |
| Mon 19 Oct | d+2 | 58.9 | 40.3 to 86.1 | 153 | 66.2 | 158 | -11% | yes |
| Tue 20 Oct | d+3 | 58.7 | 40.0 to 86.3 | 153 | 74.8 | 165 | -22% | yes |
| Wed 21 Oct | d+4 | 58.6 | 39.8 to 86.4 | 153 | 78.2 | 167 | -25% | yes |
| Thu 22 Oct | d+5 | 58.6 | 39.6 to 86.5 | 153 | 91.8 | 176 | -36% | **no** |
| Fri 23 Oct | d+6 | 58.5 | 39.7 to 86.2 | 153 | 108.7 | 188 | -46% | **no** |
| Sat 24 Oct | d+7 | 58.5 | 39.6 to 86.5 | 153 | pending | pending | n/a | n/a |

### Issued 2026-10-17

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 17 Oct | d+1 | 50.8 | 36.8 to 70.3 | 139 | 59.7 | 154 | -15% | yes |
| Sun 18 Oct | d+2 | 54.1 | 37.0 to 79.1 | 147 | 57.4 | 152 | -6% | yes |
| Mon 19 Oct | d+3 | 56.1 | 38.1 to 82.5 | 151 | 66.2 | 158 | -15% | yes |
| Tue 20 Oct | d+4 | 57.2 | 38.8 to 84.5 | 152 | 74.8 | 165 | -24% | yes |
| Wed 21 Oct | d+5 | 57.9 | 39.1 to 85.7 | 153 | 78.2 | 167 | -26% | yes |
| Thu 22 Oct | d+6 | 58.3 | 39.5 to 86.0 | 153 | 91.8 | 176 | -37% | **no** |
| Fri 23 Oct | d+7 | 58.5 | 39.5 to 86.6 | 153 | 108.7 | 188 | -46% | **no** |

### Issued 2026-10-16

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 16 Oct | d+1 | 43.0 | 31.1 to 59.4 | 119 | 46.1 | 127 | -7% | yes |
| Sat 17 Oct | d+2 | 50.0 | 34.2 to 73.1 | 137 | 59.7 | 154 | -16% | yes |
| Sun 18 Oct | d+3 | 54.5 | 37.1 to 80.1 | 148 | 57.4 | 152 | -5% | yes |
| Mon 19 Oct | d+4 | 57.2 | 38.8 to 84.4 | 152 | 66.2 | 158 | -14% | yes |
| Tue 20 Oct | d+5 | 58.8 | 39.8 to 86.9 | 153 | 74.8 | 165 | -21% | yes |
| Wed 21 Oct | d+6 | 59.7 | 40.5 to 88.0 | 154 | 78.2 | 167 | -24% | yes |
| Thu 22 Oct | d+7 | 60.3 | 40.8 to 89.1 | 154 | 91.8 | 176 | -34% | **no** |

### Issued 2026-10-15

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 15 Oct | d+1 | 60.5 | 43.9 to 83.3 | 155 | 33.2 | 96 | +82% | **no** |
| Fri 16 Oct | d+2 | 61.8 | 42.4 to 90.0 | 155 | 46.1 | 127 | +34% | yes |
| Sat 17 Oct | d+3 | 62.5 | 42.6 to 91.6 | 156 | 59.7 | 154 | +5% | yes |
| Sun 18 Oct | d+4 | 62.9 | 42.8 to 92.5 | 156 | 57.4 | 152 | +10% | yes |
| Mon 19 Oct | d+5 | 63.2 | 42.9 to 93.0 | 156 | 66.2 | 158 | -4% | yes |
| Tue 20 Oct | d+6 | 63.3 | 43.2 to 93.0 | 156 | 74.8 | 165 | -15% | yes |
| Wed 21 Oct | d+7 | 63.4 | 43.1 to 93.3 | 157 | 78.2 | 167 | -19% | yes |

_51 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

