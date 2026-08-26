# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-08-27 02:53 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-08-26, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Thu 27 Aug | d+1 | 47.8 | 33.8 to 67.6 | 55.6 | 131 | Unhealthy for Sensitive Groups | drizzle, 24 to 33C, 1mm |
| Fri 28 Aug | d+2 | 43.8 | 29.2 to 65.7 | 50.5 | 121 | Unhealthy for Sensitive Groups | thunderstorm, 25 to 33C, 3mm |
| Sat 29 Aug | d+3 | 41.7 | 27.7 to 62.7 | 47.9 | 116 | Unhealthy for Sensitive Groups | thunderstorm, 27 to 33C, 1mm |
| Sun 30 Aug | d+4 | 40.6 | 27.0 to 61.0 | 46.6 | 113 | Unhealthy for Sensitive Groups | thunderstorm, 25 to 32C, 7mm |
| Mon 31 Aug | d+5 | 39.9 | 26.5 to 60.1 | 45.9 | 112 | Unhealthy for Sensitive Groups | thunderstorm, 25 to 31C, 11mm |
| Tue 01 Sep | d+6 | 39.6 | 26.4 to 59.3 | 45.5 | 111 | Unhealthy for Sensitive Groups | thunderstorm, 24 to 30C, 14mm |
| Wed 02 Sep | d+7 | 39.4 | 26.2 to 59.2 | 45.3 | 111 | Unhealthy for Sensitive Groups | drizzle, 24 to 31C, 2mm |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 3 | 23% | 23% | -23% | 100% | 33% | 100% |
| d+2 | 2 | 26% | 26% | -26% | 100% | 0% | 100% |
| d+3 | 1 | 20% | 20% | -20% | 100% | 0% | 100% |
| d+4 | 1 | 23% | 23% | +23% | 100% | 0% | 100% |
| d+5 | 1 | 1% | 1% | +1% | 100% | 100% | 100% |
| d+6 | 1 | 22% | 22% | -22% | 100% | 100% | 100% |
| d+7 | 1 | 34% | 34% | -34% | 0% | 0% | 100% |

Across all lead times the 80% range contained the truth **90%** of the time on **10** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-08-27

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 27 Aug | d+1 | 47.8 | 33.8 to 67.6 | 131 | pending | pending | n/a | n/a |
| Fri 28 Aug | d+2 | 43.8 | 29.2 to 65.7 | 121 | pending | pending | n/a | n/a |
| Sat 29 Aug | d+3 | 41.7 | 27.7 to 62.7 | 116 | pending | pending | n/a | n/a |
| Sun 30 Aug | d+4 | 40.6 | 27.0 to 61.0 | 114 | pending | pending | n/a | n/a |
| Mon 31 Aug | d+5 | 39.9 | 26.5 to 60.1 | 112 | pending | pending | n/a | n/a |
| Tue 01 Sep | d+6 | 39.6 | 26.4 to 59.3 | 111 | pending | pending | n/a | n/a |
| Wed 02 Sep | d+7 | 39.4 | 26.2 to 59.2 | 111 | pending | pending | n/a | n/a |

### Issued 2026-08-26

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 26 Aug | d+1 | 43.0 | 30.4 to 60.8 | 119 | 55.7 | 151 | -23% | yes |
| Thu 27 Aug | d+2 | 41.0 | 27.3 to 61.5 | 115 | pending | pending | n/a | n/a |
| Fri 28 Aug | d+3 | 39.9 | 26.6 to 60.0 | 112 | pending | pending | n/a | n/a |
| Sat 29 Aug | d+4 | 39.3 | 26.2 to 59.2 | 110 | pending | pending | n/a | n/a |
| Sun 30 Aug | d+5 | 39.0 | 25.9 to 58.7 | 110 | pending | pending | n/a | n/a |
| Mon 31 Aug | d+6 | 38.8 | 25.9 to 58.1 | 109 | pending | pending | n/a | n/a |
| Tue 01 Sep | d+7 | 38.7 | 25.8 to 58.1 | 109 | pending | pending | n/a | n/a |

### Issued 2026-08-25

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 25 Aug | d+1 | 36.9 | 26.1 to 52.2 | 104 | 46.8 | 129 | -21% | yes |
| Wed 26 Aug | d+2 | 37.4 | 25.0 to 56.2 | 106 | 55.7 | 151 | -33% | yes |
| Thu 27 Aug | d+3 | 37.8 | 25.1 to 56.8 | 107 | pending | pending | n/a | n/a |
| Fri 28 Aug | d+4 | 38.0 | 25.2 to 57.2 | 107 | pending | pending | n/a | n/a |
| Sat 29 Aug | d+5 | 38.1 | 25.3 to 57.3 | 107 | pending | pending | n/a | n/a |
| Sun 30 Aug | d+6 | 38.1 | 25.5 to 57.1 | 107 | pending | pending | n/a | n/a |
| Mon 31 Aug | d+7 | 38.2 | 25.4 to 57.3 | 108 | pending | pending | n/a | n/a |

### Issued 2026-08-19

_Recorded before this log moved to the EPA index. The concentrations are exactly as they were published; the index column is recomputed from them on the EPA scale so that it can be compared with the rest._

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 20 Aug | d+1 | 31.6 | 22.3 to 44.9 | 93 | 41.9 | 117 | -25% | yes |
| Fri 21 Aug | d+2 | 33.8 | 22.4 to 50.9 | 97 | 41.8 | 116 | -19% | yes |
| Sat 22 Aug | d+3 | 35.0 | 23.2 to 53.0 | 99 | 43.5 | 120 | -20% | yes |
| Sun 23 Aug | d+4 | 35.8 | 23.6 to 54.2 | 102 | 29.1 | 88 | +23% | yes |
| Mon 24 Aug | d+5 | 36.2 | 23.9 to 54.8 | 103 | 35.8 | 102 | +1% | yes |
| Tue 25 Aug | d+6 | 36.5 | 24.2 to 54.9 | 103 | 46.8 | 129 | -22% | yes |
| Wed 26 Aug | d+7 | 36.6 | 24.2 to 55.2 | 104 | 55.7 | 151 | -34% | **no** |

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

