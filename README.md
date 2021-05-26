# Helsingin Sanomat News Archive Search Automation

This script allows to automate queries and download news headline data from Helsingin Sanomat News Archive. Only the headline (title/heading) and the time of publishing are returned.

The script returns a csv file with three columns: 
- article number
- time of publishing
- headline.



# Disclaimer

Helsingin Sanomat (Sanoma Media Finland) owns the copyright to all articles. No infringement of these copyrights is intentional.

Use of this script is subject to the General Terms and Conditions of Sanoma Media Finland, found here (only in Finnish):
https://oma.sanoma.fi/v2/aihe/tilaus-ja-kayttoehdot/kayttoehdot

To comply with the Terms and Conditions, use of this script is prohibited without permission from Sanoma Media Finland. This permission can be obtained by contacting Helsingin Sanomat directly.



# Requirements

1. Install Google Chrome if not already installed (other browsers work too, but the script has to be modified).

2. Install ChromeDriver at https://chromedriver.chromium.org/downloads

Make sure you download the correct ChromeDriver version according to the version of Chrome you have installed (and your operating system)

Save the downloaded file wherever you like, but make sure that you know its location, because the filepath is going to get referenced in the script.

Insert this filepath in line 24 of `hs-news-archive-scrape.py`

For example: `path = "C:/Users/username/webdriver"`

3. Install the required modules and you are good to go


# How It Works

Run `hs-news-archive-scrape.py`

Once prompted, type in a search term and the number of headlines you want in return.

Next type in the time period you want to use ('Any' or 'Custom')
- 'Any': all headlines (roughly from 1990 onwards) will be returned
- 'Custom': you will be asked to select your own start and end dates

Once these are typed in, a tab in Chrome opens, press OK to accept cookies (haven't been able to automate this yet) and let it run.

(The ChromeDriver will run twice because of an issue with the website: once the last page is loaded, all results disappear...)

At the end, a csv file is created, which includes all the headlines resulting from that query.



# How to Contribute

Like most hobby projects, this script is far from perfect. All contributions are welcome.

Issues that I haven't solved yet:
- Automatically handle the cookie popup window when the browser opens.
- Figure out an easier way to compute the maximum 'acceptable load more times'.



