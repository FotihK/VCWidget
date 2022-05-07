# VCWidget
**Widget for VLR score scraping**

*designed for Tarik "tarik" Celik*

Using BS4, PIL, TKinter, and the requests libraries in Python, this widget will scrape current match data from the desired bracket at VLR.gg and display it in a compact format.

# Configuration
The widget can take a few parameters using a separate `config.txt` file.

`config.txt` should be formatted as follows:
```
URL
Refresh Interval (min)
Names of teams whose matches should be grabbed (separated by newlines)
```
for example, this config file,
```
https://www.vlr.gg/event/800/champions-tour-north-america-stage-2-challengers/open-qualifier-2
10
100 Thieves
Version1
Sentinels
Evil Geniuses
```
will grab the bracket for the VCT NA Open Qualifier #2 at 10 minute intervals and will watch for ongoing matches from the four teams listed.

Note that the team names need to be **EXACTLY** copied as shown on the bracket being grabbed.
