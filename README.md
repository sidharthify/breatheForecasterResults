# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-03 04:08 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-02, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Sat 03 Oct | d+1 | 62.4 | 45.1 to 86.3 | 71.9 | 156 | Unhealthy | clear, 23 to 33C |
| Sun 04 Oct | d+2 | 62.4 | 42.6 to 91.3 | 71.6 | 156 | Unhealthy | clear, 23 to 32C |
| Mon 05 Oct | d+3 | 62.4 | 42.4 to 91.8 | 71.4 | 156 | Unhealthy | clear, 23 to 33C |
| Tue 06 Oct | d+4 | 62.4 | 42.3 to 92.0 | 71.3 | 156 | Unhealthy | cloudy, 24 to 32C |
| Wed 07 Oct | d+5 | 62.4 | 42.2 to 92.2 | 71.2 | 156 | Unhealthy | thunderstorm, 24 to 30C, 1mm |
| Thu 08 Oct | d+6 | 62.4 | 42.4 to 91.8 | 71.2 | 156 | Unhealthy | thunderstorm, 20 to 30C, 2mm |
| Fri 09 Oct | d+7 | 62.4 | 42.3 to 92.1 | 71.2 | 156 | Unhealthy | drizzle, 18 to 28C, 4mm |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 39 | 10% | 13% | -5% | 95% | 74% | 100% |
| d+2 | 38 | 12% | 14% | -7% | 89% | 66% | 100% |
| d+3 | 37 | 12% | 17% | -8% | 92% | 62% | 100% |
| d+4 | 36 | 15% | 17% | -8% | 89% | 58% | 100% |
| d+5 | 35 | 15% | 17% | -9% | 86% | 51% | 100% |
| d+6 | 35 | 14% | 18% | -11% | 86% | 57% | 100% |
| d+7 | 34 | 15% | 19% | -12% | 82% | 59% | 100% |

Across all lead times the 80% range contained the truth **89%** of the time on **254** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 03 Oct | d+1 | 62.4 | 45.1 to 86.3 | 156 | pending | pending | n/a | n/a |
| Sun 04 Oct | d+2 | 62.4 | 42.6 to 91.3 | 156 | pending | pending | n/a | n/a |
| Mon 05 Oct | d+3 | 62.4 | 42.4 to 91.8 | 156 | pending | pending | n/a | n/a |
| Tue 06 Oct | d+4 | 62.4 | 42.3 to 92.0 | 156 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+5 | 62.4 | 42.2 to 92.2 | 156 | pending | pending | n/a | n/a |
| Thu 08 Oct | d+6 | 62.4 | 42.4 to 91.8 | 156 | pending | pending | n/a | n/a |
| Fri 09 Oct | d+7 | 62.4 | 42.3 to 92.1 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-02

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 02 Oct | d+1 | 57.6 | 41.6 to 79.8 | 152 | 62.4 | 156 | -8% | yes |
| Sat 03 Oct | d+2 | 59.0 | 40.3 to 86.4 | 153 | pending | pending | n/a | n/a |
| Sun 04 Oct | d+3 | 59.7 | 40.6 to 88.0 | 154 | pending | pending | n/a | n/a |
| Mon 05 Oct | d+4 | 60.2 | 40.8 to 88.9 | 154 | pending | pending | n/a | n/a |
| Tue 06 Oct | d+5 | 60.4 | 40.9 to 89.4 | 154 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+6 | 60.6 | 41.1 to 89.3 | 155 | pending | pending | n/a | n/a |
| Thu 08 Oct | d+7 | 60.7 | 41.1 to 89.6 | 155 | pending | pending | n/a | n/a |

### Issued 2026-10-01

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 01 Oct | d+1 | 55.1 | 39.8 to 76.4 | 149 | 55.4 | 150 | -1% | yes |
| Fri 02 Oct | d+2 | 56.5 | 38.5 to 82.8 | 152 | 62.4 | 156 | -9% | yes |
| Sat 03 Oct | d+3 | 57.2 | 38.8 to 84.4 | 152 | pending | pending | n/a | n/a |
| Sun 04 Oct | d+4 | 57.7 | 39.0 to 85.3 | 153 | pending | pending | n/a | n/a |
| Mon 05 Oct | d+5 | 57.9 | 39.1 to 85.8 | 153 | pending | pending | n/a | n/a |
| Tue 06 Oct | d+6 | 58.1 | 39.4 to 85.7 | 153 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+7 | 58.2 | 39.3 to 86.0 | 153 | pending | pending | n/a | n/a |

### Issued 2026-09-30

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 30 Sep | d+1 | 50.9 | 36.7 to 70.6 | 139 | 52.9 | 144 | -4% | yes |
| Thu 01 Oct | d+2 | 53.8 | 36.7 to 79.0 | 146 | 55.4 | 150 | -3% | yes |
| Fri 02 Oct | d+3 | 55.6 | 37.6 to 82.0 | 151 | 62.4 | 156 | -11% | yes |
| Sat 03 Oct | d+4 | 56.6 | 38.2 to 83.7 | 152 | pending | pending | n/a | n/a |
| Sun 04 Oct | d+5 | 57.2 | 38.6 to 84.7 | 152 | pending | pending | n/a | n/a |
| Mon 05 Oct | d+6 | 57.5 | 38.9 to 84.9 | 152 | pending | pending | n/a | n/a |
| Tue 06 Oct | d+7 | 57.7 | 39.0 to 85.4 | 153 | pending | pending | n/a | n/a |

### Issued 2026-09-29

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 29 Sep | d+1 | 55.3 | 39.8 to 76.7 | 150 | 46.2 | 127 | +20% | yes |
| Wed 30 Sep | d+2 | 56.2 | 38.3 to 82.4 | 151 | 52.9 | 144 | +6% | yes |
| Thu 01 Oct | d+3 | 56.7 | 38.4 to 83.7 | 152 | 55.4 | 150 | +2% | yes |
| Fri 02 Oct | d+4 | 57.0 | 38.5 to 84.4 | 152 | 62.4 | 156 | -9% | yes |
| Sat 03 Oct | d+5 | 57.2 | 38.6 to 84.8 | 152 | pending | pending | n/a | n/a |
| Sun 04 Oct | d+6 | 57.3 | 38.8 to 84.6 | 152 | pending | pending | n/a | n/a |
| Mon 05 Oct | d+7 | 57.3 | 38.7 to 84.9 | 152 | pending | pending | n/a | n/a |

### Issued 2026-09-27

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 27 Sep | d+1 | 63.0 | 45.3 to 87.5 | 156 | 71.1 | 162 | -11% | yes |
| Mon 28 Sep | d+2 | 60.2 | 40.9 to 88.4 | 154 | 53.7 | 146 | +12% | yes |
| Tue 29 Sep | d+3 | 58.6 | 39.6 to 86.6 | 153 | 46.2 | 127 | +27% | yes |
| Wed 30 Sep | d+4 | 57.7 | 38.9 to 85.6 | 153 | 52.9 | 144 | +9% | yes |
| Thu 01 Oct | d+5 | 57.2 | 38.6 to 85.0 | 152 | 55.4 | 150 | +3% | yes |
| Fri 02 Oct | d+6 | 57.0 | 38.5 to 84.2 | 152 | 62.4 | 156 | -9% | yes |
| Sat 03 Oct | d+7 | 56.8 | 38.3 to 84.2 | 152 | pending | pending | n/a | n/a |

### Issued 2026-09-26

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 26 Sep | d+1 | 66.8 | 48.1 to 92.9 | 159 | 68.2 | 160 | -2% | yes |
| Sun 27 Sep | d+2 | 62.0 | 42.1 to 91.2 | 156 | 71.1 | 162 | -13% | yes |
| Mon 28 Sep | d+3 | 59.4 | 40.1 to 87.9 | 154 | 53.7 | 146 | +11% | yes |
| Tue 29 Sep | d+4 | 58.0 | 39.1 to 86.0 | 153 | 46.2 | 127 | +26% | yes |
| Wed 30 Sep | d+5 | 57.2 | 38.5 to 84.9 | 152 | 52.9 | 144 | +8% | yes |
| Thu 01 Oct | d+6 | 56.7 | 38.3 to 83.9 | 152 | 55.4 | 150 | +2% | yes |
| Fri 02 Oct | d+7 | 56.4 | 38.1 to 83.7 | 152 | 62.4 | 156 | -10% | yes |

### Issued 2026-09-25

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 25 Sep | d+1 | 61.6 | 44.3 to 85.6 | 155 | 76.2 | 165 | -19% | yes |
| Sat 26 Sep | d+2 | 58.7 | 39.9 to 86.5 | 153 | 68.2 | 160 | -14% | yes |
| Sun 27 Sep | d+3 | 57.2 | 38.6 to 84.6 | 152 | 71.1 | 162 | -20% | yes |
| Mon 28 Sep | d+4 | 56.3 | 38.0 to 83.5 | 152 | 53.7 | 146 | +5% | yes |
| Tue 29 Sep | d+5 | 55.8 | 37.6 to 82.8 | 151 | 46.2 | 127 | +21% | yes |
| Wed 30 Sep | d+6 | 55.5 | 37.6 to 82.1 | 151 | 52.9 | 144 | +5% | yes |
| Thu 01 Oct | d+7 | 55.4 | 37.4 to 82.0 | 150 | 55.4 | 150 | +0% | yes |

### Issued 2026-09-24

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 24 Sep | d+1 | 70.4 | 50.6 to 98.0 | 161 | 66.8 | 159 | +5% | yes |
| Fri 25 Sep | d+2 | 62.8 | 42.6 to 92.6 | 156 | 76.2 | 165 | -18% | yes |
| Sat 26 Sep | d+3 | 58.9 | 39.7 to 87.2 | 153 | 68.2 | 160 | -14% | yes |
| Sun 27 Sep | d+4 | 56.7 | 38.2 to 84.2 | 152 | 71.1 | 162 | -20% | yes |
| Mon 28 Sep | d+5 | 55.5 | 37.4 to 82.5 | 151 | 53.7 | 146 | +3% | yes |
| Tue 29 Sep | d+6 | 54.9 | 37.1 to 81.1 | 149 | 46.2 | 127 | +19% | yes |
| Wed 30 Sep | d+7 | 54.5 | 36.8 to 80.8 | 148 | 52.9 | 144 | +3% | yes |

### Issued 2026-09-23

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 23 Sep | d+1 | 69.2 | 49.7 to 96.4 | 161 | 86.0 | 172 | -20% | yes |
| Thu 24 Sep | d+2 | 61.7 | 41.9 to 90.8 | 155 | 66.8 | 159 | -8% | yes |
| Fri 25 Sep | d+3 | 57.8 | 39.1 to 85.4 | 153 | 76.2 | 165 | -24% | yes |
| Sat 26 Sep | d+4 | 55.7 | 37.6 to 82.4 | 151 | 68.2 | 160 | -18% | yes |
| Sun 27 Sep | d+5 | 54.5 | 36.8 to 80.8 | 148 | 71.1 | 162 | -23% | yes |
| Mon 28 Sep | d+6 | 53.9 | 36.5 to 79.5 | 146 | 53.7 | 146 | +0% | yes |
| Tue 29 Sep | d+7 | 53.5 | 36.2 to 79.2 | 145 | 46.2 | 127 | +16% | yes |

_30 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

