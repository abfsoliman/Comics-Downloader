# XKCD Comic Downloader

This Python script is designed to automatically download XKCD comics from the XKCD website. It follows the trail of comics by navigating through the "Previous Comic" links, starting from the most recent comic and working its way back to the first one. This script saves the comic images locally on your hard drive.

## How to Use

1. Ensure you have Python installed on your system.
2. Install the required libraries using pip:

```
pip install requests beautifulsoup4
```
3. Run the script in your terminal or command prompt:

```
python downloadXkcd.py
```


## Description

XKCD is a popular geek webcomic with a website structure that includes a front page displaying the most recent comic and a "Previous" button that takes you to the prior comic. This script automates the process of downloading each comic sequentially.

### Steps Performed by the Script

1. **Load XKCD home page**: The script starts by loading the XKCD home page.
2. **Save the comic image**: It identifies and saves the comic image on the current page.
3. **Follow the Previous Comic link**: It finds the URL of the "Previous Comic" link and navigates to that page.
4. **Repeat until the first comic**: The script repeats this process until it reaches the first comic, downloading each one along the way.

## Dependencies

- `requests`: Used for making HTTP requests to fetch web pages.
- `beautifulsoup4`: Used for parsing HTML content and extracting data from web pages.

## Disclaimer

This script is intended for educational purposes only. Ensure compliance with XKCD's terms of use and copyright policies before using it to download comics.
