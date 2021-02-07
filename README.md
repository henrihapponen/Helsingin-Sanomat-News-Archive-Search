# Helsingin Sanomat News Archive Search


### Disclaimer

Helsingin Sanomat (Sanoma Media Finland) owns the copyright to all articles. No infringement of these copyrights is intentional.

Use of this script is subject to the general terms and conditions of Sanoma Media Finland, found here (in Finnish):
https://oma.sanoma.fi/v2/aihe/tilaus-ja-kayttoehdot/kayttoehdot

In line with the terms and conditions above, use of this script is prohibited without first obtaining formal consent from Sanoma Media Finland. This permission can be obtained by emailing dev@hs.fi.



### Description

This script allows to automate queries and fetch news headline data from Helsingin Sanomat news archive. Only the title and time of publishing are returned.

The script returns a csv file including three columns: "Article number", "Time of publishing", and "Headline".



### How It Works

Install Chrome and the required packages.

Run the script.

Once prompted, type in a search term and the number of headlines you want returned, and press enter. 

The driver opens a tab in Chrome, press OK to accept cookies (haven't been able to automate this yet) and let the script run.

A csv file is created, which includes all the headlines resulting from that query.


### Contribute

Like most hobby projects, this script is not perfect. All contributions are welcome.

Issues that I haven't solved yet:
- Automatically accept cookies when the browser opens.
- Compute the maximum 'acceptable load more times' quicker.



