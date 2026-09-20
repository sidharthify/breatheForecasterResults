# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-09-21 02:36 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-09-20, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Mon 21 Sep | d+1 | 51.4 | 36.9 to 71.5 | 59.8 | 140 | Unhealthy for Sensitive Groups | clear, 22 to 33C |
| Tue 22 Sep | d+2 | 50.9 | 34.6 to 74.8 | 59.1 | 139 | Unhealthy for Sensitive Groups | clear, 23 to 33C |
| Wed 23 Sep | d+3 | 50.7 | 34.3 to 74.7 | 58.8 | 138 | Unhealthy for Sensitive Groups | cloudy, 24 to 33C |
| Thu 24 Sep | d+4 | 50.5 | 34.2 to 74.6 | 58.6 | 138 | Unhealthy for Sensitive Groups | cloudy, 24 to 33C |
| Fri 25 Sep | d+5 | 50.4 | 34.1 to 74.6 | 58.5 | 138 | Unhealthy for Sensitive Groups | cloudy, 23 to 32C |
| Sat 26 Sep | d+6 | 50.4 | 34.2 to 74.2 | 58.4 | 137 | Unhealthy for Sensitive Groups | clear, 21 to 33C |
| Sun 27 Sep | d+7 | 50.4 | 34.1 to 74.4 | 58.4 | 137 | Unhealthy for Sensitive Groups | clear, 22 to 32C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 28 | 10% | 13% | -3% | 96% | 68% | 100% |
| d+2 | 27 | 12% | 14% | -5% | 93% | 70% | 100% |
| d+3 | 26 | 11% | 15% | -5% | 96% | 73% | 100% |
| d+4 | 25 | 12% | 15% | -4% | 92% | 72% | 100% |
| d+5 | 24 | 12% | 15% | -6% | 92% | 75% | 100% |
| d+6 | 23 | 13% | 16% | -8% | 91% | 74% | 100% |
| d+7 | 22 | 14% | 17% | -10% | 86% | 68% | 100% |

Across all lead times the 80% range contained the truth **93%** of the time on **175** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-09-21

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 21 Sep | d+1 | 51.4 | 36.9 to 71.5 | 140 | pending | pending | n/a | n/a |
| Tue 22 Sep | d+2 | 50.9 | 34.6 to 74.8 | 139 | pending | pending | n/a | n/a |
| Wed 23 Sep | d+3 | 50.7 | 34.3 to 74.7 | 138 | pending | pending | n/a | n/a |
| Thu 24 Sep | d+4 | 50.5 | 34.2 to 74.6 | 138 | pending | pending | n/a | n/a |
| Fri 25 Sep | d+5 | 50.4 | 34.1 to 74.6 | 138 | pending | pending | n/a | n/a |
| Sat 26 Sep | d+6 | 50.4 | 34.2 to 74.2 | 138 | pending | pending | n/a | n/a |
| Sun 27 Sep | d+7 | 50.4 | 34.1 to 74.4 | 138 | pending | pending | n/a | n/a |

### Issued 2026-09-20

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 20 Sep | d+1 | 49.8 | 35.8 to 69.4 | 136 | 52.2 | 142 | -5% | yes |
| Mon 21 Sep | d+2 | 49.9 | 33.9 to 73.4 | 136 | pending | pending | n/a | n/a |
| Tue 22 Sep | d+3 | 49.9 | 33.8 to 73.7 | 136 | pending | pending | n/a | n/a |
| Wed 23 Sep | d+4 | 50.0 | 33.8 to 73.9 | 137 | pending | pending | n/a | n/a |
| Thu 24 Sep | d+5 | 50.0 | 33.8 to 74.0 | 137 | pending | pending | n/a | n/a |
| Fri 25 Sep | d+6 | 50.0 | 33.9 to 73.7 | 137 | pending | pending | n/a | n/a |
| Sat 26 Sep | d+7 | 50.0 | 33.8 to 73.9 | 137 | pending | pending | n/a | n/a |

### Issued 2026-09-19

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 19 Sep | d+1 | 46.0 | 33.0 to 64.2 | 127 | 49.7 | 136 | -7% | yes |
| Sun 20 Sep | d+2 | 47.6 | 32.3 to 70.1 | 131 | 52.2 | 142 | -9% | yes |
| Mon 21 Sep | d+3 | 48.5 | 32.8 to 71.7 | 133 | pending | pending | n/a | n/a |
| Tue 22 Sep | d+4 | 49.0 | 33.1 to 72.6 | 134 | pending | pending | n/a | n/a |
| Wed 23 Sep | d+5 | 49.3 | 33.3 to 73.1 | 135 | pending | pending | n/a | n/a |
| Thu 24 Sep | d+6 | 49.5 | 33.5 to 73.0 | 135 | pending | pending | n/a | n/a |
| Fri 25 Sep | d+7 | 49.6 | 33.5 to 73.4 | 136 | pending | pending | n/a | n/a |

### Issued 2026-09-18

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 18 Sep | d+1 | 38.1 | 27.3 to 53.1 | 107 | 43.4 | 120 | -12% | yes |
| Sat 19 Sep | d+2 | 42.9 | 29.1 to 63.3 | 119 | 49.7 | 136 | -14% | yes |
| Sun 20 Sep | d+3 | 45.9 | 31.0 to 68.0 | 127 | 52.2 | 142 | -12% | yes |
| Mon 21 Sep | d+4 | 47.7 | 32.2 to 70.7 | 131 | pending | pending | n/a | n/a |
| Tue 22 Sep | d+5 | 48.8 | 32.9 to 72.3 | 134 | pending | pending | n/a | n/a |
| Wed 23 Sep | d+6 | 49.4 | 33.4 to 72.9 | 135 | pending | pending | n/a | n/a |
| Thu 24 Sep | d+7 | 49.7 | 33.5 to 73.7 | 136 | pending | pending | n/a | n/a |

### Issued 2026-09-17

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 17 Sep | d+1 | 50.0 | 35.9 to 69.6 | 137 | 30.8 | 91 | +62% | **no** |
| Fri 18 Sep | d+2 | 50.6 | 34.4 to 74.6 | 138 | 43.4 | 120 | +17% | yes |
| Sat 19 Sep | d+3 | 51.0 | 34.5 to 75.3 | 139 | 49.7 | 136 | +3% | yes |
| Sun 20 Sep | d+4 | 51.2 | 34.6 to 75.7 | 140 | 52.2 | 142 | -2% | yes |
| Mon 21 Sep | d+5 | 51.3 | 34.6 to 76.0 | 140 | pending | pending | n/a | n/a |
| Tue 22 Sep | d+6 | 51.4 | 34.8 to 75.8 | 140 | pending | pending | n/a | n/a |
| Wed 23 Sep | d+7 | 51.4 | 34.7 to 76.1 | 140 | pending | pending | n/a | n/a |

### Issued 2026-09-16

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 16 Sep | d+1 | 44.5 | 31.9 to 61.9 | 123 | 49.0 | 134 | -9% | yes |
| Thu 17 Sep | d+2 | 47.0 | 31.9 to 69.2 | 129 | 30.8 | 91 | +53% | **no** |
| Fri 18 Sep | d+3 | 48.4 | 32.8 to 71.6 | 133 | 43.4 | 120 | +12% | yes |
| Sat 19 Sep | d+4 | 49.3 | 33.3 to 73.0 | 135 | 49.7 | 136 | -1% | yes |
| Sun 20 Sep | d+5 | 49.8 | 33.6 to 73.8 | 136 | 52.2 | 142 | -5% | yes |
| Mon 21 Sep | d+6 | 50.1 | 33.9 to 74.0 | 137 | pending | pending | n/a | n/a |
| Tue 22 Sep | d+7 | 50.2 | 33.9 to 74.5 | 137 | pending | pending | n/a | n/a |

### Issued 2026-09-15

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 15 Sep | d+1 | 52.0 | 37.4 to 72.5 | 142 | 40.4 | 113 | +29% | yes |
| Wed 16 Sep | d+2 | 51.4 | 34.8 to 75.7 | 140 | 49.0 | 134 | +5% | yes |
| Thu 17 Sep | d+3 | 51.0 | 34.5 to 75.4 | 139 | 30.8 | 91 | +66% | **no** |
| Fri 18 Sep | d+4 | 50.8 | 34.3 to 75.2 | 139 | 43.4 | 120 | +17% | yes |
| Sat 19 Sep | d+5 | 50.7 | 34.1 to 75.2 | 138 | 49.7 | 136 | +2% | yes |
| Sun 20 Sep | d+6 | 50.6 | 34.2 to 74.8 | 138 | 52.2 | 142 | -3% | yes |
| Mon 21 Sep | d+7 | 50.5 | 34.1 to 75.0 | 138 | pending | pending | n/a | n/a |

### Issued 2026-09-14

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 14 Sep | d+1 | 54.6 | 39.2 to 76.1 | 148 | 53.3 | 145 | +3% | yes |
| Tue 15 Sep | d+2 | 52.5 | 35.5 to 77.4 | 143 | 40.4 | 113 | +30% | yes |
| Wed 16 Sep | d+3 | 51.3 | 34.6 to 75.9 | 140 | 49.0 | 134 | +5% | yes |
| Thu 17 Sep | d+4 | 50.6 | 34.1 to 75.0 | 138 | 30.8 | 91 | +64% | **no** |
| Fri 18 Sep | d+5 | 50.2 | 33.8 to 74.6 | 137 | 43.4 | 120 | +16% | yes |
| Sat 19 Sep | d+6 | 50.0 | 33.8 to 74.0 | 137 | 49.7 | 136 | +1% | yes |
| Sun 20 Sep | d+7 | 49.9 | 33.6 to 74.1 | 136 | 52.2 | 142 | -4% | yes |

### Issued 2026-09-13

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 13 Sep | d+1 | 55.1 | 39.5 to 76.9 | 149 | 58.7 | 153 | -6% | yes |
| Mon 14 Sep | d+2 | 52.3 | 35.4 to 77.2 | 142 | 53.3 | 145 | -2% | yes |
| Tue 15 Sep | d+3 | 50.7 | 34.2 to 75.1 | 138 | 40.4 | 113 | +26% | yes |
| Wed 16 Sep | d+4 | 49.9 | 33.6 to 74.0 | 136 | 49.0 | 134 | +2% | yes |
| Thu 17 Sep | d+5 | 49.4 | 33.2 to 73.4 | 135 | 30.8 | 91 | +60% | **no** |
| Fri 18 Sep | d+6 | 49.1 | 33.2 to 72.7 | 134 | 43.4 | 120 | +13% | yes |
| Sat 19 Sep | d+7 | 49.0 | 33.0 to 72.7 | 134 | 49.7 | 136 | -1% | yes |

### Issued 2026-09-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 12 Sep | d+1 | 54.3 | 38.9 to 75.9 | 147 | 60.4 | 154 | -10% | yes |
| Sun 13 Sep | d+2 | 51.4 | 34.8 to 75.9 | 140 | 58.7 | 153 | -12% | yes |
| Mon 14 Sep | d+3 | 49.8 | 33.6 to 73.8 | 136 | 53.3 | 145 | -6% | yes |
| Tue 15 Sep | d+4 | 48.9 | 32.9 to 72.6 | 134 | 40.4 | 113 | +21% | yes |
| Wed 16 Sep | d+5 | 48.4 | 32.6 to 72.0 | 133 | 49.0 | 134 | -1% | yes |
| Thu 17 Sep | d+6 | 48.1 | 32.5 to 71.3 | 132 | 30.8 | 91 | +56% | **no** |
| Fri 18 Sep | d+7 | 48.0 | 32.3 to 71.3 | 132 | 43.4 | 120 | +11% | yes |

_19 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

