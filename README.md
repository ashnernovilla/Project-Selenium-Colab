# Project-Selenium-Colab

## Overview
This script automates the process of extracting gaming laptop details from Flipkart using Selenium. The extracted data includes laptop specifications, prices, ratings, and more. The script iterates through multiple pages of search results and compiles the data into lists for further analysis.

## Requirements
To run this script, you need to have the following installed:
- Python 3.x
- Selenium
- Google Chrome
- Chrome WebDriver (matching your Chrome version)
- Pandas
- Matplotlib
- Seaborn
- Plotly

## Installation
1. Install required Python packages using pip:
   ```bash
   pip install -r requirements.txt
   ```
2. Download the appropriate Chrome WebDriver from [ChromeDriver](https://sites.google.com/chromium.org/driver/).
3. Place the ChromeDriver in a directory accessible by your system's PATH.

## How the Script Works
1. Initializes Selenium with a Chrome WebDriver.

2. Defines placeholder lists for storing laptop details.

3. Iterates over multiple pages of Flipkart's gaming laptop search results.

4. Extracts details such as:

   - Name

   - Price (Discounted Price Only)

   - Rating

   - Processor Type

   - Memory (RAM)

   - Operating System

   - Storage

   - Display Size

   - Additional Inclusions

5. Appends extracted data to lists only when all expected specifications are available.

6. Sleeps for 5 seconds between page requests to prevent being blocked.

7. Closes the browser instance once data extraction is complete.


## Data Extraction Breakdown
- The script searches Flipkart with the query "gaming laptop."

- It extracts data using class names associated with different elements.

- It splits specification details into individual categories for better structuring.

- Handles missing data by using try-except blocks.


## Usage
To run the script, execute the following command:

```bash

python script_name.py

```
Make sure to replace `script_name.py` with the actual filename of your script.


## Notes
- The script scrapes only **two pages** of Flipkart results but can be modified for more.

- It extracts only laptops with complete specification details.

- If Flipkart updates its website structure, the script may require modifications.

- To avoid being blocked, consider adding a user-agent header or increasing sleep time.


## Future Enhancements
- Convert extracted data into a structured CSV file or a Pandas DataFrame.

- Implement error logging for debugging.

- Use a headless browser mode for faster execution.

- Add proxies to prevent detection.

- Implement dynamic scrolling to capture more data.


## Disclaimer
This script is intended for educational purposes only. Scraping websites without permission may violate their terms of service. Use responsibly.

