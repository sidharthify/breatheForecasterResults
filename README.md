# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-09-04 02:57 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-09-03, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Fri 04 Sep | d+1 | 43.4 | 31.0 to 61.0 | 51.6 | 120 | Unhealthy for Sensitive Groups | thunderstorm, 23 to 31C, 10mm |
| Sat 05 Sep | d+2 | 43.0 | 28.9 to 64.0 | 50.9 | 119 | Unhealthy for Sensitive Groups | thunderstorm, 22 to 30C, 12mm |
| Sun 06 Sep | d+3 | 42.8 | 28.7 to 63.8 | 50.5 | 119 | Unhealthy for Sensitive Groups | drizzle, 23 to 30C, 1mm |
| Mon 07 Sep | d+4 | 42.7 | 28.6 to 63.7 | 50.3 | 118 | Unhealthy for Sensitive Groups | cloudy, 24 to 32C |
| Tue 08 Sep | d+5 | 42.6 | 28.5 to 63.6 | 50.2 | 118 | Unhealthy for Sensitive Groups | clear, 24 to 32C |
| Wed 09 Sep | d+6 | 42.6 | 28.6 to 63.3 | 50.2 | 118 | Unhealthy for Sensitive Groups | drizzle, 24 to 32C |
| Thu 10 Sep | d+7 | 42.5 | 28.5 to 63.4 | 50.1 | 118 | Unhealthy for Sensitive Groups | drizzle, 24 to 31C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 11 | 5% | 10% | -7% | 100% | 82% | 100% |
| d+2 | 10 | 7% | 11% | -8% | 100% | 80% | 100% |
| d+3 | 9 | 8% | 10% | -8% | 100% | 89% | 100% |
| d+4 | 8 | 9% | 11% | -3% | 100% | 88% | 100% |
| d+5 | 7 | 8% | 8% | -5% | 100% | 100% | 100% |
| d+6 | 6 | 10% | 11% | -9% | 100% | 100% | 100% |
| d+7 | 5 | 11% | 14% | -11% | 80% | 80% | 100% |

Across all lead times the 80% range contained the truth **98%** of the time on **56** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-09-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 04 Sep | d+1 | 43.4 | 31.0 to 61.0 | 120 | pending | pending | n/a | n/a |
| Sat 05 Sep | d+2 | 43.0 | 28.9 to 64.0 | 119 | pending | pending | n/a | n/a |
| Sun 06 Sep | d+3 | 42.8 | 28.7 to 63.8 | 119 | pending | pending | n/a | n/a |
| Mon 07 Sep | d+4 | 42.7 | 28.6 to 63.7 | 119 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+5 | 42.6 | 28.5 to 63.6 | 118 | pending | pending | n/a | n/a |
| Wed 09 Sep | d+6 | 42.6 | 28.6 to 63.3 | 118 | pending | pending | n/a | n/a |
| Thu 10 Sep | d+7 | 42.5 | 28.5 to 63.4 | 118 | pending | pending | n/a | n/a |

### Issued 2026-09-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 03 Sep | d+1 | 39.4 | 28.1 to 55.3 | 111 | 44.2 | 122 | -11% | yes |
| Fri 04 Sep | d+2 | 40.7 | 27.3 to 60.5 | 114 | pending | pending | n/a | n/a |
| Sat 05 Sep | d+3 | 41.4 | 27.7 to 61.8 | 116 | pending | pending | n/a | n/a |
| Sun 06 Sep | d+4 | 41.8 | 28.0 to 62.4 | 117 | pending | pending | n/a | n/a |
| Mon 07 Sep | d+5 | 42.0 | 28.1 to 62.8 | 117 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+6 | 42.2 | 28.3 to 62.8 | 117 | pending | pending | n/a | n/a |
| Wed 09 Sep | d+7 | 42.2 | 28.3 to 63.0 | 117 | pending | pending | n/a | n/a |

### Issued 2026-09-02

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 02 Sep | d+1 | 41.2 | 29.3 to 58.0 | 115 | 37.3 | 105 | +11% | yes |
| Thu 03 Sep | d+2 | 41.4 | 27.8 to 61.7 | 116 | 44.2 | 122 | -6% | yes |
| Fri 04 Sep | d+3 | 41.5 | 27.7 to 62.0 | 116 | pending | pending | n/a | n/a |
| Sat 05 Sep | d+4 | 41.5 | 27.8 to 62.1 | 116 | pending | pending | n/a | n/a |
| Sun 06 Sep | d+5 | 41.5 | 27.8 to 62.2 | 116 | pending | pending | n/a | n/a |
| Mon 07 Sep | d+6 | 41.6 | 27.9 to 61.9 | 116 | pending | pending | n/a | n/a |
| Tue 08 Sep | d+7 | 41.6 | 27.8 to 62.1 | 116 | pending | pending | n/a | n/a |

### Issued 2026-09-01

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 01 Sep | d+1 | 42.4 | 30.1 to 59.7 | 118 | 41.0 | 114 | +3% | yes |
| Wed 02 Sep | d+2 | 42.0 | 28.2 to 62.7 | 117 | 37.3 | 105 | +13% | yes |
| Thu 03 Sep | d+3 | 41.8 | 27.9 to 62.5 | 117 | 44.2 | 122 | -5% | yes |
| Fri 04 Sep | d+4 | 41.7 | 27.8 to 62.4 | 116 | pending | pending | n/a | n/a |
| Sat 05 Sep | d+5 | 41.6 | 27.8 to 62.3 | 116 | pending | pending | n/a | n/a |
| Sun 06 Sep | d+6 | 41.6 | 27.9 to 62.0 | 116 | pending | pending | n/a | n/a |
| Mon 07 Sep | d+7 | 41.5 | 27.8 to 62.1 | 116 | pending | pending | n/a | n/a |

### Issued 2026-08-31

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 31 Aug | d+1 | 42.8 | 30.4 to 60.3 | 119 | 43.1 | 120 | -1% | yes |
| Tue 01 Sep | d+2 | 41.8 | 28.0 to 62.5 | 117 | 41.0 | 114 | +2% | yes |
| Wed 02 Sep | d+3 | 41.3 | 27.6 to 61.8 | 115 | 37.3 | 105 | +11% | yes |
| Thu 03 Sep | d+4 | 41.0 | 27.3 to 61.4 | 115 | 44.2 | 122 | -7% | yes |
| Fri 04 Sep | d+5 | 40.8 | 27.2 to 61.2 | 114 | pending | pending | n/a | n/a |
| Sat 05 Sep | d+6 | 40.7 | 27.3 to 60.8 | 114 | pending | pending | n/a | n/a |
| Sun 06 Sep | d+7 | 40.7 | 27.2 to 60.9 | 114 | pending | pending | n/a | n/a |

### Issued 2026-08-30

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 30 Aug | d+1 | 42.9 | 30.5 to 60.5 | 119 | 44.6 | 123 | -4% | yes |
| Mon 31 Aug | d+2 | 41.7 | 27.9 to 62.4 | 116 | 43.1 | 120 | -3% | yes |
| Tue 01 Sep | d+3 | 41.1 | 27.4 to 61.6 | 115 | 41.0 | 114 | +0% | yes |
| Wed 02 Sep | d+4 | 40.7 | 27.1 to 61.1 | 114 | 37.3 | 105 | +9% | yes |
| Thu 03 Sep | d+5 | 40.5 | 27.0 to 60.8 | 113 | 44.2 | 122 | -8% | yes |
| Fri 04 Sep | d+6 | 40.4 | 27.0 to 60.4 | 113 | pending | pending | n/a | n/a |
| Sat 05 Sep | d+7 | 40.3 | 26.9 to 60.4 | 113 | pending | pending | n/a | n/a |

### Issued 2026-08-29

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 29 Aug | d+1 | 42.7 | 30.3 to 60.3 | 119 | 45.1 | 125 | -5% | yes |
| Sun 30 Aug | d+2 | 41.5 | 27.7 to 62.1 | 116 | 44.6 | 123 | -7% | yes |
| Mon 31 Aug | d+3 | 40.8 | 27.2 to 61.3 | 114 | 43.1 | 120 | -5% | yes |
| Tue 01 Sep | d+4 | 40.4 | 26.9 to 60.8 | 113 | 41.0 | 114 | -1% | yes |
| Wed 02 Sep | d+5 | 40.2 | 26.8 to 60.5 | 113 | 37.3 | 105 | +8% | yes |
| Thu 03 Sep | d+6 | 40.1 | 26.8 to 60.0 | 112 | 44.2 | 122 | -9% | yes |
| Fri 04 Sep | d+7 | 40.0 | 26.7 to 60.1 | 112 | pending | pending | n/a | n/a |

### Issued 2026-08-28

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 28 Aug | d+1 | 44.3 | 31.4 to 62.7 | 123 | 45.0 | 124 | -2% | yes |
| Sat 29 Aug | d+2 | 42.0 | 28.0 to 63.0 | 117 | 45.1 | 125 | -7% | yes |
| Sun 30 Aug | d+3 | 40.8 | 27.1 to 61.3 | 114 | 44.6 | 123 | -8% | yes |
| Mon 31 Aug | d+4 | 40.1 | 26.7 to 60.3 | 112 | 43.1 | 120 | -7% | yes |
| Tue 01 Sep | d+5 | 39.7 | 26.4 to 59.8 | 111 | 41.0 | 114 | -3% | yes |
| Wed 02 Sep | d+6 | 39.5 | 26.4 to 59.2 | 111 | 37.3 | 105 | +6% | yes |
| Thu 03 Sep | d+7 | 39.4 | 26.2 to 59.1 | 111 | 44.2 | 122 | -11% | yes |

### Issued 2026-08-27

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 27 Aug | d+1 | 47.8 | 33.8 to 67.6 | 131 | 48.7 | 134 | -2% | yes |
| Fri 28 Aug | d+2 | 43.8 | 29.2 to 65.7 | 121 | 45.0 | 124 | -3% | yes |
| Sat 29 Aug | d+3 | 41.7 | 27.7 to 62.7 | 116 | 45.1 | 125 | -8% | yes |
| Sun 30 Aug | d+4 | 40.6 | 27.0 to 61.0 | 114 | 44.6 | 123 | -9% | yes |
| Mon 31 Aug | d+5 | 39.9 | 26.5 to 60.1 | 112 | 43.1 | 120 | -7% | yes |
| Tue 01 Sep | d+6 | 39.6 | 26.4 to 59.3 | 111 | 41.0 | 114 | -3% | yes |
| Wed 02 Sep | d+7 | 39.4 | 26.2 to 59.2 | 111 | 37.3 | 105 | +6% | yes |

### Issued 2026-08-26

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 26 Aug | d+1 | 43.0 | 30.4 to 60.8 | 119 | 55.7 | 151 | -23% | yes |
| Thu 27 Aug | d+2 | 41.0 | 27.3 to 61.5 | 115 | 48.7 | 134 | -16% | yes |
| Fri 28 Aug | d+3 | 39.9 | 26.6 to 60.0 | 112 | 45.0 | 124 | -11% | yes |
| Sat 29 Aug | d+4 | 39.3 | 26.2 to 59.2 | 110 | 45.1 | 125 | -13% | yes |
| Sun 30 Aug | d+5 | 39.0 | 25.9 to 58.7 | 110 | 44.6 | 123 | -12% | yes |
| Mon 31 Aug | d+6 | 38.8 | 25.9 to 58.1 | 109 | 43.1 | 120 | -10% | yes |
| Tue 01 Sep | d+7 | 38.7 | 25.8 to 58.1 | 109 | 41.0 | 114 | -6% | yes |

_2 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

