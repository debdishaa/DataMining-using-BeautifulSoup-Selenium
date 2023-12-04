
# BeautifulSoup and Selenium Scraper

## Project Description
This Python project leverages the BeautifulSoup and Selenium libraries for web scraping official websites, with a specific focus on extracting Australian Business Number (ABN) details from the New South Wales (NSW) supplier portal. The repository provides a comprehensive guide and toolkit for efficiently collecting supplier information that is publicly available. It showcases the versatility and power of BeautifulSoup and Selenium in extracting crucial data from web sources.

### Example Website
The website used as an example for this project is the [NSW Supplier Portal] (https://buy.nsw.gov.au/supplier/search).

## Project Structure
The scraping project is organized into three distinct steps, each designed to streamline the process and reduce overall execution time:

1. **Scrape Company Details:**
   - Extract the company name and its specific link on the NSW portal.
   - Store these details in an Excel sheet for further use.

2. **Scrape Company Websites:**
   - Utilizing the links acquired from the NSW portal, the script scrapes for hyperlinks labeled "Go to supplier website" to obtain the company's official website URL.

3. **Scrape ABN Details:**
   - Again using the NSW portal links, the script scrapes for the ABN of each company, which is typically a 11-digit number formatted as 2-3-3-3.

## Efficiency Through Division and Parallel Execution
To enhance the efficiency of the scraping process:

- **Division into Parts:**
  - The project is divided into parts, each focusing on a specific aspect of the data (company details, website URLs, ABN).

- **Use of Pandas for Data Slicing:**
  - The project employs the Pandas library to further slice the data into manageable segments. This enables simultaneous processing of different data segments.

- **Parallel Execution in Google Colab:**
  - By running separate tabs in Google Colab for each data segment, the scraping process is significantly accelerated. This parallel execution approach reduces the overall time required for data collection.

