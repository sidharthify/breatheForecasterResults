# Jammu air quality forecast log

Seven day PM2.5 and PM10 forecasts for Jammu, published before the days happen and graded afterwards. A workflow regenerates this file every night. Nothing in it is written by hand, and no forecast is ever edited once recorded.

> **This is an experiment.** It is not wired into the Breathe site or the apps, and nobody should plan around it yet. It is here so that the model can be watched in public for a while before anyone decides whether it is worth shipping.

Last run **2026-10-06 05:55 IST**. Zone `jammu_city`. Index is the **US EPA AQI**. Model and method: [breatheForecaster](https://github.com/sidharthify/breatheForecaster).

## Next seven days

Anchored on 2026-10-05, the last day of sensor data that is actually finished.

| Day | Lead | PM2.5 | 80% range | PM10 | AQI | Category | Weather |
|---|---|---:|---|---:|---:|---|---|
| Tue 06 Oct | d+1 | 83.8 | 60.6 to 115.8 | 90.9 | 171 | Unhealthy | thunderstorm, 23 to 32C, 2mm |
| Wed 07 Oct | d+2 | 76.7 | 52.4 to 112.3 | 84.4 | 166 | Unhealthy | thunderstorm, 21 to 29C, 7mm |
| Thu 08 Oct | d+3 | 73.0 | 49.6 to 107.4 | 81.0 | 163 | Unhealthy | thunderstorm, 22 to 29C |
| Fri 09 Oct | d+4 | 70.9 | 48.0 to 104.7 | 79.1 | 162 | Unhealthy | cloudy, 20 to 29C |
| Sat 10 Oct | d+5 | 69.7 | 47.1 to 103.2 | 78.2 | 161 | Unhealthy | thunderstorm, 21 to 28C, 2mm |
| Sun 11 Oct | d+6 | 69.1 | 46.9 to 101.8 | 77.6 | 160 | Unhealthy | cloudy, 21 to 28C |
| Mon 12 Oct | d+7 | 68.7 | 46.5 to 101.5 | 77.3 | 160 | Unhealthy | cloudy, 19 to 28C |

Concentrations are daily means in micrograms per cubic metre. The range is an 80% interval measured from this zone's own past errors, not from theory. Past about day three the forecast is essentially the 14 day seasonal level, which is the model being honest rather than the model giving up.

## Running scorecard

Every forecast this log has published, graded once its day finished. Nothing here is a backtest.

| Lead | Days scored | Typical miss | Mean miss | Bias | Inside 80% range | Category exact | Within one band |
|---|---:|---:|---:|---:|---:|---:|---:|
| d+1 | 42 | 11% | 13% | -6% | 95% | 76% | 100% |
| d+2 | 41 | 13% | 15% | -8% | 88% | 68% | 100% |
| d+3 | 40 | 15% | 17% | -9% | 90% | 65% | 100% |
| d+4 | 39 | 17% | 18% | -9% | 87% | 62% | 100% |
| d+5 | 38 | 16% | 18% | -11% | 84% | 55% | 100% |
| d+6 | 37 | 17% | 19% | -12% | 84% | 59% | 100% |
| d+7 | 36 | 15% | 19% | -13% | 81% | 61% | 100% |

Across all lead times the 80% range contained the truth **87%** of the time on **273** scored days. A range that says 80% should land near 80%: much less and it is overconfident, much more and it is wider than it needs to be. Bias is the direction of the miss, so a positive number means the forecast ran high.

## Forecast log

One block per night. Actual values appear as each day finishes, so the newest block is empty and the oldest is complete.

### Issued 2026-10-06

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 06 Oct | d+1 | 83.8 | 60.6 to 115.8 | 171 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+2 | 76.7 | 52.4 to 112.3 | 166 | pending | pending | n/a | n/a |
| Thu 08 Oct | d+3 | 73.0 | 49.6 to 107.4 | 163 | pending | pending | n/a | n/a |
| Fri 09 Oct | d+4 | 70.9 | 48.0 to 104.7 | 162 | pending | pending | n/a | n/a |
| Sat 10 Oct | d+5 | 69.7 | 47.1 to 103.2 | 161 | pending | pending | n/a | n/a |
| Sun 11 Oct | d+6 | 69.1 | 46.9 to 101.8 | 161 | pending | pending | n/a | n/a |
| Mon 12 Oct | d+7 | 68.7 | 46.5 to 101.5 | 160 | pending | pending | n/a | n/a |

### Issued 2026-10-05

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Mon 05 Oct | d+1 | 75.6 | 54.7 to 104.6 | 165 | 97.7 | 181 | -23% | yes |
| Tue 06 Oct | d+2 | 71.4 | 48.8 to 104.5 | 162 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+3 | 69.1 | 47.0 to 101.7 | 161 | pending | pending | n/a | n/a |
| Thu 08 Oct | d+4 | 67.9 | 46.0 to 100.1 | 160 | pending | pending | n/a | n/a |
| Fri 09 Oct | d+5 | 67.1 | 45.5 to 99.1 | 159 | pending | pending | n/a | n/a |
| Sat 10 Oct | d+6 | 66.7 | 45.3 to 98.2 | 159 | pending | pending | n/a | n/a |
| Sun 11 Oct | d+7 | 66.5 | 45.1 to 98.1 | 159 | pending | pending | n/a | n/a |

### Issued 2026-10-04

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 04 Oct | d+1 | 67.9 | 49.1 to 93.9 | 160 | 83.6 | 171 | -19% | yes |
| Mon 05 Oct | d+2 | 66.2 | 45.2 to 96.8 | 159 | 97.7 | 181 | -32% | **no** |
| Tue 06 Oct | d+3 | 65.2 | 44.3 to 96.0 | 158 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+4 | 64.7 | 43.9 to 95.4 | 157 | pending | pending | n/a | n/a |
| Thu 08 Oct | d+5 | 64.4 | 43.6 to 95.1 | 157 | pending | pending | n/a | n/a |
| Fri 09 Oct | d+6 | 64.2 | 43.7 to 94.5 | 157 | pending | pending | n/a | n/a |
| Sat 10 Oct | d+7 | 64.1 | 43.5 to 94.6 | 157 | pending | pending | n/a | n/a |

### Issued 2026-10-03

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sat 03 Oct | d+1 | 62.4 | 45.1 to 86.3 | 156 | 70.9 | 162 | -12% | yes |
| Sun 04 Oct | d+2 | 62.4 | 42.6 to 91.3 | 156 | 83.6 | 171 | -25% | yes |
| Mon 05 Oct | d+3 | 62.4 | 42.4 to 91.8 | 156 | 97.7 | 181 | -36% | **no** |
| Tue 06 Oct | d+4 | 62.4 | 42.3 to 92.0 | 156 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+5 | 62.4 | 42.2 to 92.2 | 156 | pending | pending | n/a | n/a |
| Thu 08 Oct | d+6 | 62.4 | 42.4 to 91.8 | 156 | pending | pending | n/a | n/a |
| Fri 09 Oct | d+7 | 62.4 | 42.3 to 92.1 | 156 | pending | pending | n/a | n/a |

### Issued 2026-10-02

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Fri 02 Oct | d+1 | 57.6 | 41.6 to 79.8 | 152 | 62.4 | 156 | -8% | yes |
| Sat 03 Oct | d+2 | 59.0 | 40.3 to 86.4 | 153 | 70.9 | 162 | -17% | yes |
| Sun 04 Oct | d+3 | 59.7 | 40.6 to 88.0 | 154 | 83.6 | 171 | -29% | yes |
| Mon 05 Oct | d+4 | 60.2 | 40.8 to 88.9 | 154 | 97.7 | 181 | -38% | **no** |
| Tue 06 Oct | d+5 | 60.4 | 40.9 to 89.4 | 154 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+6 | 60.6 | 41.1 to 89.3 | 155 | pending | pending | n/a | n/a |
| Thu 08 Oct | d+7 | 60.7 | 41.1 to 89.6 | 155 | pending | pending | n/a | n/a |

### Issued 2026-10-01

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Thu 01 Oct | d+1 | 55.1 | 39.8 to 76.4 | 149 | 55.4 | 150 | -1% | yes |
| Fri 02 Oct | d+2 | 56.5 | 38.5 to 82.8 | 152 | 62.4 | 156 | -9% | yes |
| Sat 03 Oct | d+3 | 57.2 | 38.8 to 84.4 | 152 | 70.9 | 162 | -19% | yes |
| Sun 04 Oct | d+4 | 57.7 | 39.0 to 85.3 | 153 | 83.6 | 171 | -31% | yes |
| Mon 05 Oct | d+5 | 57.9 | 39.1 to 85.8 | 153 | 97.7 | 181 | -41% | **no** |
| Tue 06 Oct | d+6 | 58.1 | 39.4 to 85.7 | 153 | pending | pending | n/a | n/a |
| Wed 07 Oct | d+7 | 58.2 | 39.3 to 86.0 | 153 | pending | pending | n/a | n/a |

### Issued 2026-09-30

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Wed 30 Sep | d+1 | 50.9 | 36.7 to 70.6 | 139 | 52.9 | 144 | -4% | yes |
| Thu 01 Oct | d+2 | 53.8 | 36.7 to 79.0 | 146 | 55.4 | 150 | -3% | yes |
| Fri 02 Oct | d+3 | 55.6 | 37.6 to 82.0 | 151 | 62.4 | 156 | -11% | yes |
| Sat 03 Oct | d+4 | 56.6 | 38.2 to 83.7 | 152 | 70.9 | 162 | -20% | yes |
| Sun 04 Oct | d+5 | 57.2 | 38.6 to 84.7 | 152 | 83.6 | 171 | -32% | yes |
| Mon 05 Oct | d+6 | 57.5 | 38.9 to 84.9 | 152 | 97.7 | 181 | -41% | **no** |
| Tue 06 Oct | d+7 | 57.7 | 39.0 to 85.4 | 153 | pending | pending | n/a | n/a |

### Issued 2026-09-29

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Tue 29 Sep | d+1 | 55.3 | 39.8 to 76.7 | 150 | 46.2 | 127 | +20% | yes |
| Wed 30 Sep | d+2 | 56.2 | 38.3 to 82.4 | 151 | 52.9 | 144 | +6% | yes |
| Thu 01 Oct | d+3 | 56.7 | 38.4 to 83.7 | 152 | 55.4 | 150 | +2% | yes |
| Fri 02 Oct | d+4 | 57.0 | 38.5 to 84.4 | 152 | 62.4 | 156 | -9% | yes |
| Sat 03 Oct | d+5 | 57.2 | 38.6 to 84.8 | 152 | 70.9 | 162 | -19% | yes |
| Sun 04 Oct | d+6 | 57.3 | 38.8 to 84.6 | 152 | 83.6 | 171 | -31% | yes |
| Mon 05 Oct | d+7 | 57.3 | 38.7 to 84.9 | 152 | 97.7 | 181 | -41% | **no** |

### Issued 2026-09-27

| Day | Lead | Forecast PM2.5 | 80% range | Forecast AQI | Actual PM2.5 | Actual AQI | Miss | In range |
|---|---|---:|---|---:|---:|---:|---:|---|
| Sun 27 Sep | d+1 | 63.0 | 45.3 to 87.5 | 156 | 71.1 | 162 | -11% | yes |
| Mon 28 Sep | d+2 | 60.2 | 40.9 to 88.4 | 154 | 53.7 | 146 | +12% | yes |
| Tue 29 Sep | d+3 | 58.6 | 39.6 to 86.6 | 153 | 46.2 | 127 | +27% | yes |
| Wed 30 Sep | d+4 | 57.7 | 38.9 to 85.6 | 153 | 52.9 | 144 | +9% | yes |
| Thu 01 Oct | d+5 | 57.2 | 38.6 to 85.0 | 152 | 55.4 | 150 | +3% | yes |
| Fri 02 Oct | d+6 | 57.0 | 38.5 to 84.2 | 152 | 62.4 | 156 | -9% | yes |
| Sat 03 Oct | d+7 | 56.8 | 38.3 to 84.2 | 152 | 70.9 | 162 | -20% | yes |

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

_33 older forecasts are not shown. The full journal is in `journal/` and nothing is ever removed from it._

## What these numbers do and do not show

**A miss is a percentage, not micrograms.** A 20% miss on a clean day and a 20% miss on a filthy one are the same size of mistake to this model, which is why it works in logs.

**Category accuracy flatters itself.** Most days in one place fall in the same EPA band, so a program that printed the most common band every day would already score well. Read the category columns against that, not against zero.

**The record is short and starts in January 2026.** No autumn or winter has been observed here at all. Everything this model does in November is extrapolation until it has been through one, and absolute errors in winter will be larger because winter levels are several times higher.

