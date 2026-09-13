# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-09-14 02:41 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-09-13, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Mon 14 Sep | d+1 | 54.6 | 39.2 to 76.1 | 63.4 | 148 | Unhealthy for Sensitive Groups | thunderstorm, 24 to 31C |
| Tue 15 Sep | d+2 | 52.5 | 35.5 to 77.4 | 61.1 | 143 | Unhealthy for Sensitive Groups | thunderstorm, 23 to 30C, 3mm |
| Wed 16 Sep | d+3 | 51.3 | 34.6 to 75.9 | 59.9 | 140 | Unhealthy for Sensitive Groups | thunderstorm, 23 to 28C, 4mm |
| Thu 17 Sep | d+4 | 50.6 | 34.1 to 75.0 | 59.2 | 138 | Unhealthy for Sensitive Groups | drizzle, 22 to 30C, 4mm |
| Fri 18 Sep | d+5 | 50.2 | 33.8 to 74.6 | 58.8 | 137 | Unhealthy for Sensitive Groups | cloudy, 22 to 29C |
| Sat 19 Sep | d+6 | 50.0 | 33.8 to 74.0 | 58.6 | 137 | Unhealthy for Sensitive Groups | clear, 22 to 30C |
| Sun 20 Sep | d+7 | 49.9 | 33.6 to 74.1 | 58.5 | 136 | Unhealthy for Sensitive Groups | clear, 22 to 31C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 21 | 10% | 11% | -7% | 100% | 62% | 100% |
| d+2 | 20 | 10% | 12% | -10% | 95% | 65% | 100% |
| d+3 | 19 | 11% | 13% | -12% | 100% | 68% | 100% |
| d+4 | 18 | 12% | 14% | -11% | 94% | 67% | 100% |
| d+5 | 17 | 13% | 14% | -13% | 94% | 71% | 100% |
| d+6 | 16 | 14% | 17% | -16% | 94% | 69% | 100% |
| d+7 | 15 | 15% | 19% | -18% | 87% | 60% | 100% |

Across all lead times the 80% range contained the truth **95%** of the time on **126** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-09-14

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 14 Sep | d+1 | 54.6 | 39.2 to 76.1 | 148 | pending | pending | n/a | n/a |
| Tue 15 Sep | d+2 | 52.5 | 35.5 to 77.4 | 143 | pending | pending | n/a | n/a |
| Wed 16 Sep | d+3 | 51.3 | 34.6 to 75.9 | 140 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+4 | 50.6 | 34.1 to 75.0 | 138 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+5 | 50.2 | 33.8 to 74.6 | 137 | pending | pending | n/a | n/a |
| Sat 19 Sep | d+6 | 50.0 | 33.8 to 74.0 | 137 | pending | pending | n/a | n/a |
| Sun 20 Sep | d+7 | 49.9 | 33.6 to 74.1 | 136 | pending | pending | n/a | n/a |

### Issued 2026-09-13

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 13 Sep | d+1 | 55.1 | 39.5 to 76.9 | 149 | 58.7 | 153 | -6% | yes |
| Mon 14 Sep | d+2 | 52.3 | 35.4 to 77.2 | 142 | pending | pending | n/a | n/a |
| Tue 15 Sep | d+3 | 50.7 | 34.2 to 75.1 | 138 | pending | pending | n/a | n/a |
| Wed 16 Sep | d+4 | 49.9 | 33.6 to 74.0 | 136 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+5 | 49.4 | 33.2 to 73.4 | 135 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+6 | 49.1 | 33.2 to 72.7 | 134 | pending | pending | n/a | n/a |
| Sat 19 Sep | d+7 | 49.0 | 33.0 to 72.7 | 134 | pending | pending | n/a | n/a |

### Issued 2026-09-12

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 12 Sep | d+1 | 54.3 | 38.9 to 75.9 | 147 | 60.5 | 154 | -10% | yes |
| Sun 13 Sep | d+2 | 51.4 | 34.8 to 75.9 | 140 | 58.7 | 153 | -12% | yes |
| Mon 14 Sep | d+3 | 49.8 | 33.6 to 73.8 | 136 | pending | pending | n/a | n/a |
| Tue 15 Sep | d+4 | 48.9 | 32.9 to 72.6 | 134 | pending | pending | n/a | n/a |
| Wed 16 Sep | d+5 | 48.4 | 32.6 to 72.0 | 133 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+6 | 48.1 | 32.5 to 71.3 | 132 | pending | pending | n/a | n/a |
| Fri 18 Sep | d+7 | 48.0 | 32.3 to 71.3 | 132 | pending | pending | n/a | n/a |

### Issued 2026-09-11

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 11 Sep | d+1 | 48.5 | 34.7 to 67.7 | 133 | 60.0 | 154 | -19% | yes |
| Sat 12 Sep | d+2 | 47.8 | 32.3 to 70.6 | 131 | 60.5 | 154 | -21% | yes |
| Sun 13 Sep | d+3 | 47.3 | 31.9 to 70.2 | 130 | 58.7 | 153 | -19% | yes |
| Mon 14 Sep | d+4 | 47.1 | 31.7 to 70.0 | 130 | pending | pending | n/a | n/a |
| Tue 15 Sep | d+5 | 47.0 | 31.6 to 69.8 | 129 | pending | pending | n/a | n/a |
| Wed 16 Sep | d+6 | 46.9 | 31.7 to 69.5 | 129 | pending | pending | n/a | n/a |
| Thu 17 Sep | d+7 | 46.9 | 31.5 to 69.6 | 129 | pending | pending | n/a | n/a |

### Issued 2026-09-10

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 10 Sep | d+1 | 57.3 | 41.0 to 80.0 | 152 | 49.8 | 136 | +15% | yes |
| Fri 11 Sep | d+2 | 52.4 | 35.4 to 77.6 | 143 | 60.0 | 154 | -13% | yes |
| Sat 12 Sep | d+3 | 49.9 | 33.6 to 74.1 | 136 | 60.5 | 154 | -17% | yes |
| Sun 13 Sep | d+4 | 48.5 | 32.6 to 72.1 | 133 | 58.7 | 153 | -17% | yes |
| Mon 14 Sep | d+5 | 47.7 | 32.1 to 71.0 | 131 | pending | pending | n/a | n/a |
| Tue 15 Sep | d+6 | 47.3 | 31.9 to 70.1 | 130 | pending | pending | n/a | n/a |
| Wed 16 Sep | d+7 | 47.0 | 31.6 to 69.9 | 129 | pending | pending | n/a | n/a |

### Issued 2026-09-09

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 09 Sep | d+1 | 52.6 | 37.6 to 73.5 | 143 | 66.9 | 159 | -21% | yes |
| Thu 10 Sep | d+2 | 49.6 | 33.5 to 73.5 | 136 | 49.8 | 136 | -0% | yes |
| Fri 11 Sep | d+3 | 48.1 | 32.4 to 71.4 | 132 | 60.0 | 154 | -20% | yes |
| Sat 12 Sep | d+4 | 47.2 | 31.8 to 70.1 | 130 | 60.5 | 154 | -22% | yes |
| Sun 13 Sep | d+5 | 46.7 | 31.4 to 69.5 | 129 | 58.7 | 153 | -20% | yes |
| Mon 14 Sep | d+6 | 46.5 | 31.4 to 68.8 | 128 | pending | pending | n/a | n/a |
| Tue 15 Sep | d+7 | 46.3 | 31.2 to 68.8 | 128 | pending | pending | n/a | n/a |

### Issued 2026-09-08

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 08 Sep | d+1 | 44.9 | 32.1 to 62.8 | 124 | 58.1 | 153 | -23% | yes |
| Wed 09 Sep | d+2 | 45.1 | 30.5 to 66.8 | 125 | 66.9 | 159 | -33% | **no** |
| Thu 10 Sep | d+3 | 45.3 | 30.5 to 67.2 | 125 | 49.8 | 136 | -9% | yes |
| Fri 11 Sep | d+4 | 45.3 | 30.5 to 67.3 | 125 | 60.0 | 154 | -24% | yes |
| Sat 12 Sep | d+5 | 45.4 | 30.5 to 67.4 | 125 | 60.5 | 154 | -25% | yes |
| Sun 13 Sep | d+6 | 45.4 | 30.6 to 67.2 | 125 | 58.7 | 153 | -23% | yes |
| Mon 14 Sep | d+7 | 45.4 | 30.6 to 67.4 | 125 | pending | pending | n/a | n/a |

### Issued 2026-09-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 07 Sep | d+1 | 46.3 | 33.1 to 64.8 | 128 | 44.5 | 123 | +4% | yes |
| Tue 08 Sep | d+2 | 45.6 | 30.7 to 67.6 | 126 | 58.1 | 153 | -22% | yes |
| Wed 09 Sep | d+3 | 45.2 | 30.4 to 67.2 | 125 | 66.9 | 159 | -32% | yes |
| Thu 10 Sep | d+4 | 45.0 | 30.2 to 66.9 | 124 | 49.8 | 136 | -10% | yes |
| Fri 11 Sep | d+5 | 44.9 | 30.1 to 66.8 | 124 | 60.0 | 154 | -25% | yes |
| Sat 12 Sep | d+6 | 44.8 | 30.2 to 66.4 | 124 | 60.5 | 154 | -26% | yes |
| Sun 13 Sep | d+7 | 44.8 | 30.1 to 66.5 | 124 | 58.7 | 153 | -24% | yes |

### Issued 2026-09-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 06 Sep | d+1 | 44.5 | 31.8 to 62.4 | 123 | 47.5 | 130 | -6% | yes |
| Mon 07 Sep | d+2 | 43.9 | 29.6 to 65.2 | 122 | 44.5 | 123 | -1% | yes |
| Tue 08 Sep | d+3 | 43.6 | 29.3 to 64.9 | 121 | 58.1 | 153 | -25% | yes |
| Wed 09 Sep | d+4 | 43.4 | 29.2 to 64.6 | 120 | 66.9 | 159 | -35% | **no** |
| Thu 10 Sep | d+5 | 43.3 | 29.1 to 64.5 | 120 | 49.8 | 136 | -13% | yes |
| Fri 11 Sep | d+6 | 43.2 | 29.1 to 64.2 | 120 | 60.0 | 154 | -28% | yes |
| Sat 12 Sep | d+7 | 43.2 | 29.0 to 64.3 | 120 | 60.5 | 154 | -29% | yes |

### Issued 2026-09-05

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 05 Sep | d+1 | 46.5 | 33.1 to 65.2 | 128 | 45.6 | 126 | +2% | yes |
| Sun 06 Sep | d+2 | 44.9 | 30.2 to 66.8 | 124 | 47.5 | 130 | -5% | yes |
| Mon 07 Sep | d+3 | 44.1 | 29.6 to 65.7 | 122 | 44.5 | 123 | -1% | yes |
| Tue 08 Sep | d+4 | 43.6 | 29.3 to 65.0 | 121 | 58.1 | 153 | -25% | yes |
| Wed 09 Sep | d+5 | 43.4 | 29.1 to 64.7 | 120 | 66.9 | 159 | -35% | **no** |
| Thu 10 Sep | d+6 | 43.2 | 29.1 to 64.2 | 120 | 49.8 | 136 | -13% | yes |
| Fri 11 Sep | d+7 | 43.1 | 29.0 to 64.2 | 120 | 60.0 | 154 | -28% | yes |

_12 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

