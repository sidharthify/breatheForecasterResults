# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-15 03:28 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-14, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Thu 15 Oct | d+1 | 60.5 | 43.9 to 83.3 | 69.6 | 154 | Unhealthy | drizzle, 18 to 26C, 2mm |
| Fri 16 Oct | d+2 | 61.8 | 42.4 to 90.0 | 70.7 | 155 | Unhealthy | cloudy, 15 to 28C |
| Sat 17 Oct | d+3 | 62.5 | 42.6 to 91.6 | 71.4 | 156 | Unhealthy | clear, 15 to 28C |
| Sun 18 Oct | d+4 | 62.9 | 42.8 to 92.5 | 71.7 | 156 | Unhealthy | clear, 13 to 28C |
| Mon 19 Oct | d+5 | 63.2 | 42.9 to 93.0 | 71.9 | 156 | Unhealthy | clear, 14 to 28C |
| Tue 20 Oct | d+6 | 63.3 | 43.2 to 93.0 | 72.0 | 156 | Unhealthy | clear, 15 to 28C |
| Wed 21 Oct | d+7 | 63.4 | 43.1 to 93.3 | 72.0 | 157 | Unhealthy | clear, 16 to 29C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 51 | 11% | 13% | -3% | 96% | 71% | 100% |
| d+2 | 50 | 13% | 16% | -5% | 90% | 62% | 100% |
| d+3 | 49 | 16% | 18% | -5% | 92% | 63% | 100% |
| d+4 | 48 | 17% | 19% | -5% | 90% | 58% | 100% |
| d+5 | 47 | 16% | 18% | -7% | 87% | 55% | 100% |
| d+6 | 46 | 18% | 19% | -8% | 87% | 59% | 100% |
| d+7 | 45 | 16% | 19% | -9% | 84% | 56% | 100% |

Across all lead times the 80% range contained the truth **90%** of the time on **336** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-15

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 15 Oct | d+1 | 60.5 | 43.9 to 83.3 | 155 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+2 | 61.8 | 42.4 to 90.0 | 155 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+3 | 62.5 | 42.6 to 91.6 | 156 | pending | pending | n/a | n/a |
| Sun 18 Oct | d+4 | 62.9 | 42.8 to 92.5 | 156 | pending | pending | n/a | n/a |
| Mon 19 Oct | d+5 | 63.2 | 42.9 to 93.0 | 156 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+6 | 63.3 | 43.2 to 93.0 | 156 | pending | pending | n/a | n/a |
| Wed 21 Oct | d+7 | 63.4 | 43.1 to 93.3 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-14

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 14 Oct | d+1 | 57.9 | 42.0 to 79.8 | 153 | 58.3 | 153 | -1% | yes |
| Thu 15 Oct | d+2 | 60.0 | 41.2 to 87.5 | 154 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+3 | 61.2 | 41.7 to 89.8 | 155 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+4 | 61.9 | 42.1 to 91.1 | 155 | pending | pending | n/a | n/a |
| Sun 18 Oct | d+5 | 62.3 | 42.3 to 91.8 | 156 | pending | pending | n/a | n/a |
| Mon 19 Oct | d+6 | 62.6 | 42.6 to 91.9 | 156 | pending | pending | n/a | n/a |
| Tue 20 Oct | d+7 | 62.7 | 42.6 to 92.3 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-13

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 13 Oct | d+1 | 54.7 | 39.7 to 75.5 | 148 | 54.5 | 148 | +0% | yes |
| Wed 14 Oct | d+2 | 57.8 | 39.6 to 84.3 | 153 | 58.3 | 153 | -1% | yes |
| Thu 15 Oct | d+3 | 59.6 | 40.6 to 87.5 | 154 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+4 | 60.7 | 41.2 to 89.3 | 155 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+5 | 61.3 | 41.6 to 90.4 | 155 | pending | pending | n/a | n/a |
| Sun 18 Oct | d+6 | 61.7 | 42.0 to 90.6 | 155 | pending | pending | n/a | n/a |
| Mon 19 Oct | d+7 | 61.9 | 42.0 to 91.1 | 155 | pending | pending | n/a | n/a |

### Issued 2026-10-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 12 Oct | d+1 | 57.9 | 42.0 to 79.9 | 153 | 49.8 | 136 | +16% | yes |
| Tue 13 Oct | d+2 | 59.8 | 41.0 to 87.3 | 154 | 54.5 | 148 | +10% | yes |
| Wed 14 Oct | d+3 | 61.0 | 41.5 to 89.5 | 155 | 58.3 | 153 | +5% | yes |
| Thu 15 Oct | d+4 | 61.6 | 41.9 to 90.7 | 155 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+5 | 62.0 | 42.1 to 91.4 | 156 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+6 | 62.2 | 42.3 to 91.3 | 156 | pending | pending | n/a | n/a |
| Sun 18 Oct | d+7 | 62.3 | 42.3 to 91.7 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-11

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 11 Oct | d+1 | 69.5 | 50.4 to 95.9 | 161 | 54.9 | 149 | +27% | yes |
| Mon 12 Oct | d+2 | 66.9 | 45.8 to 97.7 | 159 | 49.8 | 136 | +34% | yes |
| Tue 13 Oct | d+3 | 65.5 | 44.6 to 96.2 | 158 | 54.5 | 148 | +20% | yes |
| Wed 14 Oct | d+4 | 64.7 | 43.9 to 95.3 | 157 | 58.3 | 153 | +11% | yes |
| Thu 15 Oct | d+5 | 64.3 | 43.6 to 94.7 | 157 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+6 | 64.0 | 43.6 to 94.0 | 157 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+7 | 63.9 | 43.4 to 94.0 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-10

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 10 Oct | d+1 | 57.3 | 41.5 to 79.0 | 152 | 74.5 | 164 | -23% | yes |
| Sun 11 Oct | d+2 | 59.8 | 40.9 to 87.3 | 154 | 54.9 | 149 | +9% | yes |
| Mon 12 Oct | d+3 | 61.3 | 41.7 to 90.1 | 155 | 49.8 | 136 | +23% | yes |
| Tue 13 Oct | d+4 | 62.1 | 42.1 to 91.6 | 156 | 54.5 | 148 | +14% | yes |
| Wed 14 Oct | d+5 | 62.6 | 42.4 to 92.4 | 156 | 58.3 | 153 | +7% | yes |
| Thu 15 Oct | d+6 | 62.9 | 42.8 to 92.5 | 156 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+7 | 63.1 | 42.8 to 92.9 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-09

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 09 Oct | d+1 | 60.3 | 43.7 to 83.3 | 154 | 53.3 | 145 | +13% | yes |
| Sat 10 Oct | d+2 | 62.3 | 42.6 to 91.0 | 156 | 74.5 | 164 | -16% | yes |
| Sun 11 Oct | d+3 | 63.4 | 43.1 to 93.2 | 157 | 54.9 | 149 | +16% | yes |
| Mon 12 Oct | d+4 | 64.0 | 43.4 to 94.4 | 157 | 49.8 | 136 | +28% | yes |
| Tue 13 Oct | d+5 | 64.4 | 43.6 to 95.1 | 157 | 54.5 | 148 | +18% | yes |
| Wed 14 Oct | d+6 | 64.6 | 43.9 to 95.1 | 157 | 58.3 | 153 | +11% | yes |
| Thu 15 Oct | d+7 | 64.8 | 43.9 to 95.5 | 158 | pending | pending | n/a | n/a |

### Issued 2026-10-08

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 08 Oct | d+1 | 59.6 | 43.1 to 82.3 | 154 | 57.3 | 152 | +4% | yes |
| Fri 09 Oct | d+2 | 62.1 | 42.5 to 90.8 | 156 | 53.3 | 145 | +16% | yes |
| Sat 10 Oct | d+3 | 63.6 | 43.2 to 93.6 | 157 | 74.5 | 164 | -15% | yes |
| Sun 11 Oct | d+4 | 64.5 | 43.7 to 95.1 | 157 | 54.9 | 149 | +18% | yes |
| Mon 12 Oct | d+5 | 65.0 | 44.0 to 96.0 | 158 | 49.8 | 136 | +30% | yes |
| Tue 13 Oct | d+6 | 65.3 | 44.3 to 96.1 | 158 | 54.5 | 148 | +20% | yes |
| Wed 14 Oct | d+7 | 65.5 | 44.3 to 96.6 | 158 | 58.3 | 153 | +12% | yes |

### Issued 2026-10-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 07 Oct | d+1 | 73.4 | 53.1 to 101.3 | 164 | 55.5 | 150 | +32% | yes |
| Thu 08 Oct | d+2 | 70.9 | 48.5 to 103.7 | 162 | 57.3 | 152 | +24% | yes |
| Fri 09 Oct | d+3 | 69.6 | 47.3 to 102.3 | 161 | 53.3 | 145 | +31% | yes |
| Sat 10 Oct | d+4 | 68.8 | 46.6 to 101.5 | 160 | 74.5 | 164 | -8% | yes |
| Sun 11 Oct | d+5 | 68.4 | 46.2 to 101.1 | 160 | 54.9 | 149 | +25% | yes |
| Mon 12 Oct | d+6 | 68.1 | 46.2 to 100.4 | 160 | 49.8 | 136 | +37% | yes |
| Tue 13 Oct | d+7 | 68.0 | 46.0 to 100.4 | 160 | 54.5 | 148 | +25% | yes |

### Issued 2026-10-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 06 Oct | d+1 | 83.8 | 60.6 to 115.8 | 171 | 78.1 | 167 | +7% | yes |
| Wed 07 Oct | d+2 | 76.7 | 52.4 to 112.3 | 166 | 55.5 | 150 | +38% | yes |
| Thu 08 Oct | d+3 | 73.0 | 49.6 to 107.4 | 163 | 57.3 | 152 | +27% | yes |
| Fri 09 Oct | d+4 | 70.9 | 48.0 to 104.7 | 162 | 53.3 | 145 | +33% | yes |
| Sat 10 Oct | d+5 | 69.7 | 47.1 to 103.2 | 161 | 74.5 | 164 | -6% | yes |
| Sun 11 Oct | d+6 | 69.1 | 46.9 to 101.8 | 161 | 54.9 | 149 | +26% | yes |
| Mon 12 Oct | d+7 | 68.7 | 46.5 to 101.5 | 160 | 49.8 | 136 | +38% | yes |

_42 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

