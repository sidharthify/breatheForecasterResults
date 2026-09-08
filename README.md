# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-09-09 02:59 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-09-08, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Wed 09 Sep | d+1 | 52.6 | 37.6 to 73.5 | 61.5 | 143 | Unhealthy for Sensitive Groups | thunderstorm, 24 to 32C, 1mm |
| Thu 10 Sep | d+2 | 49.6 | 33.5 to 73.5 | 58.3 | 136 | Unhealthy for Sensitive Groups | cloudy, 25 to 33C |
| Fri 11 Sep | d+3 | 48.1 | 32.4 to 71.4 | 56.6 | 132 | Unhealthy for Sensitive Groups | drizzle, 25 to 33C |
| Sat 12 Sep | d+4 | 47.2 | 31.8 to 70.1 | 55.7 | 130 | Unhealthy for Sensitive Groups | drizzle, 25 to 33C |
| Sun 13 Sep | d+5 | 46.7 | 31.4 to 69.5 | 55.3 | 129 | Unhealthy for Sensitive Groups | drizzle, 24 to 33C, 2mm |
| Mon 14 Sep | d+6 | 46.5 | 31.4 to 68.8 | 55.0 | 128 | Unhealthy for Sensitive Groups | drizzle, 24 to 30C |
| Tue 15 Sep | d+7 | 46.3 | 31.2 to 68.8 | 54.9 | 128 | Unhealthy for Sensitive Groups | drizzle, 24 to 30C, 1mm |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 16 | 6% | 10% | -7% | 100% | 81% | 100% |
| d+2 | 15 | 7% | 11% | -9% | 100% | 80% | 100% |
| d+3 | 14 | 10% | 11% | -9% | 100% | 86% | 100% |
| d+4 | 13 | 9% | 12% | -7% | 100% | 85% | 100% |
| d+5 | 12 | 9% | 11% | -9% | 100% | 92% | 100% |
| d+6 | 11 | 11% | 13% | -12% | 100% | 91% | 100% |
| d+7 | 10 | 12% | 15% | -14% | 90% | 80% | 100% |

Across all lead times the 80% range contained the truth **99%** of the time on **91** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-09-09

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 09 Sep | d+1 | 52.6 | 37.6 to 73.5 | 143 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+2 | 49.6 | 33.5 to 73.5 | 136 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+3 | 48.1 | 32.4 to 71.4 | 132 | pending | pending | n/a | n/a |
| Sat 12 Sep | d+4 | 47.2 | 31.8 to 70.1 | 130 | pending | pending | n/a | n/a |
| Sun 13 Sep | d+5 | 46.7 | 31.4 to 69.5 | 129 | pending | pending | n/a | n/a |
| Mon 14 Sep | d+6 | 46.5 | 31.4 to 68.8 | 128 | pending | pending | n/a | n/a |
| Tue 15 Sep | d+7 | 46.3 | 31.2 to 68.8 | 128 | pending | pending | n/a | n/a |

### Issued 2026-09-08

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 08 Sep | d+1 | 44.9 | 32.1 to 62.8 | 124 | 58.1 | 153 | -23% | yes |
| Wed 09 Sep | d+2 | 45.1 | 30.5 to 66.8 | 125 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+3 | 45.3 | 30.5 to 67.2 | 125 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+4 | 45.3 | 30.5 to 67.3 | 125 | pending | pending | n/a | n/a |
| Sat 12 Sep | d+5 | 45.4 | 30.5 to 67.4 | 125 | pending | pending | n/a | n/a |
| Sun 13 Sep | d+6 | 45.4 | 30.6 to 67.2 | 125 | pending | pending | n/a | n/a |
| Mon 14 Sep | d+7 | 45.4 | 30.6 to 67.4 | 125 | pending | pending | n/a | n/a |

### Issued 2026-09-07

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 07 Sep | d+1 | 46.3 | 33.1 to 64.8 | 128 | 44.6 | 123 | +4% | yes |
| Tue 08 Sep | d+2 | 45.6 | 30.7 to 67.6 | 126 | 58.1 | 153 | -22% | yes |
| Wed 09 Sep | d+3 | 45.2 | 30.4 to 67.2 | 125 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+4 | 45.0 | 30.2 to 66.9 | 124 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+5 | 44.9 | 30.1 to 66.8 | 124 | pending | pending | n/a | n/a |
| Sat 12 Sep | d+6 | 44.8 | 30.2 to 66.4 | 124 | pending | pending | n/a | n/a |
| Sun 13 Sep | d+7 | 44.8 | 30.1 to 66.5 | 124 | pending | pending | n/a | n/a |

### Issued 2026-09-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 06 Sep | d+1 | 44.5 | 31.8 to 62.4 | 123 | 47.5 | 131 | -6% | yes |
| Mon 07 Sep | d+2 | 43.9 | 29.6 to 65.2 | 122 | 44.6 | 123 | -1% | yes |
| Tue 08 Sep | d+3 | 43.6 | 29.3 to 64.9 | 121 | 58.1 | 153 | -25% | yes |
| Wed 09 Sep | d+4 | 43.4 | 29.2 to 64.6 | 120 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+5 | 43.3 | 29.1 to 64.5 | 120 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+6 | 43.2 | 29.1 to 64.2 | 120 | pending | pending | n/a | n/a |
| Sat 12 Sep | d+7 | 43.2 | 29.0 to 64.3 | 120 | pending | pending | n/a | n/a |

### Issued 2026-09-05

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 05 Sep | d+1 | 46.5 | 33.1 to 65.2 | 128 | 45.6 | 126 | +2% | yes |
| Sun 06 Sep | d+2 | 44.9 | 30.2 to 66.8 | 124 | 47.5 | 131 | -5% | yes |
| Mon 07 Sep | d+3 | 44.1 | 29.6 to 65.7 | 122 | 44.6 | 123 | -1% | yes |
| Tue 08 Sep | d+4 | 43.6 | 29.3 to 65.0 | 121 | 58.1 | 153 | -25% | yes |
| Wed 09 Sep | d+5 | 43.4 | 29.1 to 64.7 | 120 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+6 | 43.2 | 29.1 to 64.2 | 120 | pending | pending | n/a | n/a |
| Fri 11 Sep | d+7 | 43.1 | 29.0 to 64.2 | 120 | pending | pending | n/a | n/a |

### Issued 2026-09-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 04 Sep | d+1 | 43.4 | 31.0 to 61.0 | 120 | 49.3 | 135 | -12% | yes |
| Sat 05 Sep | d+2 | 43.0 | 28.9 to 64.0 | 119 | 45.6 | 126 | -6% | yes |
| Sun 06 Sep | d+3 | 42.8 | 28.7 to 63.8 | 119 | 47.5 | 131 | -10% | yes |
| Mon 07 Sep | d+4 | 42.7 | 28.6 to 63.7 | 119 | 44.6 | 123 | -4% | yes |
| Tue 08 Sep | d+5 | 42.6 | 28.5 to 63.6 | 118 | 58.1 | 153 | -27% | yes |
| Wed 09 Sep | d+6 | 42.6 | 28.6 to 63.3 | 118 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+7 | 42.5 | 28.5 to 63.4 | 118 | pending | pending | n/a | n/a |

### Issued 2026-09-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 03 Sep | d+1 | 39.4 | 28.1 to 55.3 | 111 | 44.2 | 122 | -11% | yes |
| Fri 04 Sep | d+2 | 40.7 | 27.3 to 60.5 | 114 | 49.3 | 135 | -17% | yes |
| Sat 05 Sep | d+3 | 41.4 | 27.7 to 61.8 | 116 | 45.6 | 126 | -9% | yes |
| Sun 06 Sep | d+4 | 41.8 | 28.0 to 62.4 | 117 | 47.5 | 131 | -12% | yes |
| Mon 07 Sep | d+5 | 42.0 | 28.1 to 62.8 | 117 | 44.6 | 123 | -6% | yes |
| Tue 08 Sep | d+6 | 42.2 | 28.3 to 62.8 | 117 | 58.1 | 153 | -27% | yes |
| Wed 09 Sep | d+7 | 42.2 | 28.3 to 63.0 | 117 | pending | pending | n/a | n/a |

### Issued 2026-09-02

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 02 Sep | d+1 | 41.2 | 29.3 to 58.0 | 115 | 37.2 | 105 | +11% | yes |
| Thu 03 Sep | d+2 | 41.4 | 27.8 to 61.7 | 116 | 44.2 | 122 | -6% | yes |
| Fri 04 Sep | d+3 | 41.5 | 27.7 to 62.0 | 116 | 49.3 | 135 | -16% | yes |
| Sat 05 Sep | d+4 | 41.5 | 27.8 to 62.1 | 116 | 45.6 | 126 | -9% | yes |
| Sun 06 Sep | d+5 | 41.5 | 27.8 to 62.2 | 116 | 47.5 | 131 | -13% | yes |
| Mon 07 Sep | d+6 | 41.6 | 27.9 to 61.9 | 116 | 44.6 | 123 | -7% | yes |
| Tue 08 Sep | d+7 | 41.6 | 27.8 to 62.1 | 116 | 58.1 | 153 | -28% | yes |

### Issued 2026-09-01

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 01 Sep | d+1 | 42.4 | 30.1 to 59.7 | 118 | 41.0 | 114 | +3% | yes |
| Wed 02 Sep | d+2 | 42.0 | 28.2 to 62.7 | 117 | 37.2 | 105 | +13% | yes |
| Thu 03 Sep | d+3 | 41.8 | 27.9 to 62.5 | 117 | 44.2 | 122 | -5% | yes |
| Fri 04 Sep | d+4 | 41.7 | 27.8 to 62.4 | 116 | 49.3 | 135 | -15% | yes |
| Sat 05 Sep | d+5 | 41.6 | 27.8 to 62.3 | 116 | 45.6 | 126 | -9% | yes |
| Sun 06 Sep | d+6 | 41.6 | 27.9 to 62.0 | 116 | 47.5 | 131 | -12% | yes |
| Mon 07 Sep | d+7 | 41.5 | 27.8 to 62.1 | 116 | 44.6 | 123 | -7% | yes |

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

_7 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

