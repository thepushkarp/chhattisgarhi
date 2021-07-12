<h1 align="center"> Scrape Chhattigarhi</h1>

<p align="center">Script to collect scrape and clean sentences in Chhattisgarhi for the project <a href="https://www.respin.iisc.ac.in/">Speech Recognition in Agriculture and Finance for the Poor in India</a></p>

<hr/>

## What is this

This script uses [Google Sheets API](https://developers.google.com/sheets/api/quickstart/python) to fetch data from a Google Sheet containing links of sites containing Chhattisgarhi text in the domains of Agriculture and Finance and then does the following:

-   Identifies duplicate links
-   Generates all the links from the sitemaps of popular Chhattisgarhi news portals and gets a list of all links that are not in the sheet (Note: Not all links are useful for us)
-   Scrapes and extracts useful text from the links
-   Optionally, can query all the links to get links containing a particular substring in them
-   Cleans the extracted text and tokenizes them into words to form a vocabulary of Chhattisgarhi words
-   Stores the clean sentences to form our Chhattisgarhi corpus

## How to use?

Create a `.env` file and add a `SPREADSHEET_ID` field with the [unique ID](https://developers.google.com/sheets/api/guides/concepts) of your Google Sheet. Then run `scrape.ipynb`.

## Authors

-   [Pushkar Patel](https://github.com/thepushkarp)
-   [Mayank Bazari](https://github.com/Mayankbazari)
