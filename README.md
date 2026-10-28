# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-29 04:24 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-28, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Thu 29 Oct | d+1 | 67.4 | 48.8 to 93.0 | 76.2 | 159 | Unhealthy | cloudy, 15 to 28C |
| Fri 30 Oct | d+2 | 66.6 | 45.7 to 97.2 | 75.2 | 159 | Unhealthy | drizzle, 17 to 28C, 1mm |
| Sat 31 Oct | d+3 | 66.2 | 45.1 to 97.2 | 74.7 | 159 | Unhealthy | cloudy, 16 to 27C |
| Sun 01 Nov | d+4 | 66.0 | 44.8 to 97.1 | 74.4 | 158 | Unhealthy | cloudy, 15 to 27C |
| Mon 02 Nov | d+5 | 65.9 | 44.7 to 97.1 | 74.2 | 158 | Unhealthy | clear, 15 to 28C |
| Tue 03 Nov | d+6 | 65.8 | 44.7 to 96.7 | 74.2 | 158 | Unhealthy | cloudy, 14 to 27C |
| Wed 04 Nov | d+7 | 65.7 | 44.6 to 96.9 | 74.1 | 158 | Unhealthy | cloudy, 14 to 27C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 65 | 13% | 16% | -5% | 92% | 72% | 98% |
| d+2 | 64 | 17% | 19% | -7% | 88% | 69% | 98% |
| d+3 | 63 | 19% | 20% | -8% | 87% | 71% | 98% |
| d+4 | 62 | 17% | 21% | -8% | 84% | 69% | 98% |
| d+5 | 61 | 16% | 20% | -9% | 84% | 67% | 98% |
| d+6 | 60 | 16% | 21% | -9% | 83% | 67% | 98% |
| d+7 | 59 | 17% | 22% | -10% | 85% | 64% | 98% |

Across all lead times the 80% range contained the truth **86%** of the time on **434** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-29

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 29 Oct | d+1 | 67.4 | 48.8 to 93.0 | 159 | pending | pending | n/a | n/a |
| Fri 30 Oct | d+2 | 66.6 | 45.7 to 97.2 | 159 | pending | pending | n/a | n/a |
| Sat 31 Oct | d+3 | 66.2 | 45.1 to 97.2 | 159 | pending | pending | n/a | n/a |
| Sun 01 Nov | d+4 | 66.0 | 44.8 to 97.1 | 158 | pending | pending | n/a | n/a |
| Mon 02 Nov | d+5 | 65.9 | 44.7 to 97.1 | 158 | pending | pending | n/a | n/a |
| Tue 03 Nov | d+6 | 65.8 | 44.7 to 96.7 | 158 | pending | pending | n/a | n/a |
| Wed 04 Nov | d+7 | 65.7 | 44.6 to 96.9 | 158 | pending | pending | n/a | n/a |

### Issued 2026-10-28

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 28 Oct | d+1 | 73.6 | 53.3 to 101.7 | 164 | 68.7 | 160 | +7% | yes |
| Thu 29 Oct | d+2 | 69.7 | 47.8 to 101.9 | 161 | pending | pending | n/a | n/a |
| Fri 30 Oct | d+3 | 67.6 | 46.1 to 99.3 | 159 | pending | pending | n/a | n/a |
| Sat 31 Oct | d+4 | 66.5 | 45.1 to 97.9 | 159 | pending | pending | n/a | n/a |
| Sun 01 Nov | d+5 | 65.8 | 44.6 to 97.1 | 158 | pending | pending | n/a | n/a |
| Mon 02 Nov | d+6 | 65.4 | 44.5 to 96.3 | 158 | pending | pending | n/a | n/a |
| Tue 03 Nov | d+7 | 65.2 | 44.2 to 96.2 | 158 | pending | pending | n/a | n/a |

### Issued 2026-10-27

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 27 Oct | d+1 | 71.7 | 51.9 to 99.2 | 162 | 81.0 | 169 | -11% | yes |
| Wed 28 Oct | d+2 | 67.9 | 46.5 to 99.2 | 160 | 68.7 | 160 | -1% | yes |
| Thu 29 Oct | d+3 | 65.8 | 44.8 to 96.6 | 158 | pending | pending | n/a | n/a |
| Fri 30 Oct | d+4 | 64.6 | 43.9 to 95.2 | 157 | pending | pending | n/a | n/a |
| Sat 31 Oct | d+5 | 64.0 | 43.3 to 94.5 | 157 | pending | pending | n/a | n/a |
| Sun 01 Nov | d+6 | 63.6 | 43.2 to 93.6 | 157 | pending | pending | n/a | n/a |
| Mon 02 Nov | d+7 | 63.4 | 43.0 to 93.5 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-26

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 26 Oct | d+1 | 61.3 | 44.4 to 84.7 | 155 | 79.0 | 167 | -22% | yes |
| Tue 27 Oct | d+2 | 61.3 | 41.9 to 89.5 | 155 | 81.0 | 169 | -24% | yes |
| Wed 28 Oct | d+3 | 61.2 | 41.7 to 90.0 | 155 | 68.7 | 160 | -11% | yes |
| Thu 29 Oct | d+4 | 61.2 | 41.5 to 90.3 | 155 | pending | pending | n/a | n/a |
| Fri 30 Oct | d+5 | 61.2 | 41.5 to 90.4 | 155 | pending | pending | n/a | n/a |
| Sat 31 Oct | d+6 | 61.2 | 41.6 to 90.1 | 155 | pending | pending | n/a | n/a |
| Sun 01 Nov | d+7 | 61.2 | 41.5 to 90.3 | 155 | pending | pending | n/a | n/a |

### Issued 2026-10-25

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 25 Oct | d+1 | 54.7 | 39.6 to 75.7 | 148 | 61.5 | 155 | -11% | yes |
| Mon 26 Oct | d+2 | 57.3 | 39.2 to 83.7 | 152 | 79.0 | 167 | -28% | yes |
| Tue 27 Oct | d+3 | 58.8 | 40.0 to 86.5 | 153 | 81.0 | 169 | -27% | yes |
| Wed 28 Oct | d+4 | 59.7 | 40.5 to 88.1 | 154 | 68.7 | 160 | -13% | yes |
| Thu 29 Oct | d+5 | 60.2 | 40.8 to 89.0 | 154 | pending | pending | n/a | n/a |
| Fri 30 Oct | d+6 | 60.5 | 41.1 to 89.1 | 155 | pending | pending | n/a | n/a |
| Sat 31 Oct | d+7 | 60.7 | 41.1 to 89.6 | 155 | pending | pending | n/a | n/a |

### Issued 2026-10-24

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 24 Oct | d+1 | 86.2 | 62.5 to 118.9 | 173 | 50.5 | 138 | +71% | **no** |
| Sun 25 Oct | d+2 | 75.4 | 51.6 to 110.1 | 165 | 61.5 | 155 | +23% | yes |
| Mon 26 Oct | d+3 | 69.8 | 47.4 to 102.7 | 161 | 79.0 | 167 | -12% | yes |
| Tue 27 Oct | d+4 | 66.7 | 45.2 to 98.5 | 159 | 81.0 | 169 | -18% | yes |
| Wed 28 Oct | d+5 | 65.0 | 44.0 to 96.2 | 158 | 68.7 | 160 | -5% | yes |
| Thu 29 Oct | d+6 | 64.1 | 43.5 to 94.5 | 157 | pending | pending | n/a | n/a |
| Fri 30 Oct | d+7 | 63.5 | 43.0 to 93.9 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-23

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 23 Oct | d+1 | 76.4 | 55.4 to 105.3 | 166 | 108.8 | 188 | -30% | **no** |
| Sat 24 Oct | d+2 | 68.7 | 47.1 to 100.3 | 160 | 50.5 | 138 | +36% | yes |
| Sun 25 Oct | d+3 | 64.7 | 44.1 to 95.0 | 157 | 61.5 | 155 | +5% | yes |
| Mon 26 Oct | d+4 | 62.5 | 42.5 to 92.1 | 156 | 79.0 | 167 | -21% | yes |
| Tue 27 Oct | d+5 | 61.3 | 41.5 to 90.5 | 155 | 81.0 | 169 | -24% | yes |
| Wed 28 Oct | d+6 | 60.6 | 41.2 to 89.2 | 155 | 68.7 | 160 | -12% | yes |
| Thu 29 Oct | d+7 | 60.2 | 40.8 to 88.8 | 154 | pending | pending | n/a | n/a |

### Issued 2026-10-22

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 22 Oct | d+1 | 68.6 | 49.8 to 94.6 | 160 | 91.8 | 176 | -25% | yes |
| Fri 23 Oct | d+2 | 63.6 | 43.7 to 92.8 | 157 | 108.8 | 188 | -42% | **no** |
| Sat 24 Oct | d+3 | 61.0 | 41.6 to 89.5 | 155 | 50.5 | 138 | +21% | yes |
| Sun 25 Oct | d+4 | 59.5 | 40.5 to 87.6 | 154 | 61.5 | 155 | -3% | yes |
| Mon 26 Oct | d+5 | 58.7 | 39.8 to 86.6 | 153 | 79.0 | 167 | -26% | yes |
| Tue 27 Oct | d+6 | 58.2 | 39.6 to 85.6 | 153 | 81.0 | 169 | -28% | yes |
| Wed 28 Oct | d+7 | 58.0 | 39.3 to 85.5 | 153 | 68.7 | 160 | -16% | yes |

### Issued 2026-10-21

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 21 Oct | d+1 | 66.3 | 48.0 to 91.4 | 159 | 78.3 | 167 | -15% | yes |
| Thu 22 Oct | d+2 | 61.8 | 42.4 to 90.2 | 155 | 91.8 | 176 | -33% | **no** |
| Fri 23 Oct | d+3 | 59.4 | 40.5 to 87.2 | 154 | 108.8 | 188 | -45% | **no** |
| Sat 24 Oct | d+4 | 58.1 | 39.5 to 85.6 | 153 | 50.5 | 138 | +15% | yes |
| Sun 25 Oct | d+5 | 57.4 | 38.9 to 84.7 | 152 | 61.5 | 155 | -7% | yes |
| Mon 26 Oct | d+6 | 57.0 | 38.7 to 83.8 | 152 | 79.0 | 167 | -28% | yes |
| Tue 27 Oct | d+7 | 56.7 | 38.5 to 83.7 | 152 | 81.0 | 169 | -30% | yes |

### Issued 2026-10-20

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 20 Oct | d+1 | 61.7 | 44.7 to 85.2 | 155 | 74.8 | 164 | -18% | yes |
| Wed 21 Oct | d+2 | 59.3 | 40.6 to 86.4 | 154 | 78.3 | 167 | -24% | yes |
| Thu 22 Oct | d+3 | 57.9 | 39.5 to 85.0 | 153 | 91.8 | 176 | -37% | **no** |
| Fri 23 Oct | d+4 | 57.2 | 38.8 to 84.1 | 152 | 108.8 | 188 | -47% | **no** |
| Sat 24 Oct | d+5 | 56.7 | 38.5 to 83.7 | 152 | 50.5 | 138 | +12% | yes |
| Sun 25 Oct | d+6 | 56.5 | 38.4 to 83.1 | 152 | 61.5 | 155 | -8% | yes |
| Mon 26 Oct | d+7 | 56.4 | 38.2 to 83.2 | 152 | 79.0 | 167 | -29% | yes |

_56 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

