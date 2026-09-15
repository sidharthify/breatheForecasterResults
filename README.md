# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-09-16 03:18 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-09-15, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Wed 16 Sep | d+1 | 44.5 | 31.9 to 61.9 | 52.4 | 123 | Unhealthy for Sensitive Groups | drizzle, 23 to 30C, 1mm |
| Thu 17 Sep | d+2 | 47.0 | 31.9 to 69.2 | 55.3 | 129 | Unhealthy for Sensitive Groups | thunderstorm, 23 to 28C, 5mm |
| Fri 18 Sep | d+3 | 48.4 | 32.8 to 71.6 | 57.0 | 133 | Unhealthy for Sensitive Groups | cloudy, 22 to 30C |
| Sat 19 Sep | d+4 | 49.3 | 33.3 to 73.0 | 57.9 | 135 | Unhealthy for Sensitive Groups | clear, 21 to 31C |
| Sun 20 Sep | d+5 | 49.8 | 33.6 to 73.8 | 58.4 | 136 | Unhealthy for Sensitive Groups | clear, 22 to 31C |
| Mon 21 Sep | d+6 | 50.1 | 33.9 to 74.0 | 58.7 | 137 | Unhealthy for Sensitive Groups | clear, 22 to 32C |
| Tue 22 Sep | d+7 | 50.2 | 33.9 to 74.5 | 58.9 | 137 | Unhealthy for Sensitive Groups | clear, 23 to 31C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 23 | 10% | 11% | -5% | 100% | 65% | 100% |
| d+2 | 22 | 10% | 12% | -8% | 95% | 68% | 100% |
| d+3 | 21 | 11% | 13% | -10% | 100% | 71% | 100% |
| d+4 | 20 | 12% | 15% | -9% | 95% | 70% | 100% |
| d+5 | 19 | 13% | 14% | -12% | 95% | 74% | 100% |
| d+6 | 18 | 14% | 16% | -14% | 94% | 72% | 100% |
| d+7 | 17 | 15% | 18% | -16% | 88% | 65% | 100% |

Across all lead times the 80% range contained the truth **96%** of the time on **140** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-09-16

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 16 Sep | d+1 | 44.5 | 31.9 to 61.9 | 123 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+2 | 47.0 | 31.9 to 69.2 | 129 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+3 | 48.4 | 32.8 to 71.6 | 133 | pending | pending | n/a | n/a |
| Sat 19 Sep | d+4 | 49.3 | 33.3 to 73.0 | 135 | pending | pending | n/a | n/a |
| Sun 20 Sep | d+5 | 49.8 | 33.6 to 73.8 | 136 | pending | pending | n/a | n/a |
| Mon 21 Sep | d+6 | 50.1 | 33.9 to 74.0 | 137 | pending | pending | n/a | n/a |
| Tue 22 Sep | d+7 | 50.2 | 33.9 to 74.5 | 137 | pending | pending | n/a | n/a |

### Issued 2026-09-15

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 15 Sep | d+1 | 52.0 | 37.4 to 72.5 | 142 | 40.4 | 113 | +29% | yes |
| Wed 16 Sep | d+2 | 51.4 | 34.8 to 75.7 | 140 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+3 | 51.0 | 34.5 to 75.4 | 139 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+4 | 50.8 | 34.3 to 75.2 | 139 | pending | pending | n/a | n/a |
| Sat 19 Sep | d+5 | 50.7 | 34.1 to 75.2 | 138 | pending | pending | n/a | n/a |
| Sun 20 Sep | d+6 | 50.6 | 34.2 to 74.8 | 138 | pending | pending | n/a | n/a |
| Mon 21 Sep | d+7 | 50.5 | 34.1 to 75.0 | 138 | pending | pending | n/a | n/a |

### Issued 2026-09-14

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 14 Sep | d+1 | 54.6 | 39.2 to 76.1 | 148 | 53.3 | 145 | +3% | yes |
| Tue 15 Sep | d+2 | 52.5 | 35.5 to 77.4 | 143 | 40.4 | 113 | +30% | yes |
| Wed 16 Sep | d+3 | 51.3 | 34.6 to 75.9 | 140 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+4 | 50.6 | 34.1 to 75.0 | 138 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+5 | 50.2 | 33.8 to 74.6 | 137 | pending | pending | n/a | n/a |
| Sat 19 Sep | d+6 | 50.0 | 33.8 to 74.0 | 137 | pending | pending | n/a | n/a |
| Sun 20 Sep | d+7 | 49.9 | 33.6 to 74.1 | 136 | pending | pending | n/a | n/a |

### Issued 2026-09-13

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 13 Sep | d+1 | 55.1 | 39.5 to 76.9 | 149 | 58.6 | 153 | -6% | yes |
| Mon 14 Sep | d+2 | 52.3 | 35.4 to 77.2 | 142 | 53.3 | 145 | -2% | yes |
| Tue 15 Sep | d+3 | 50.7 | 34.2 to 75.1 | 138 | 40.4 | 113 | +26% | yes |
| Wed 16 Sep | d+4 | 49.9 | 33.6 to 74.0 | 136 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+5 | 49.4 | 33.2 to 73.4 | 135 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+6 | 49.1 | 33.2 to 72.7 | 134 | pending | pending | n/a | n/a |
| Sat 19 Sep | d+7 | 49.0 | 33.0 to 72.7 | 134 | pending | pending | n/a | n/a |

### Issued 2026-09-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 12 Sep | d+1 | 54.3 | 38.9 to 75.9 | 147 | 60.4 | 154 | -10% | yes |
| Sun 13 Sep | d+2 | 51.4 | 34.8 to 75.9 | 140 | 58.6 | 153 | -12% | yes |
| Mon 14 Sep | d+3 | 49.8 | 33.6 to 73.8 | 136 | 53.3 | 145 | -6% | yes |
| Tue 15 Sep | d+4 | 48.9 | 32.9 to 72.6 | 134 | 40.4 | 113 | +21% | yes |
| Wed 16 Sep | d+5 | 48.4 | 32.6 to 72.0 | 133 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+6 | 48.1 | 32.5 to 71.3 | 132 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+7 | 48.0 | 32.3 to 71.3 | 132 | pending | pending | n/a | n/a |

### Issued 2026-09-11

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 11 Sep | d+1 | 48.5 | 34.7 to 67.7 | 133 | 60.0 | 154 | -19% | yes |
| Sat 12 Sep | d+2 | 47.8 | 32.3 to 70.6 | 131 | 60.4 | 154 | -21% | yes |
| Sun 13 Sep | d+3 | 47.3 | 31.9 to 70.2 | 130 | 58.6 | 153 | -19% | yes |
| Mon 14 Sep | d+4 | 47.1 | 31.7 to 70.0 | 130 | 53.3 | 145 | -12% | yes |
| Tue 15 Sep | d+5 | 47.0 | 31.6 to 69.8 | 129 | 40.4 | 113 | +16% | yes |
| Wed 16 Sep | d+6 | 46.9 | 31.7 to 69.5 | 129 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+7 | 46.9 | 31.5 to 69.6 | 129 | pending | pending | n/a | n/a |

### Issued 2026-09-10

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 10 Sep | d+1 | 57.3 | 41.0 to 80.0 | 152 | 49.8 | 136 | +15% | yes |
| Fri 11 Sep | d+2 | 52.4 | 35.4 to 77.6 | 143 | 60.0 | 154 | -13% | yes |
| Sat 12 Sep | d+3 | 49.9 | 33.6 to 74.1 | 136 | 60.4 | 154 | -17% | yes |
| Sun 13 Sep | d+4 | 48.5 | 32.6 to 72.1 | 133 | 58.6 | 153 | -17% | yes |
| Mon 14 Sep | d+5 | 47.7 | 32.1 to 71.0 | 131 | 53.3 | 145 | -10% | yes |
| Tue 15 Sep | d+6 | 47.3 | 31.9 to 70.1 | 130 | 40.4 | 113 | +17% | yes |
| Wed 16 Sep | d+7 | 47.0 | 31.6 to 69.9 | 129 | pending | pending | n/a | n/a |

### Issued 2026-09-09

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 09 Sep | d+1 | 52.6 | 37.6 to 73.5 | 143 | 66.9 | 159 | -21% | yes |
| Thu 10 Sep | d+2 | 49.6 | 33.5 to 73.5 | 136 | 49.8 | 136 | -0% | yes |
| Fri 11 Sep | d+3 | 48.1 | 32.4 to 71.4 | 132 | 60.0 | 154 | -20% | yes |
| Sat 12 Sep | d+4 | 47.2 | 31.8 to 70.1 | 130 | 60.4 | 154 | -22% | yes |
| Sun 13 Sep | d+5 | 46.7 | 31.4 to 69.5 | 129 | 58.6 | 153 | -20% | yes |
| Mon 14 Sep | d+6 | 46.5 | 31.4 to 68.8 | 128 | 53.3 | 145 | -13% | yes |
| Tue 15 Sep | d+7 | 46.3 | 31.2 to 68.8 | 128 | 40.4 | 113 | +15% | yes |

### Issued 2026-09-08

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 08 Sep | d+1 | 44.9 | 32.1 to 62.8 | 124 | 58.1 | 153 | -23% | yes |
| Wed 09 Sep | d+2 | 45.1 | 30.5 to 66.8 | 125 | 66.9 | 159 | -33% | **no** |
| Thu 10 Sep | d+3 | 45.3 | 30.5 to 67.2 | 125 | 49.8 | 136 | -9% | yes |
| Fri 11 Sep | d+4 | 45.3 | 30.5 to 67.3 | 125 | 60.0 | 154 | -24% | yes |
| Sat 12 Sep | d+5 | 45.4 | 30.5 to 67.4 | 125 | 60.4 | 154 | -25% | yes |
| Sun 13 Sep | d+6 | 45.4 | 30.6 to 67.2 | 125 | 58.6 | 153 | -23% | yes |
| Mon 14 Sep | d+7 | 45.4 | 30.6 to 67.4 | 125 | 53.3 | 145 | -15% | yes |

### Issued 2026-09-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 07 Sep | d+1 | 46.3 | 33.1 to 64.8 | 128 | 44.5 | 123 | +4% | yes |
| Tue 08 Sep | d+2 | 45.6 | 30.7 to 67.6 | 126 | 58.1 | 153 | -22% | yes |
| Wed 09 Sep | d+3 | 45.2 | 30.4 to 67.2 | 125 | 66.9 | 159 | -32% | yes |
| Thu 10 Sep | d+4 | 45.0 | 30.2 to 66.9 | 124 | 49.8 | 136 | -10% | yes |
| Fri 11 Sep | d+5 | 44.9 | 30.1 to 66.8 | 124 | 60.0 | 154 | -25% | yes |
| Sat 12 Sep | d+6 | 44.8 | 30.2 to 66.4 | 124 | 60.4 | 154 | -26% | yes |
| Sun 13 Sep | d+7 | 44.8 | 30.1 to 66.5 | 124 | 58.6 | 153 | -24% | yes |

_14 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

