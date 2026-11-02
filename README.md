# Kill Zones [LW]

A Pine Script v5 indicator that marks four configurable time windows with developing high/low boxes: Asia, London, New York, and London Close.

## Default windows

| Zone | Window |
| --- | --- |
| Asia | 20:00–22:00 |
| London | 02:00–05:00 |
| New York | 07:00–10:00 |
| London Close | 10:00–12:00 |

The default timezone is `America/New_York`. The timezone setting applies to all four windows, and the on-chart table displays the selected timezone. Pine's `time()` session checks use the timezone argument supplied by the script; the chart's display timezone does not change script calculations. See TradingView's [sessions](https://www.tradingview.com/pine-script-docs/concepts/sessions/) and [time](https://www.tradingview.com/pine-script-docs/concepts/time/) documentation.

## Add to TradingView

1. Open TradingView's Pine Editor.
2. Paste the contents of [`lw-kill-zones.pine`](lw-kill-zones.pine).
3. Save the script and choose **Add to chart**.

Enable or disable each zone from the **Kill Zones** inputs. The boxes follow each selected window's highs and lows as new bars form. This indicator marks time and price context only; it does not generate trade signals.

## License

Licensed under the MIT License. See [`LICENSE`](LICENSE) for the terms, including the warranty disclaimer.
