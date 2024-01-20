## Geohashing

Calculations related to the daily game of Geohashing.

[Original XKCD comic here](https://xkcd.com/426/)

[Geohashing site here](https://geohashing.site/)

#### Usage

```sh
usage: geohashing.py [-h] [-d DATE] [-j DOW_JONES] [--30w {e,w,east,west}] [-g] [-s] [--centicule] [-b {g,o}] [--near-lat-start NEAR_LAT_START] [--near-lat-stop NEAR_LAT_STOP]
                     [--near-lon-start NEAR_LON_START] [--near-lon-stop NEAR_LON_STOP] [--open-og-comic] [--open-geohashing-home]
                     [latitude] [longitude]

Calculate geohashes as defined by Randall Munroe in xkcd #426.

positional arguments:
  latitude              The latitude of your location (just the integer part is enough for graticule).
  longitude             The longitude of your location (just the integer part is enough for graticule).

options:
  -h, --help            show this help message and exit
  -d DATE, --date DATE  The geohash date in YYYY-MM-DD format. The current date is used otherwise.
  -j DOW_JONES, --dow-jones DOW_JONES, --dj DOW_JONES
                        The Dow Jones value, with two decimal places. The most recent compilant open value is used otherwise
  --30w {e,w,east,west}
                        Override automatic 30W detection, forcing either east or west.
  -g, --global          Calculate the globalhash instead. Lat and lon are ignored.
  -s, --simple          Only return lat and lon, separated by a newline.
  --centicule           Calculate the centicule instead.
  -b {g,o}, --browser {g,o}
                        Open in web browser. 'g' for Google Maps or 'o' for OpenStreetMaps.
  --near-lat-start NEAR_LAT_START
                        Calculate the graticules starting from x graticules away from input latitude.
  --near-lat-stop NEAR_LAT_STOP
                        Calculate the graticules ending at x graticules away from input latitude.
  --near-lon-start NEAR_LON_START
                        Calculate the graticules starting from x graticules away from input longitude.
  --near-lon-stop NEAR_LON_STOP
                        Calculate the graticules ending at x graticules away from input longitude.
  --open-og-comic       Open XKCD #426 in web browser.
  --open-geohashing-home
                        Open the homepage of Geohashing in web browser.
```
