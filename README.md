# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-19 02:37 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-18, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Mon 19 Oct | d+1 | 57.3 | 41.5 to 79.1 | 65.2 | 152 | Unhealthy | clear, 14 to 28C |
| Tue 20 Oct | d+2 | 57.3 | 39.2 to 83.6 | 65.0 | 152 | Unhealthy | cloudy, 15 to 28C |
| Wed 21 Oct | d+3 | 57.3 | 39.0 to 84.1 | 64.8 | 152 | Unhealthy | clear, 16 to 28C |
| Thu 22 Oct | d+4 | 57.3 | 38.9 to 84.3 | 64.8 | 152 | Unhealthy | clear, 15 to 28C |
| Fri 23 Oct | d+5 | 57.3 | 38.8 to 84.5 | 64.7 | 152 | Unhealthy | clear, 15 to 28C |
| Sat 24 Oct | d+6 | 57.3 | 38.9 to 84.3 | 64.7 | 152 | Unhealthy | cloudy, 15 to 29C |
| Sun 25 Oct | d+7 | 57.3 | 38.8 to 84.5 | 64.7 | 152 | Unhealthy | clear, 14 to 30C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 55 | 11% | 14% | -1% | 95% | 73% | 98% |
| d+2 | 54 | 13% | 17% | -2% | 91% | 61% | 98% |
| d+3 | 53 | 17% | 19% | -2% | 91% | 58% | 98% |
| d+4 | 52 | 17% | 20% | -2% | 88% | 58% | 98% |
| d+5 | 51 | 17% | 20% | -3% | 86% | 53% | 98% |
| d+6 | 50 | 18% | 20% | -4% | 86% | 56% | 98% |
| d+7 | 49 | 17% | 20% | -5% | 86% | 59% | 98% |

Across all lead times the 80% range contained the truth **89%** of the time on **364** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-19

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 19 Oct | d+1 | 57.3 | 41.5 to 79.1 | 152 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+2 | 57.3 | 39.2 to 83.6 | 152 | pending | pending | n/a | n/a |
| Wed 21 Oct | d+3 | 57.3 | 39.0 to 84.1 | 152 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+4 | 57.3 | 38.9 to 84.3 | 152 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+5 | 57.3 | 38.8 to 84.5 | 152 | pending | pending | n/a | n/a |
| Sat 24 Oct | d+6 | 57.3 | 38.9 to 84.3 | 152 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+7 | 57.3 | 38.8 to 84.5 | 152 | pending | pending | n/a | n/a |

### Issued 2026-10-18

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 18 Oct | d+1 | 59.2 | 42.9 to 81.9 | 154 | 57.4 | 152 | +3% | yes |
| Mon 19 Oct | d+2 | 58.9 | 40.3 to 86.1 | 153 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+3 | 58.7 | 40.0 to 86.3 | 153 | pending | pending | n/a | n/a |
| Wed 21 Oct | d+4 | 58.6 | 39.8 to 86.4 | 153 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+5 | 58.6 | 39.6 to 86.5 | 153 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+6 | 58.5 | 39.7 to 86.2 | 153 | pending | pending | n/a | n/a |
| Sat 24 Oct | d+7 | 58.5 | 39.6 to 86.5 | 153 | pending | pending | n/a | n/a |

### Issued 2026-10-17

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 17 Oct | d+1 | 50.8 | 36.8 to 70.3 | 139 | 59.7 | 154 | -15% | yes |
| Sun 18 Oct | d+2 | 54.1 | 37.0 to 79.1 | 147 | 57.4 | 152 | -6% | yes |
| Mon 19 Oct | d+3 | 56.1 | 38.1 to 82.5 | 151 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+4 | 57.2 | 38.8 to 84.5 | 152 | pending | pending | n/a | n/a |
| Wed 21 Oct | d+5 | 57.9 | 39.1 to 85.7 | 153 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+6 | 58.3 | 39.5 to 86.0 | 153 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+7 | 58.5 | 39.5 to 86.6 | 153 | pending | pending | n/a | n/a |

### Issued 2026-10-16

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 16 Oct | d+1 | 43.0 | 31.1 to 59.4 | 119 | 45.6 | 126 | -6% | yes |
| Sat 17 Oct | d+2 | 50.0 | 34.2 to 73.1 | 137 | 59.7 | 154 | -16% | yes |
| Sun 18 Oct | d+3 | 54.5 | 37.1 to 80.1 | 148 | 57.4 | 152 | -5% | yes |
| Mon 19 Oct | d+4 | 57.2 | 38.8 to 84.4 | 152 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+5 | 58.8 | 39.8 to 86.9 | 153 | pending | pending | n/a | n/a |
| Wed 21 Oct | d+6 | 59.7 | 40.5 to 88.0 | 154 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+7 | 60.3 | 40.8 to 89.1 | 154 | pending | pending | n/a | n/a |

### Issued 2026-10-15

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 15 Oct | d+1 | 60.5 | 43.9 to 83.3 | 155 | 32.9 | 95 | +84% | **no** |
| Fri 16 Oct | d+2 | 61.8 | 42.4 to 90.0 | 155 | 45.6 | 126 | +36% | yes |
| Sat 17 Oct | d+3 | 62.5 | 42.6 to 91.6 | 156 | 59.7 | 154 | +5% | yes |
| Sun 18 Oct | d+4 | 62.9 | 42.8 to 92.5 | 156 | 57.4 | 152 | +10% | yes |
| Mon 19 Oct | d+5 | 63.2 | 42.9 to 93.0 | 156 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+6 | 63.3 | 43.2 to 93.0 | 156 | pending | pending | n/a | n/a |
| Wed 21 Oct | d+7 | 63.4 | 43.1 to 93.3 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-14

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 14 Oct | d+1 | 57.9 | 42.0 to 79.8 | 153 | 58.3 | 153 | -1% | yes |
| Thu 15 Oct | d+2 | 60.0 | 41.2 to 87.5 | 154 | 32.9 | 95 | +83% | **no** |
| Fri 16 Oct | d+3 | 61.2 | 41.7 to 89.8 | 155 | 45.6 | 126 | +34% | yes |
| Sat 17 Oct | d+4 | 61.9 | 42.1 to 91.1 | 155 | 59.7 | 154 | +4% | yes |
| Sun 18 Oct | d+5 | 62.3 | 42.3 to 91.8 | 156 | 57.4 | 152 | +9% | yes |
| Mon 19 Oct | d+6 | 62.6 | 42.6 to 91.9 | 156 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+7 | 62.7 | 42.6 to 92.3 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-13

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 13 Oct | d+1 | 54.7 | 39.7 to 75.5 | 148 | 54.4 | 148 | +0% | yes |
| Wed 14 Oct | d+2 | 57.8 | 39.6 to 84.3 | 153 | 58.3 | 153 | -1% | yes |
| Thu 15 Oct | d+3 | 59.6 | 40.6 to 87.5 | 154 | 32.9 | 95 | +81% | **no** |
| Fri 16 Oct | d+4 | 60.7 | 41.2 to 89.3 | 155 | 45.6 | 126 | +33% | yes |
| Sat 17 Oct | d+5 | 61.3 | 41.6 to 90.4 | 155 | 59.7 | 154 | +3% | yes |
| Sun 18 Oct | d+6 | 61.7 | 42.0 to 90.6 | 155 | 57.4 | 152 | +8% | yes |
| Mon 19 Oct | d+7 | 61.9 | 42.0 to 91.1 | 155 | pending | pending | n/a | n/a |

### Issued 2026-10-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 12 Oct | d+1 | 57.9 | 42.0 to 79.9 | 153 | 49.4 | 135 | +17% | yes |
| Tue 13 Oct | d+2 | 59.8 | 41.0 to 87.3 | 154 | 54.4 | 148 | +10% | yes |
| Wed 14 Oct | d+3 | 61.0 | 41.5 to 89.5 | 155 | 58.3 | 153 | +5% | yes |
| Thu 15 Oct | d+4 | 61.6 | 41.9 to 90.7 | 155 | 32.9 | 95 | +87% | **no** |
| Fri 16 Oct | d+5 | 62.0 | 42.1 to 91.4 | 156 | 45.6 | 126 | +36% | yes |
| Sat 17 Oct | d+6 | 62.2 | 42.3 to 91.3 | 156 | 59.7 | 154 | +4% | yes |
| Sun 18 Oct | d+7 | 62.3 | 42.3 to 91.7 | 156 | 57.4 | 152 | +9% | yes |

### Issued 2026-10-11

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 11 Oct | d+1 | 69.5 | 50.4 to 95.9 | 161 | 54.3 | 147 | +28% | yes |
| Mon 12 Oct | d+2 | 66.9 | 45.8 to 97.7 | 159 | 49.4 | 135 | +35% | yes |
| Tue 13 Oct | d+3 | 65.5 | 44.6 to 96.2 | 158 | 54.4 | 148 | +20% | yes |
| Wed 14 Oct | d+4 | 64.7 | 43.9 to 95.3 | 157 | 58.3 | 153 | +11% | yes |
| Thu 15 Oct | d+5 | 64.3 | 43.6 to 94.7 | 157 | 32.9 | 95 | +96% | **no** |
| Fri 16 Oct | d+6 | 64.0 | 43.6 to 94.0 | 157 | 45.6 | 126 | +40% | yes |
| Sat 17 Oct | d+7 | 63.9 | 43.4 to 94.0 | 157 | 59.7 | 154 | +7% | yes |

### Issued 2026-10-10

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 10 Oct | d+1 | 57.3 | 41.5 to 79.0 | 152 | 73.9 | 164 | -23% | yes |
| Sun 11 Oct | d+2 | 59.8 | 40.9 to 87.3 | 154 | 54.3 | 147 | +10% | yes |
| Mon 12 Oct | d+3 | 61.3 | 41.7 to 90.1 | 155 | 49.4 | 135 | +24% | yes |
| Tue 13 Oct | d+4 | 62.1 | 42.1 to 91.6 | 156 | 54.4 | 148 | +14% | yes |
| Wed 14 Oct | d+5 | 62.6 | 42.4 to 92.4 | 156 | 58.3 | 153 | +7% | yes |
| Thu 15 Oct | d+6 | 62.9 | 42.8 to 92.5 | 156 | 32.9 | 95 | +91% | **no** |
| Fri 16 Oct | d+7 | 63.1 | 42.8 to 92.9 | 156 | 45.6 | 126 | +38% | yes |

_46 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

