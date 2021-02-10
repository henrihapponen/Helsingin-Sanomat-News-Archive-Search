# Helsingin Sanomat News Archive Search Automation and Scraper

This script allows to automate queries and fetch news headline data from Helsingin Sanomat News Archive. Only the headline (title) and the time of publishing are returned.

The script returns a csv file including three columns: article number, time of publishing (ISO 8610), and headline.



# Disclaimer

Helsingin Sanomat (Sanoma Media Finland) owns the copyright to all articles. No infringement of these copyrights is intentional.

Use of this script is subject to the general terms and conditions of Sanoma Media Finland, found here (only in Finnish):
https://oma.sanoma.fi/v2/aihe/tilaus-ja-kayttoehdot/kayttoehdot

To comply with their terms and conditions, use of this script is prohibited without permission from Sanoma Media Finland. This permission can be obtained by contacting Helsingin Sanomat directly.



# How It Works

Install Chrome and the required packages.

Run `hs-news-archive-scrape.py`

Once prompted, type in a search term and the number of headlines you want returned, and press enter. 

A tab in Chrome is opened, press OK to accept cookies (haven't been able to automate this yet) and let it run.

A csv file is created, which includes all the headlines resulting from that query.



# How to Contribute

Like most hobby projects, this script is not perfect. All contributions are welcome.

Issues that I haven't solved yet:
- Automatically handle the cookie popup window when the browser opens. This seems to be quite tricky.
- Figure out an easier way to compute the maximum 'acceptable load more times'.



