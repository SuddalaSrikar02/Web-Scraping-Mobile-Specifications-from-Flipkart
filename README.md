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


 🛍️ Flipkart Fashion Web Scraping

This project focuses on **web scraping fashion product data from Flipkart** using Python.  
It extracts product details such as **name, price, rating, and reviews**, which can be used for analysis, comparison, or trend prediction in the e-commerce fashion sector.

---

## 📘 Project Overview
Flipkart is one of India's largest online marketplaces.  
This project demonstrates how to use **Python web scraping techniques** to collect structured product data from Flipkart’s fashion section.

You’ll learn:
- How to send HTTP requests to a webpage  
- How to parse HTML content using BeautifulSoup  
- How to extract useful product details  
- How to store data using Pandas  

---

## 🧰 Tools and Libraries Used
| Library | Purpose |
|----------|----------|
| `requests` | To send HTTP requests and get webpage data |
| `beautifulsoup4` | To parse and extract data from HTML |
| `pandas` | To store, clean, and analyze scraped data |
| `jupyter` | To run the code interactively |

Install all dependencies:
pip install requests beautifulsoup4 pandas


⚙️ How to Run This Project

Clone this repository

Open the Jupyter Notebook
jupyter notebook "nani (1).ipynb"


Run all cells

The script will fetch product details (like name, price, rating, and review count) from Flipkart’s fashion section.

The results will be displayed in a Pandas DataFrame.


🧩 Example of HTML Structure Used

The scraper targets key HTML tags on Flipkart product pages such as:

<div class="_2WkVRV">Product Name</div>
<div class="_30jeq3 _1_WHN1">₹499</div>
<div class="_3LWZlK">4.2</div>
<span class="_2_R_DZ">(250)</span>


These tags are extracted using BeautifulSoup like this:

product_name = soup.find_all('div', class_='_2WkVRV')
price = soup.find_all('div', class_='_30jeq3 _1_WHN1')
rating = soup.find_all('div', class_='_3LWZlK')
reviews = soup.find_all('span', class_='_2_R_DZ')

🧾 Example Output
Product Name	Price	Rating	Reviews
Men’s Cotton T-shirt	₹499	4.2	210
Women’s Kurta Set	₹1,199	4.5	360
Denim Jeans	₹899	4.3	120


You can also export the scraped data to a CSV file for further analysis:
data.to_csv("flipkart_fashion_data.csv", index=False)

🌟 Future Enhancements

Add support for multiple categories (men, women, kids)

Handle pagination for larger datasets

Visualize pricing and rating trends

Automate daily data collection
