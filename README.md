# ESP35 4h OHLCV Index Historical Data — Free Sample

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Dataset rows](https://img.shields.io/badge/full_dataset-13_370_rows-blue)](https://ork.ad/) [![Updated](https://img.shields.io/badge/weekly_update-every_Sunday-green)](https://ork.ad/) [![Full data on ork.ad](https://img.shields.io/badge/download-ork.ad-orange)](https://ork.ad/)

### → [**Download the full ESP35 dataset on ork.ad**](https://ork.ad/)

**ESP35 4h OHLCV Stock index historical data** — ultra high-quality 4h OHLCV for **Spain 35**. Global cash and extended index sessions — Asia, Europe and US coverage, not US-hours only. Clean `time, open, high, low, close, volume` CSV for backtesting, algorithmic trading and quantitative research.

## Table of contents

- [Why this dataset?](#why-this-dataset)
- [Download sample CSV](#download-sample)
- [GitHub Pages preview](#github-pages)
- [Sample vs full dataset](#sample-vs-full-dataset)
- [Timeframes on ork.ad](#timeframes-on-orkad)
- [Weekly updates](#weekly-updates)
- [Data preview](#data-preview)
- [Schema](#schema)
- [Code examples](#code-examples)
- [Download full data on ork.ad](#download-full-data)

## Why this dataset?

- **Ultra high-quality 4h OHLCV** for **Spain 35** (Stock index)
- **Global cash and extended index sessions — Asia, Europe and US coverage, not US-hours only**
- **Clean CSV schema** — `time, open, high, low, close, volume` (no gaps in formatting)
- **Free evaluation sample** on GitHub (`4h`) · **13 timeframes** on [ork.ad](https://ork.ad/) · **13,370** `4h` rows in the full archive
- Built for **backtesting**, **algorithmic trading** and **quantitative finance** workflows
- **Weekly refresh** — [ork.ad](https://ork.ad/) every **Sunday**; GitHub `4h` sample updated in sync

> **Sample on GitHub** · `ESP35_4h.csv` (566 rows, `2025-10-03` → `2026-07-03`). **Full archive on [ork.ad](https://ork.ad/)** — **13,370** `4h` rows (~0.67 MB), **13 timeframes** (``1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W``), `2008-09-10` → `2026-07-03`.

## Download sample

**[ESP35_4h.csv](https://github.com/ork-ad/esp35-4h-ohlcv-index-historical-data/blob/main/ESP35_4h.csv)** on GitHub ([raw CSV](https://raw.githubusercontent.com/ork-ad/esp35-4h-ohlcv-index-historical-data/main/ESP35_4h.csv)) · [GitHub Releases](https://github.com/ork-ad/esp35-4h-ohlcv-index-historical-data/releases) when the release workflow is active.

## GitHub Pages

Interactive chart & stats: **[https://ork-ad.github.io/esp35-4h-ohlcv-index-historical-data/](https://ork-ad.github.io/esp35-4h-ohlcv-index-historical-data/)**

## Sample vs full dataset

| | **Sample (this repo)** | **Full dataset ([ork.ad](https://ork.ad/))** |
|---|--:|---|
| Instrument | Spain 35 · Stock index | Spain 35 · Stock index |
| Timeframes | `4h` (sample) | **13** — `1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W` |
| 4h rows | 566 | **13,370** |
| Size | 0.03 MB | ~0.67 MB |
| Period | `2025-10-03` → `2026-07-03` | `2008-09-10` → `2026-07-03` |
| File | `ESP35_4h.csv` | ZIP on [ork.ad](https://ork.ad/) |
| Updates | Weekly (Sunday) — GitHub sample | Weekly (Sunday) — all timeframes |

## Timeframes on ork.ad

This GitHub repository ships a **`4h` evaluation sample** only. On **[ork.ad](https://ork.ad/)**, each full asset archive is delivered as a ZIP with **13 gap-free OHLCV timeframes** (one CSV per timeframe):

**1m** · **3m** · **5m** · **15m** · **30m** · **1H** · **2H** · **4H** · **8H** · **12H** · **16H** · **1D** · **1W**

GitHub = `4h` sample · [ork.ad](https://ork.ad/) = all **13** timeframes above for the same instrument.

## Weekly updates

- **[ork.ad](https://ork.ad/)** — Full datasets on ork.ad are updated every Sunday.
- **GitHub (this repo)** — GitHub samples are refreshed weekly (every Sunday), in sync with ork.ad.

When a new `4h` sample is published on GitHub, the README, chart preview and CSV reflect the latest week of data.

## Data preview

First and latest rows from the GitHub sample **`ESP35_4h.csv`**:

**First rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| 2025-10-03T14:00:00Z | 15618.61 | 15619.12 | 15560.6 | 15565.6 | 2380 |
| 2025-10-06T06:00:00Z | 15565.6 | 15628.53 | 15490.02 | 15600.04 | 8168 |
| 2025-10-06T10:00:00Z | 15600.04 | 15632.55 | 15573.53 | 15580.54 | 4401 |
| 2025-10-06T14:00:00Z | 15580.54 | 15599.04 | 15543.02 | 15545.53 | 2868 |
| 2025-10-07T06:00:00Z | 15545.53 | 15601.91 | 15484.4 | 15582.39 | 5435 |

**Last rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| time | open | high | low | close | volume |
| 2026-07-02T10:00:00Z | 19608.51 | 19810.51 | 19576.51 | 19780.01 | 5296 |
| 2026-07-02T14:00:00Z | 19780.01 | 19791.03 | 19619.99 | 19627.51 | 6198 |
| 2026-07-03T06:00:00Z | 19627.51 | 19805.47 | 19627.51 | 19784.46 | 5189 |
| 2026-07-03T10:00:00Z | 19784.46 | 19883.98 | 19774.45 | 19878.47 | 2873 |

## Schema

```text
time,open,high,low,close,volume
```

## Code examples

### pandas

```python
import pandas as pd

df = pd.read_csv('ESP35_4h.csv', parse_dates=['time'])
df.set_index('time', inplace=True)
print(df.describe())
print(df.resample('1h').agg({'open': 'first', 'high': 'max',
                              'low': 'min', 'close': 'last', 'volume': 'sum'}).head())
```

### backtrader

```python
import backtrader as bt
import pandas as pd

df = pd.read_csv('ESP35_4h.csv', parse_dates=['time'])
df.set_index('time', inplace=True)

class PandasData(bt.feeds.PandasData):
    params = (('datetime', None), ('open', 'open'), ('high', 'high'),
              ('low', 'low'), ('close', 'close'), ('volume', 'volume'))

cerebro = bt.Cerebro()
cerebro.adddata(PandasData(dataname=df))
# cerebro.addstrategy(YourStrategy)
# cerebro.run()
```

### vectorbt

```python
import pandas as pd
import vectorbt as vbt

df = pd.read_csv('ESP35_4h.csv', parse_dates=['time'])
close = df.set_index('time')['close']
fast, slow = vbt.MA.run(close, 10), vbt.MA.run(close, 50)
entries = fast.ma_crossed_above(slow)
exits = fast.ma_crossed_below(slow)
pf = vbt.Portfolio.from_signals(close, entries, exits, init_cash=10_000, freq='4h')
print(pf.stats())
```

## Download full data

The complete **ESP35** archive on **[ork.ad](https://ork.ad/)** includes **13 OHLCV timeframes** (`1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W`) — **13,370** rows at `4h`, plus all other timeframes in the same ZIP.

**[→ Get the full ESP35 dataset on ork.ad](https://ork.ad/)**

---
*GetData · ESP35 4h OHLCV sample on GitHub · Full historical data on [ork.ad](https://ork.ad/) · 2026-07-06 UTC*