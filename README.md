# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-13 06:30 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-12, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Tue 13 Oct | d+1 | 54.7 | 39.7 to 75.5 | 63.0 | 148 | Unhealthy for Sensitive Groups | drizzle, 20 to 28C |
| Wed 14 Oct | d+2 | 57.8 | 39.6 to 84.3 | 66.5 | 153 | Unhealthy | drizzle, 17 to 28C, 2mm |
| Thu 15 Oct | d+3 | 59.6 | 40.6 to 87.5 | 68.5 | 154 | Unhealthy | showers, 17 to 26C, 3mm |
| Fri 16 Oct | d+4 | 60.7 | 41.2 to 89.3 | 69.7 | 155 | Unhealthy | clear, 15 to 27C |
| Sat 17 Oct | d+5 | 61.3 | 41.6 to 90.4 | 70.3 | 155 | Unhealthy | clear, 15 to 27C |
| Sun 18 Oct | d+6 | 61.7 | 42.0 to 90.6 | 70.6 | 155 | Unhealthy | clear, 14 to 27C |
| Mon 19 Oct | d+7 | 61.9 | 42.0 to 91.1 | 70.8 | 155 | Unhealthy | clear, 14 to 26C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 49 | 11% | 14% | -3% | 96% | 73% | 100% |
| d+2 | 48 | 13% | 16% | -5% | 92% | 67% | 100% |
| d+3 | 47 | 16% | 18% | -6% | 91% | 62% | 100% |
| d+4 | 46 | 18% | 19% | -6% | 89% | 59% | 100% |
| d+5 | 45 | 17% | 18% | -7% | 87% | 53% | 100% |
| d+6 | 44 | 18% | 19% | -9% | 86% | 57% | 100% |
| d+7 | 43 | 16% | 19% | -10% | 84% | 60% | 100% |

Across all lead times the 80% range contained the truth **89%** of the time on **322** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-13

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 13 Oct | d+1 | 54.7 | 39.7 to 75.5 | 148 | pending | pending | n/a | n/a |
| Wed 14 Oct | d+2 | 57.8 | 39.6 to 84.3 | 153 | pending | pending | n/a | n/a |
| Thu 15 Oct | d+3 | 59.6 | 40.6 to 87.5 | 154 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+4 | 60.7 | 41.2 to 89.3 | 155 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+5 | 61.3 | 41.6 to 90.4 | 155 | pending | pending | n/a | n/a |
| Sun 18 Oct | d+6 | 61.7 | 42.0 to 90.6 | 155 | pending | pending | n/a | n/a |
| Mon 19 Oct | d+7 | 61.9 | 42.0 to 91.1 | 155 | pending | pending | n/a | n/a |

### Issued 2026-10-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 12 Oct | d+1 | 57.9 | 42.0 to 79.9 | 153 | 49.7 | 136 | +16% | yes |
| Tue 13 Oct | d+2 | 59.8 | 41.0 to 87.3 | 154 | pending | pending | n/a | n/a |
| Wed 14 Oct | d+3 | 61.0 | 41.5 to 89.5 | 155 | pending | pending | n/a | n/a |
| Thu 15 Oct | d+4 | 61.6 | 41.9 to 90.7 | 155 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+5 | 62.0 | 42.1 to 91.4 | 156 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+6 | 62.2 | 42.3 to 91.3 | 156 | pending | pending | n/a | n/a |
| Sun 18 Oct | d+7 | 62.3 | 42.3 to 91.7 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-11

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 11 Oct | d+1 | 69.5 | 50.4 to 95.9 | 161 | 54.7 | 148 | +27% | yes |
| Mon 12 Oct | d+2 | 66.9 | 45.8 to 97.7 | 159 | 49.7 | 136 | +35% | yes |
| Tue 13 Oct | d+3 | 65.5 | 44.6 to 96.2 | 158 | pending | pending | n/a | n/a |
| Wed 14 Oct | d+4 | 64.7 | 43.9 to 95.3 | 157 | pending | pending | n/a | n/a |
| Thu 15 Oct | d+5 | 64.3 | 43.6 to 94.7 | 157 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+6 | 64.0 | 43.6 to 94.0 | 157 | pending | pending | n/a | n/a |
| Sat 17 Oct | d+7 | 63.9 | 43.4 to 94.0 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-10

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 10 Oct | d+1 | 57.3 | 41.5 to 79.0 | 152 | 74.2 | 164 | -23% | yes |
| Sun 11 Oct | d+2 | 59.8 | 40.9 to 87.3 | 154 | 54.7 | 148 | +9% | yes |
| Mon 12 Oct | d+3 | 61.3 | 41.7 to 90.1 | 155 | 49.7 | 136 | +23% | yes |
| Tue 13 Oct | d+4 | 62.1 | 42.1 to 91.6 | 156 | pending | pending | n/a | n/a |
| Wed 14 Oct | d+5 | 62.6 | 42.4 to 92.4 | 156 | pending | pending | n/a | n/a |
| Thu 15 Oct | d+6 | 62.9 | 42.8 to 92.5 | 156 | pending | pending | n/a | n/a |
| Fri 16 Oct | d+7 | 63.1 | 42.8 to 92.9 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-09

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 09 Oct | d+1 | 60.3 | 43.7 to 83.3 | 154 | 53.1 | 144 | +13% | yes |
| Sat 10 Oct | d+2 | 62.3 | 42.6 to 91.0 | 156 | 74.2 | 164 | -16% | yes |
| Sun 11 Oct | d+3 | 63.4 | 43.1 to 93.2 | 157 | 54.7 | 148 | +16% | yes |
| Mon 12 Oct | d+4 | 64.0 | 43.4 to 94.4 | 157 | 49.7 | 136 | +29% | yes |
| Tue 13 Oct | d+5 | 64.4 | 43.6 to 95.1 | 157 | pending | pending | n/a | n/a |
| Wed 14 Oct | d+6 | 64.6 | 43.9 to 95.1 | 157 | pending | pending | n/a | n/a |
| Thu 15 Oct | d+7 | 64.8 | 43.9 to 95.5 | 158 | pending | pending | n/a | n/a |

### Issued 2026-10-08

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 08 Oct | d+1 | 59.6 | 43.1 to 82.3 | 154 | 57.1 | 152 | +4% | yes |
| Fri 09 Oct | d+2 | 62.1 | 42.5 to 90.8 | 156 | 53.1 | 144 | +17% | yes |
| Sat 10 Oct | d+3 | 63.6 | 43.2 to 93.6 | 157 | 74.2 | 164 | -14% | yes |
| Sun 11 Oct | d+4 | 64.5 | 43.7 to 95.1 | 157 | 54.7 | 148 | +18% | yes |
| Mon 12 Oct | d+5 | 65.0 | 44.0 to 96.0 | 158 | 49.7 | 136 | +31% | yes |
| Tue 13 Oct | d+6 | 65.3 | 44.3 to 96.1 | 158 | pending | pending | n/a | n/a |
| Wed 14 Oct | d+7 | 65.5 | 44.3 to 96.6 | 158 | pending | pending | n/a | n/a |

### Issued 2026-10-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 07 Oct | d+1 | 73.4 | 53.1 to 101.3 | 164 | 55.3 | 150 | +33% | yes |
| Thu 08 Oct | d+2 | 70.9 | 48.5 to 103.7 | 162 | 57.1 | 152 | +24% | yes |
| Fri 09 Oct | d+3 | 69.6 | 47.3 to 102.3 | 161 | 53.1 | 144 | +31% | yes |
| Sat 10 Oct | d+4 | 68.8 | 46.6 to 101.5 | 160 | 74.2 | 164 | -7% | yes |
| Sun 11 Oct | d+5 | 68.4 | 46.2 to 101.1 | 160 | 54.7 | 148 | +25% | yes |
| Mon 12 Oct | d+6 | 68.1 | 46.2 to 100.4 | 160 | 49.7 | 136 | +37% | yes |
| Tue 13 Oct | d+7 | 68.0 | 46.0 to 100.4 | 160 | pending | pending | n/a | n/a |

### Issued 2026-10-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 06 Oct | d+1 | 83.8 | 60.6 to 115.8 | 171 | 77.8 | 167 | +8% | yes |
| Wed 07 Oct | d+2 | 76.7 | 52.4 to 112.3 | 166 | 55.3 | 150 | +39% | yes |
| Thu 08 Oct | d+3 | 73.0 | 49.6 to 107.4 | 163 | 57.1 | 152 | +28% | yes |
| Fri 09 Oct | d+4 | 70.9 | 48.0 to 104.7 | 162 | 53.1 | 144 | +33% | yes |
| Sat 10 Oct | d+5 | 69.7 | 47.1 to 103.2 | 161 | 74.2 | 164 | -6% | yes |
| Sun 11 Oct | d+6 | 69.1 | 46.9 to 101.8 | 161 | 54.7 | 148 | +26% | yes |
| Mon 12 Oct | d+7 | 68.7 | 46.5 to 101.5 | 160 | 49.7 | 136 | +38% | yes |

### Issued 2026-10-05

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 05 Oct | d+1 | 75.6 | 54.7 to 104.6 | 165 | 97.6 | 180 | -23% | yes |
| Tue 06 Oct | d+2 | 71.4 | 48.8 to 104.5 | 162 | 77.8 | 167 | -8% | yes |
| Wed 07 Oct | d+3 | 69.1 | 47.0 to 101.7 | 161 | 55.3 | 150 | +25% | yes |
| Thu 08 Oct | d+4 | 67.9 | 46.0 to 100.1 | 160 | 57.1 | 152 | +19% | yes |
| Fri 09 Oct | d+5 | 67.1 | 45.5 to 99.1 | 159 | 53.1 | 144 | +26% | yes |
| Sat 10 Oct | d+6 | 66.7 | 45.3 to 98.2 | 159 | 74.2 | 164 | -10% | yes |
| Sun 11 Oct | d+7 | 66.5 | 45.1 to 98.1 | 159 | 54.7 | 148 | +22% | yes |

### Issued 2026-10-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 04 Oct | d+1 | 67.9 | 49.1 to 93.9 | 160 | 83.5 | 171 | -19% | yes |
| Mon 05 Oct | d+2 | 66.2 | 45.2 to 96.8 | 159 | 97.6 | 180 | -32% | **no** |
| Tue 06 Oct | d+3 | 65.2 | 44.3 to 96.0 | 158 | 77.8 | 167 | -16% | yes |
| Wed 07 Oct | d+4 | 64.7 | 43.9 to 95.4 | 157 | 55.3 | 150 | +17% | yes |
| Thu 08 Oct | d+5 | 64.4 | 43.6 to 95.1 | 157 | 57.1 | 152 | +13% | yes |
| Fri 09 Oct | d+6 | 64.2 | 43.7 to 94.5 | 157 | 53.1 | 144 | +21% | yes |
| Sat 10 Oct | d+7 | 64.1 | 43.5 to 94.6 | 157 | 74.2 | 164 | -14% | yes |

_40 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

