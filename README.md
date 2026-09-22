# Indian Two-Wheeler Market Intelligence

## Web Scraping, Data Cleaning, EDA and Price–Performance Analysis Using Python

## Project Overview

This project analyzes the Indian two-wheeler market using publicly available bike listing information collected from BikeWale.

The project follows an end-to-end data science workflow:

**Web Scraping → Data Collection → Data Cleaning → Feature Engineering → Exploratory Data Analysis → Market Segmentation → Business Insights**

A total of **444 unique bike listings** were collected and analyzed using Python.

The analysis focuses on relationships between bike price, engine capacity, power, mileage, weight and user ratings.

---

## Business Problem

The Indian two-wheeler market contains bikes across a wide range of prices, engine capacities, performance levels and efficiency levels.

The objective of this project is to collect structured bike information from a public web source and analyze the dataset to understand:

- How bike price varies with engine capacity and power
- How engine capacity and power relate to mileage
- How bikes are distributed across different price segments
- How average pricing differs across brands
- Whether bike ratings have a strong relationship with price
- How performance and efficiency vary across market segments

---

## Project Objectives

- Scrape structured bike information using Python
- Build a dataset containing at least 400 bike listings
- Clean and standardize scraped data
- Handle missing values and inconsistent formats
- Perform exploratory data analysis
- Analyze relationships between important numerical features
- Create price-based market segments
- Engineer performance-related features
- Identify meaningful market patterns and business insights
- Export the cleaned dataset for further analysis

---

## Data Source

**Website:** BikeWale

The data was collected from publicly accessible bike listing pages using:

- `requests`
- `BeautifulSoup`
- HTML parsing
- Regular expressions

The scraping process collected bike listing information across multiple pages.

> Note: The dataset represents a snapshot of publicly available listings at the time of collection. It should not be interpreted as a complete representation of the entire Indian two-wheeler market.

---

## Dataset

### Final Dataset

- **Records:** 444
- **Features:** 13
- **Duplicate bike URLs:** 0

### Main Features

| Feature | Description |
|---|---|
| `bike_name` | Name of the bike |
| `brand` | Bike manufacturer/brand |
| `bike_url` | BikeWale detail-page URL |
| `rating` | User rating |
| `rating_count` | Number of ratings |
| `engine_cc` | Engine capacity in cc |
| `mileage_kmpl` | Mileage in km/l |
| `power_bhp` | Engine power in BHP |
| `weight_kg` | Bike weight in kg |
| `ex_showroom_price` | Ex-showroom price |
| `price_segment` | Price-based market segment |
| `power_to_weight` | Power-to-weight ratio |
| `price_per_bhp` | Price per unit of engine power |

---

## Web Scraping Process

The scraping pipeline was developed using Python.

### Workflow

```text
BikeWale
   ↓
HTTP Requests
   ↓
HTML Pages
   ↓
BeautifulSoup Parsing
   ↓
Bike Listing Extraction
   ↓
Data Validation
   ↓
Raw Dataset
