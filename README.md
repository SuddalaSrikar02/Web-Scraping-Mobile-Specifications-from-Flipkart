📱 Web Scraping Flipkart Mobile Data
📌 Project Overview

This project demonstrates how to scrape mobile phone details from Flipkart using Python. It collects structured product information such as:

Brand & Model Name

Price

RAM & ROM (Storage)

Display Size

Battery Capacity

Color Variants

Additional Features

The scraped data is cleaned, organized, and stored into a Pandas DataFrame for further analysis.

🛠️ Tech Stack

Python

BeautifulSoup (bs4) – for parsing HTML

Requests – for sending HTTP requests

Regex (re) – for extracting structured details

Pandas & NumPy – for data cleaning and analysis

Jupyter Notebook – for interactive execution

📂 Workflow

Send request to Flipkart search results page.

Parse HTML using BeautifulSoup.

Extract data: brand, model, price, RAM, ROM, display size, battery, and colors.

Use Regex to capture specifications like RAM size, battery mAh, and screen size.

Store data into a Pandas DataFrame.

Export dataset for analysis and visualization.

📊 Example Output (DataFrame Columns)
Brand | Model | RAM | ROM | Display | Battery | Color | Price

🚀 Future Enhancements

Extend scraping to multiple pages for more products.

Add support for Amazon & other e-commerce sites.

Perform data visualization (price comparison by brand, storage vs. price trends).

Automate scraping with pagination and scheduling.
