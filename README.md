# Web Scraping and Automation with Python

## Overview

This project focuses on web scraping from Craigslist and automating login on The Old Reader using Python. The objective is to develop Python scripts to scrape Craigslist listings, save HTML content, parse information from saved HTML files, and automate the login process for The Old Reader.

## Part 1 : Scraping and Saving HTML Content from Craigslist

### Fetching Listing URLs

- Used `requests` to access the first page of the "free" section and `BeautifulSoup` to parse HTML content.
- Identified the structure holding links to individual listing pages.
- Extracted the first 250 unique listing URLs and saved them to a list, considering pagination.

### Saved HTML Pages

- Fetched HTML content for each listing URL and saved it to a separate file on disk.
- Organized files using listing IDs for easy identification.

## Part 2: Parsing and Displaying Information from Saved HTML

### Read Saved HTML Files

- Write a script to read each saved HTML file from disk.

### Extracted Information

- Used `BeautifulSoup` to parse HTML content and extracted details such as title, image URL, description, post ID, posted date, and last updated date.

## Part 3: Automating Login on The Old Reader

### Creating and Verifying a The Old Reader Account

- Created an account on The Old Reader and manually verify login.

### Exploring the Login Mechanism

- Inspected the login page's `<form>` tag and `<input>` fields using browser developer tools.

### Analyzed Network Traffic for Login Request

- Identified the network request made during login and analyzed the payload submitted to the server.

### Automating the Login Process

- Simulated the login process using Python and `requests`.
- Maintainedd login state using session objects and send a POST request to the login form's action URL.

### Verifying Successful Login

- Inspected cookies saved in the session object and access The Old Reader to verify successful login.


This project demonstrates proficiency in web scraping, HTML parsing, and automation using Python. It provided practical experience in handling web data and interacting with web services programmatically.
