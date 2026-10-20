# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-21 03:28 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-20, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Wed 21 Oct | d+1 | 66.3 | 48.0 to 91.4 | 74.6 | 159 | Unhealthy | clear, 16 to 28C |
| Thu 22 Oct | d+2 | 61.8 | 42.4 to 90.2 | 69.6 | 155 | Unhealthy | clear, 16 to 28C |
| Fri 23 Oct | d+3 | 59.4 | 40.5 to 87.2 | 67.1 | 154 | Unhealthy | clear, 15 to 28C |
| Sat 24 Oct | d+4 | 58.1 | 39.5 to 85.6 | 65.7 | 153 | Unhealthy | cloudy, 15 to 28C |
| Sun 25 Oct | d+5 | 57.4 | 38.9 to 84.7 | 65.0 | 152 | Unhealthy | clear, 15 to 28C |
| Mon 26 Oct | d+6 | 57.0 | 38.7 to 83.8 | 64.6 | 152 | Unhealthy | clear, 14 to 28C |
| Tue 27 Oct | d+7 | 56.7 | 38.5 to 83.7 | 64.3 | 152 | Unhealthy | clear, 14 to 28C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 57 | 12% | 15% | -4% | 95% | 74% | 98% |
| d+2 | 56 | 15% | 18% | -5% | 88% | 62% | 98% |
| d+3 | 55 | 19% | 19% | -5% | 89% | 65% | 98% |
| d+4 | 54 | 16% | 20% | -5% | 85% | 63% | 98% |
| d+5 | 53 | 17% | 20% | -6% | 85% | 60% | 98% |
| d+6 | 52 | 16% | 20% | -7% | 85% | 63% | 98% |
| d+7 | 51 | 16% | 21% | -7% | 86% | 61% | 98% |

Across all lead times the 80% range contained the truth **88%** of the time on **378** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-21

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 21 Oct | d+1 | 66.3 | 48.0 to 91.4 | 159 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+2 | 61.8 | 42.4 to 90.2 | 155 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+3 | 59.4 | 40.5 to 87.2 | 154 | pending | pending | n/a | n/a |
| Sat 24 Oct | d+4 | 58.1 | 39.5 to 85.6 | 153 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+5 | 57.4 | 38.9 to 84.7 | 152 | pending | pending | n/a | n/a |
| Mon 26 Oct | d+6 | 57.0 | 38.7 to 83.8 | 152 | pending | pending | n/a | n/a |
| Tue 27 Oct | d+7 | 56.7 | 38.5 to 83.7 | 152 | pending | pending | n/a | n/a |

### Issued 2026-10-20

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 20 Oct | d+1 | 61.7 | 44.7 to 85.2 | 155 | 74.9 | 165 | -18% | yes |
| Wed 21 Oct | d+2 | 59.3 | 40.6 to 86.4 | 154 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+3 | 57.9 | 39.5 to 85.0 | 153 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+4 | 57.2 | 38.8 to 84.1 | 152 | pending | pending | n/a | n/a |
| Sat 24 Oct | d+5 | 56.7 | 38.5 to 83.7 | 152 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+6 | 56.5 | 38.4 to 83.1 | 152 | pending | pending | n/a | n/a |
| Mon 26 Oct | d+7 | 56.4 | 38.2 to 83.2 | 152 | pending | pending | n/a | n/a |

### Issued 2026-10-19

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 19 Oct | d+1 | 57.3 | 41.5 to 79.1 | 152 | 66.2 | 159 | -13% | yes |
| Tue 20 Oct | d+2 | 57.3 | 39.2 to 83.6 | 152 | 74.9 | 165 | -23% | yes |
| Wed 21 Oct | d+3 | 57.3 | 39.0 to 84.1 | 152 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+4 | 57.3 | 38.9 to 84.3 | 152 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+5 | 57.3 | 38.8 to 84.5 | 152 | pending | pending | n/a | n/a |
| Sat 24 Oct | d+6 | 57.3 | 38.9 to 84.3 | 152 | pending | pending | n/a | n/a |
| Sun 25 Oct | d+7 | 57.3 | 38.8 to 84.5 | 152 | pending | pending | n/a | n/a |

### Issued 2026-10-18

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 18 Oct | d+1 | 59.2 | 42.9 to 81.9 | 154 | 57.4 | 152 | +3% | yes |
| Mon 19 Oct | d+2 | 58.9 | 40.3 to 86.1 | 153 | 66.2 | 159 | -11% | yes |
| Tue 20 Oct | d+3 | 58.7 | 40.0 to 86.3 | 153 | 74.9 | 165 | -22% | yes |
| Wed 21 Oct | d+4 | 58.6 | 39.8 to 86.4 | 153 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+5 | 58.6 | 39.6 to 86.5 | 153 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+6 | 58.5 | 39.7 to 86.2 | 153 | pending | pending | n/a | n/a |
| Sat 24 Oct | d+7 | 58.5 | 39.6 to 86.5 | 153 | pending | pending | n/a | n/a |

### Issued 2026-10-17

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 17 Oct | d+1 | 50.8 | 36.8 to 70.3 | 139 | 59.6 | 154 | -15% | yes |
| Sun 18 Oct | d+2 | 54.1 | 37.0 to 79.1 | 147 | 57.4 | 152 | -6% | yes |
| Mon 19 Oct | d+3 | 56.1 | 38.1 to 82.5 | 151 | 66.2 | 159 | -15% | yes |
| Tue 20 Oct | d+4 | 57.2 | 38.8 to 84.5 | 152 | 74.9 | 165 | -24% | yes |
| Wed 21 Oct | d+5 | 57.9 | 39.1 to 85.7 | 153 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+6 | 58.3 | 39.5 to 86.0 | 153 | pending | pending | n/a | n/a |
| Fri 23 Oct | d+7 | 58.5 | 39.5 to 86.6 | 153 | pending | pending | n/a | n/a |

### Issued 2026-10-16

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 16 Oct | d+1 | 43.0 | 31.1 to 59.4 | 119 | 45.9 | 127 | -6% | yes |
| Sat 17 Oct | d+2 | 50.0 | 34.2 to 73.1 | 137 | 59.6 | 154 | -16% | yes |
| Sun 18 Oct | d+3 | 54.5 | 37.1 to 80.1 | 148 | 57.4 | 152 | -5% | yes |
| Mon 19 Oct | d+4 | 57.2 | 38.8 to 84.4 | 152 | 66.2 | 159 | -14% | yes |
| Tue 20 Oct | d+5 | 58.8 | 39.8 to 86.9 | 153 | 74.9 | 165 | -21% | yes |
| Wed 21 Oct | d+6 | 59.7 | 40.5 to 88.0 | 154 | pending | pending | n/a | n/a |
| Thu 22 Oct | d+7 | 60.3 | 40.8 to 89.1 | 154 | pending | pending | n/a | n/a |

### Issued 2026-10-15

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 15 Oct | d+1 | 60.5 | 43.9 to 83.3 | 155 | 33.1 | 96 | +83% | **no** |
| Fri 16 Oct | d+2 | 61.8 | 42.4 to 90.0 | 155 | 45.9 | 127 | +35% | yes |
| Sat 17 Oct | d+3 | 62.5 | 42.6 to 91.6 | 156 | 59.6 | 154 | +5% | yes |
| Sun 18 Oct | d+4 | 62.9 | 42.8 to 92.5 | 156 | 57.4 | 152 | +10% | yes |
| Mon 19 Oct | d+5 | 63.2 | 42.9 to 93.0 | 156 | 66.2 | 159 | -5% | yes |
| Tue 20 Oct | d+6 | 63.3 | 43.2 to 93.0 | 156 | 74.9 | 165 | -15% | yes |
| Wed 21 Oct | d+7 | 63.4 | 43.1 to 93.3 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-14

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 14 Oct | d+1 | 57.9 | 42.0 to 79.8 | 153 | 58.4 | 153 | -1% | yes |
| Thu 15 Oct | d+2 | 60.0 | 41.2 to 87.5 | 154 | 33.1 | 96 | +81% | **no** |
| Fri 16 Oct | d+3 | 61.2 | 41.7 to 89.8 | 155 | 45.9 | 127 | +33% | yes |
| Sat 17 Oct | d+4 | 61.9 | 42.1 to 91.1 | 155 | 59.6 | 154 | +4% | yes |
| Sun 18 Oct | d+5 | 62.3 | 42.3 to 91.8 | 156 | 57.4 | 152 | +9% | yes |
| Mon 19 Oct | d+6 | 62.6 | 42.6 to 91.9 | 156 | 66.2 | 159 | -5% | yes |
| Tue 20 Oct | d+7 | 62.7 | 42.6 to 92.3 | 156 | 74.9 | 165 | -16% | yes |

### Issued 2026-10-13

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 13 Oct | d+1 | 54.7 | 39.7 to 75.5 | 148 | 55.2 | 149 | -1% | yes |
| Wed 14 Oct | d+2 | 57.8 | 39.6 to 84.3 | 153 | 58.4 | 153 | -1% | yes |
| Thu 15 Oct | d+3 | 59.6 | 40.6 to 87.5 | 154 | 33.1 | 96 | +80% | **no** |
| Fri 16 Oct | d+4 | 60.7 | 41.2 to 89.3 | 155 | 45.9 | 127 | +32% | yes |
| Sat 17 Oct | d+5 | 61.3 | 41.6 to 90.4 | 155 | 59.6 | 154 | +3% | yes |
| Sun 18 Oct | d+6 | 61.7 | 42.0 to 90.6 | 155 | 57.4 | 152 | +8% | yes |
| Mon 19 Oct | d+7 | 61.9 | 42.0 to 91.1 | 155 | 66.2 | 159 | -6% | yes |

### Issued 2026-10-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 12 Oct | d+1 | 57.9 | 42.0 to 79.9 | 153 | 51.1 | 139 | +13% | yes |
| Tue 13 Oct | d+2 | 59.8 | 41.0 to 87.3 | 154 | 55.2 | 149 | +8% | yes |
| Wed 14 Oct | d+3 | 61.0 | 41.5 to 89.5 | 155 | 58.4 | 153 | +4% | yes |
| Thu 15 Oct | d+4 | 61.6 | 41.9 to 90.7 | 155 | 33.1 | 96 | +86% | **no** |
| Fri 16 Oct | d+5 | 62.0 | 42.1 to 91.4 | 156 | 45.9 | 127 | +35% | yes |
| Sat 17 Oct | d+6 | 62.2 | 42.3 to 91.3 | 156 | 59.6 | 154 | +4% | yes |
| Sun 18 Oct | d+7 | 62.3 | 42.3 to 91.7 | 156 | 57.4 | 152 | +9% | yes |

_48 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

