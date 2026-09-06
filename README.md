# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-09-07 02:24 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-09-06, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Mon 07 Sep | d+1 | 46.3 | 33.1 to 64.8 | 54.1 | 127 | Unhealthy for Sensitive Groups | clear, 23 to 31C |
| Tue 08 Sep | d+2 | 45.6 | 30.7 to 67.6 | 53.6 | 126 | Unhealthy for Sensitive Groups | clear, 23 to 32C |
| Wed 09 Sep | d+3 | 45.2 | 30.4 to 67.2 | 53.3 | 125 | Unhealthy for Sensitive Groups | drizzle, 24 to 32C |
| Thu 10 Sep | d+4 | 45.0 | 30.2 to 66.9 | 53.2 | 124 | Unhealthy for Sensitive Groups | drizzle, 25 to 32C, 2mm |
| Fri 11 Sep | d+5 | 44.9 | 30.1 to 66.8 | 53.1 | 124 | Unhealthy for Sensitive Groups | cloudy, 25 to 33C |
| Sat 12 Sep | d+6 | 44.8 | 30.2 to 66.4 | 53.0 | 124 | Unhealthy for Sensitive Groups | drizzle, 25 to 33C |
| Sun 13 Sep | d+7 | 44.8 | 30.1 to 66.5 | 53.0 | 124 | Unhealthy for Sensitive Groups | drizzle, 24 to 31C, 1mm |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 14 | 6% | 9% | -7% | 100% | 86% | 100% |
| d+2 | 13 | 7% | 11% | -8% | 100% | 85% | 100% |
| d+3 | 12 | 10% | 11% | -9% | 100% | 92% | 100% |
| d+4 | 11 | 9% | 11% | -5% | 100% | 91% | 100% |
| d+5 | 10 | 9% | 9% | -8% | 100% | 100% | 100% |
| d+6 | 9 | 11% | 12% | -10% | 100% | 100% | 100% |
| d+7 | 8 | 12% | 14% | -13% | 88% | 88% | 100% |

Across all lead times the 80% range contained the truth **99%** of the time on **77** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-09-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 07 Sep | d+1 | 46.3 | 33.1 to 64.8 | 128 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+2 | 45.6 | 30.7 to 67.6 | 126 | pending | pending | n/a | n/a |
| Wed 09 Sep | d+3 | 45.2 | 30.4 to 67.2 | 125 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+4 | 45.0 | 30.2 to 66.9 | 124 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+5 | 44.9 | 30.1 to 66.8 | 124 | pending | pending | n/a | n/a |
| Sat 12 Sep | d+6 | 44.8 | 30.2 to 66.4 | 124 | pending | pending | n/a | n/a |
| Sun 13 Sep | d+7 | 44.8 | 30.1 to 66.5 | 124 | pending | pending | n/a | n/a |

### Issued 2026-09-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 06 Sep | d+1 | 44.5 | 31.8 to 62.4 | 123 | 47.5 | 131 | -6% | yes |
| Mon 07 Sep | d+2 | 43.9 | 29.6 to 65.2 | 122 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+3 | 43.6 | 29.3 to 64.9 | 121 | pending | pending | n/a | n/a |
| Wed 09 Sep | d+4 | 43.4 | 29.2 to 64.6 | 120 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+5 | 43.3 | 29.1 to 64.5 | 120 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+6 | 43.2 | 29.1 to 64.2 | 120 | pending | pending | n/a | n/a |
| Sat 12 Sep | d+7 | 43.2 | 29.0 to 64.3 | 120 | pending | pending | n/a | n/a |

### Issued 2026-09-05

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 05 Sep | d+1 | 46.5 | 33.1 to 65.2 | 128 | 45.6 | 126 | +2% | yes |
| Sun 06 Sep | d+2 | 44.9 | 30.2 to 66.8 | 124 | 47.5 | 131 | -6% | yes |
| Mon 07 Sep | d+3 | 44.1 | 29.6 to 65.7 | 122 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+4 | 43.6 | 29.3 to 65.0 | 121 | pending | pending | n/a | n/a |
| Wed 09 Sep | d+5 | 43.4 | 29.1 to 64.7 | 120 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+6 | 43.2 | 29.1 to 64.2 | 120 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+7 | 43.1 | 29.0 to 64.2 | 120 | pending | pending | n/a | n/a |

### Issued 2026-09-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 04 Sep | d+1 | 43.4 | 31.0 to 61.0 | 120 | 49.3 | 135 | -12% | yes |
| Sat 05 Sep | d+2 | 43.0 | 28.9 to 64.0 | 119 | 45.6 | 126 | -6% | yes |
| Sun 06 Sep | d+3 | 42.8 | 28.7 to 63.8 | 119 | 47.5 | 131 | -10% | yes |
| Mon 07 Sep | d+4 | 42.7 | 28.6 to 63.7 | 119 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+5 | 42.6 | 28.5 to 63.6 | 118 | pending | pending | n/a | n/a |
| Wed 09 Sep | d+6 | 42.6 | 28.6 to 63.3 | 118 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+7 | 42.5 | 28.5 to 63.4 | 118 | pending | pending | n/a | n/a |

### Issued 2026-09-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 03 Sep | d+1 | 39.4 | 28.1 to 55.3 | 111 | 44.2 | 122 | -11% | yes |
| Fri 04 Sep | d+2 | 40.7 | 27.3 to 60.5 | 114 | 49.3 | 135 | -17% | yes |
| Sat 05 Sep | d+3 | 41.4 | 27.7 to 61.8 | 116 | 45.6 | 126 | -9% | yes |
| Sun 06 Sep | d+4 | 41.8 | 28.0 to 62.4 | 117 | 47.5 | 131 | -12% | yes |
| Mon 07 Sep | d+5 | 42.0 | 28.1 to 62.8 | 117 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+6 | 42.2 | 28.3 to 62.8 | 117 | pending | pending | n/a | n/a |
| Wed 09 Sep | d+7 | 42.2 | 28.3 to 63.0 | 117 | pending | pending | n/a | n/a |

### Issued 2026-09-02

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 02 Sep | d+1 | 41.2 | 29.3 to 58.0 | 115 | 37.2 | 105 | +11% | yes |
| Thu 03 Sep | d+2 | 41.4 | 27.8 to 61.7 | 116 | 44.2 | 122 | -6% | yes |
| Fri 04 Sep | d+3 | 41.5 | 27.7 to 62.0 | 116 | 49.3 | 135 | -16% | yes |
| Sat 05 Sep | d+4 | 41.5 | 27.8 to 62.1 | 116 | 45.6 | 126 | -9% | yes |
| Sun 06 Sep | d+5 | 41.5 | 27.8 to 62.2 | 116 | 47.5 | 131 | -13% | yes |
| Mon 07 Sep | d+6 | 41.6 | 27.9 to 61.9 | 116 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+7 | 41.6 | 27.8 to 62.1 | 116 | pending | pending | n/a | n/a |

### Issued 2026-09-01

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 01 Sep | d+1 | 42.4 | 30.1 to 59.7 | 118 | 41.0 | 114 | +3% | yes |
| Wed 02 Sep | d+2 | 42.0 | 28.2 to 62.7 | 117 | 37.2 | 105 | +13% | yes |
| Thu 03 Sep | d+3 | 41.8 | 27.9 to 62.5 | 117 | 44.2 | 122 | -5% | yes |
| Fri 04 Sep | d+4 | 41.7 | 27.8 to 62.4 | 116 | 49.3 | 135 | -15% | yes |
| Sat 05 Sep | d+5 | 41.6 | 27.8 to 62.3 | 116 | 45.6 | 126 | -9% | yes |
| Sun 06 Sep | d+6 | 41.6 | 27.9 to 62.0 | 116 | 47.5 | 131 | -12% | yes |
| Mon 07 Sep | d+7 | 41.5 | 27.8 to 62.1 | 116 | pending | pending | n/a | n/a |

### Issued 2026-08-31

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 31 Aug | d+1 | 42.8 | 30.4 to 60.3 | 119 | 43.1 | 120 | -1% | yes |
| Tue 01 Sep | d+2 | 41.8 | 28.0 to 62.5 | 117 | 41.0 | 114 | +2% | yes |
| Wed 02 Sep | d+3 | 41.3 | 27.6 to 61.8 | 115 | 37.2 | 105 | +11% | yes |
| Thu 03 Sep | d+4 | 41.0 | 27.3 to 61.4 | 115 | 44.2 | 122 | -7% | yes |
| Fri 04 Sep | d+5 | 40.8 | 27.2 to 61.2 | 114 | 49.3 | 135 | -17% | yes |
| Sat 05 Sep | d+6 | 40.7 | 27.3 to 60.8 | 114 | 45.6 | 126 | -11% | yes |
| Sun 06 Sep | d+7 | 40.7 | 27.2 to 60.9 | 114 | 47.5 | 131 | -14% | yes |

### Issued 2026-08-30

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 30 Aug | d+1 | 42.9 | 30.5 to 60.5 | 119 | 44.5 | 123 | -4% | yes |
| Mon 31 Aug | d+2 | 41.7 | 27.9 to 62.4 | 116 | 43.1 | 120 | -3% | yes |
| Tue 01 Sep | d+3 | 41.1 | 27.4 to 61.6 | 115 | 41.0 | 114 | +0% | yes |
| Wed 02 Sep | d+4 | 40.7 | 27.1 to 61.1 | 114 | 37.2 | 105 | +9% | yes |
| Thu 03 Sep | d+5 | 40.5 | 27.0 to 60.8 | 113 | 44.2 | 122 | -8% | yes |
| Fri 04 Sep | d+6 | 40.4 | 27.0 to 60.4 | 113 | 49.3 | 135 | -18% | yes |
| Sat 05 Sep | d+7 | 40.3 | 26.9 to 60.4 | 113 | 45.6 | 126 | -12% | yes |

### Issued 2026-08-29

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 29 Aug | d+1 | 42.7 | 30.3 to 60.3 | 119 | 45.1 | 125 | -5% | yes |
| Sun 30 Aug | d+2 | 41.5 | 27.7 to 62.1 | 116 | 44.5 | 123 | -7% | yes |
| Mon 31 Aug | d+3 | 40.8 | 27.2 to 61.3 | 114 | 43.1 | 120 | -5% | yes |
| Tue 01 Sep | d+4 | 40.4 | 26.9 to 60.8 | 113 | 41.0 | 114 | -1% | yes |
| Wed 02 Sep | d+5 | 40.2 | 26.8 to 60.5 | 113 | 37.2 | 105 | +8% | yes |
| Thu 03 Sep | d+6 | 40.1 | 26.8 to 60.0 | 112 | 44.2 | 122 | -9% | yes |
| Fri 04 Sep | d+7 | 40.0 | 26.7 to 60.1 | 112 | 49.3 | 135 | -19% | yes |

_5 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

