## Overview

This project focuses on scraping mobile phone data from the Flipkart website, processing and analyzing the collected information, and storing structured data in a NoSQL database for efficient management. The workflow demonstrates end-to-end data analytics practices, including web scraping, data cleaning, exploratory analysis, and database integration.

## Project Objectives

* Extract mobile phone information from Flipkart using web scraping techniques.
* Clean and preprocess raw scraped data.
* Perform exploratory data analysis (EDA) to generate insights.
* Store structured and cleaned data in MongoDB for future use and scalability.

## Dataset

The dataset used in this project is created through web scraping from Flipkart's mobile phones listings.

### 📊 Collection Preview: `mobile_phones`
**Schema:**
```json
{
  "_id": {
    "$oid": "6a16d25811f37362908d85af"
  },
  "Product Name": "Samsung Galaxy F07 (Green, 64 GB)",
  "Offer": "16% off",
  "Camera": "50MP + 2MP | 8MP Front Camera",
  "Memory": "4 GB RAM | 64 GB ROM | Expandable Upto 2 TB",
  "Battery": "5000 mAh Battery",
  "Display": "17.02 cm (6.7 inch) HD+ Display",
  "Rating Number": 4.3,
  "Sale Price": 9999,
  "Actual Price": 11999,
  "No of Reviews": 4,
  "No of Ratings": 367
}
```

**Sample Documents:**
You can view the full dataset in [mobile_phones.json](mobile_phones.json).

## Tools & Technologies Used

### Programming Language

* Python

### Libraries Used

* BeautifulSoup
* Requests
* Pandas
* NumPy
* Matplotlib
* Seaborn
* PyMongo

### Database

* MongoDB

### Development Environment

* Jupyter Notebook / VS Code

## Project Workflow

### 1. Data Scraping

* Sent HTTP requests to Flipkart pages using Requests.
* Parsed HTML content using BeautifulSoup.
* Extracted mobile phone details from product listings.

### 2. Data Cleaning & Preprocessing

* Removed duplicate records.
* Handled missing values.
* Standardized column formats.
* Converted numerical fields into appropriate data types.

### 3. Exploratory Data Analysis (EDA)

* Analyzed pricing patterns.
* Compared ratings across brands.
* Identified popular brands and products.

### 4. MongoDB Integration

* Established connection with MongoDB.
* Converted cleaned datasets into structured documents.
* Inserted records into MongoDB collections.

## Key Insights

* Identified pricing trends among different smartphone brands.
* Analyzed customer preferences through ratings and reviews.
* Observed discount patterns across product categories.

## How to Run the Project

### Clone Repository

```bash
git clone <repository-link>
cd Flipkart-web-scraping
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

## Future Enhancements

* Automate scraping pipelines.
* Deploy dashboards for visualization.
* Add sentiment analysis on customer reviews.
* Schedule regular data updates.

## Conclusion

This project demonstrates practical skills in web scraping, data preprocessing, data analysis, and database integration while building an end-to-end analytics pipeline using real-world e-commerce data.
