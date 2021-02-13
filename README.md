# Helsingin Sanomat News Archive Search Automation and Scraper

This script allows to automate queries and fetch news headline data from Helsingin Sanomat News Archive. Only the headline (title) and the time of publishing are returned.

The script returns a csv file including three columns: 
- article number
- time of publishing (ISO 8610)
- headline.



# Disclaimer

Helsingin Sanomat (Sanoma Media Finland) owns the copyright to all articles. No infringement of these copyrights is intentional.

Use of this script is subject to the General Terms and Conditions of Sanoma Media Finland, found here (only in Finnish):
https://oma.sanoma.fi/v2/aihe/tilaus-ja-kayttoehdot/kayttoehdot

To comply with the Terms and Conditions, use of this script is prohibited without permission from Sanoma Media Finland. This permission can be obtained by contacting Helsingin Sanomat directly.



# How It Works

Install Chrome and the required modules.

Insert a path in row 58 for the WebDriver that will be created
- For example `path = "/Users/username/webdriver"`

Run `hs-news-archive-scrape.py`

Once prompted, type in a search term and the number of headlines you want returned.

Next type in the time period you want to use ('Any' or 'Custom')
- 'Any': all headlines (roughly from 1990 onwards) will be returned
- 'Custom': you will be asked to select your own start and end dates

Once these are typed in, a tab in Chrome opens, press OK to accept cookies (haven't been able to automate this yet) and let it run.

At the end, a csv file is created, which includes all the headlines resulting from that query.



# How to Contribute

Like most hobby projects, this script is far from perfect. All contributions are welcome.

Issues that I haven't solved yet:
- Automatically handle the cookie popup window when the browser opens. This seems a bit tricky.
- Figure out an easier way to compute the maximum 'acceptable load more times'.



