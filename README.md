# Automated-Market-Intelligence-Scraper
Python-based web scraper built with BeautifulSoup to automate e-commerce data collection and competitive price analysis.

Book Market Analysis

This repository contains a Jupyter Notebook (Book_Market_Analysis.ipynb) that demonstrates web scraping, data cleaning, analysis, and visualisation of book data from books.toscrape.com.

Table of Contents
•	Project Overview
•	Features
•	Data Source
•	Setup and Installation
•	Usage
•	Analysis Highlights
•	Visualizations
•	Output

Project Overview
This project aims to extract book information from an online bookstore, process the data, and perform an exploratory analysis to understand market trends, particularly focusing on book prices and their distribution across different star ratings.

Features
•	Web Scraping: Extracts book titles, prices, and stock availability.
•	Data Cleaning: Processes raw scraped data, handles currency symbols, and converts data types.
•	Data Transformation: Converts prices from GBP to INR and creates a boolean 'Is_Available' column.
•	Market Analysis: Calculates average prices by book rating.
•	Data Visualisation: Generates various plots to visualise data distributions and relationships.
•	Report Generation: Exports cleaned data and analysis summaries to an Excel file.

Data Source
The data is scraped from the first page of http://books.toscrape.com/, a sandbox website for web scraping practice.

Setup and Installation
To run this notebook, you'll need Python and a few libraries. It's recommended to use a virtual environment.
1.	Clone the repository (if applicable):
2.	git clone <repository_url>
 cd <repository_name>
3.	Install the required libraries:
4.	pip install requests beautifulsoup4 pandas matplotlib seaborn openpyxl
(Note: openpyxl is required for saving data to Excel files.)

Usage
Open the Book_Market_Analysis.ipynb notebook in Jupyter or Google Colab and run the cells sequentially. The notebook is structured into the following sections:
1.	Installation: Installs necessary libraries.
2.	Imports: Imports requests, BeautifulSoup, and pandas.
3.	Web Scraping: Code to fetch the webpage and extract initial data.
4.	Data Cleaning & Transformation: Steps to clean prices, convert to INR, and create Is_Available status.
5.	Market Analysis: Computes average prices per star rating.
6.	Visualisations: Generates various plots to display findings.
7.	Export Data: Saves the processed data and summary to an Excel file.
   
Analysis Highlights
Based on the scraped data from the first page:
•	Pricing by Rating: Books rated 'Three' had the highest average price (£42.32), while 'Four'-star books had the lowest (£31.11).
•	Rating Distribution: 'One'-star rated books were the most frequently encountered in this specific sample.

Visualizations
The notebook includes several visualisations to illustrate the data:
•	Bar Plot: Average Price by Book Rating.
•	Count Plot: Distribution of Book Ratings.
•	Box Plot: Price Distribution by Book Rating, showing median, quartiles, and outliers.
•	Histogram: Overall Distribution of Book Prices.
•	Violin Plot: Price Distribution by Book Rating, showing density and spread.

Output
The project generates an Excel file named Market_Analysis_Report.xlsx with two sheets:
•	Raw_Scraped_Data: Contains the full dataset with cleaned and transformed columns.
•	Price_Analysis: Contains the summary of average prices and counts by book rating.

