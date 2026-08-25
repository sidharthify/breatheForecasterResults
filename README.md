# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-08-26 00:51 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-08-25, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Wed 26 Aug | d+1 | 43.0 | 30.4 to 60.8 | 50.8 | 119 | Unhealthy for Sensitive Groups | clear, 26 to 33C |
| Thu 27 Aug | d+2 | 41.0 | 27.3 to 61.5 | 47.7 | 115 | Unhealthy for Sensitive Groups | drizzle, 26 to 33C |
| Fri 28 Aug | d+3 | 39.9 | 26.6 to 60.0 | 46.2 | 112 | Unhealthy for Sensitive Groups | drizzle, 25 to 33C, 1mm |
| Sat 29 Aug | d+4 | 39.3 | 26.2 to 59.2 | 45.4 | 110 | Unhealthy for Sensitive Groups | thunderstorm, 26 to 33C, 2mm |
| Sun 30 Aug | d+5 | 39.0 | 25.9 to 58.7 | 45.0 | 110 | Unhealthy for Sensitive Groups | thunderstorm, 25 to 32C, 4mm |
| Mon 31 Aug | d+6 | 38.8 | 25.9 to 58.1 | 44.7 | 109 | Unhealthy for Sensitive Groups | thunderstorm, 25 to 32C, 6mm |
| Tue 01 Sep | d+7 | 38.7 | 25.8 to 58.1 | 44.6 | 109 | Unhealthy for Sensitive Groups | thunderstorm, 25 to 30C, 13mm |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 2 | 23% | 23% | -23% | 100% | 50% | 100% |
| d+2 | 1 | 19% | 19% | -19% | 100% | 0% | 100% |
| d+3 | 1 | 20% | 20% | -20% | 100% | 0% | 100% |
| d+4 | 1 | 23% | 23% | +23% | 100% | 0% | 100% |
| d+5 | 1 | 1% | 1% | +1% | 100% | 100% | 100% |
| d+6 | 1 | 22% | 22% | -22% | 100% | 100% | 100% |

Across all lead times the 80% range contained the truth **100%** of the time on **7** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-08-26

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 26 Aug | d+1 | 43.0 | 30.4 to 60.8 | 119 | pending | pending | n/a | n/a |
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
| Wed 26 Aug | d+2 | 37.4 | 25.0 to 56.2 | 106 | pending | pending | n/a | n/a |
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
| Wed 26 Aug | d+7 | 36.6 | 24.2 to 55.2 | 104 | pending | pending | n/a | n/a |

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

