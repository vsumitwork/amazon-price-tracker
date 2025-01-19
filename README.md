# Amazon Product Price Tracker

This project is a web scraping application designed to monitor the price of a specific product on Amazon daily. The primary goal is to help users track price drops during sales events, such as Black Friday, by storing daily data in an Excel file.

## Project Overview

The application performs the following tasks:

1. **Scrapes Product Data:** Retrieves the product name, current price, and the date of scraping from a specific Amazon product page.
2. **Automates Daily Scraping:** The script runs daily to collect updated product information.
3. **Stores Data in Excel:** Saves the scraped data into an Excel file, making it easy to analyze and track price trends over time.

By comparing daily prices, users can identify price drops and make informed purchasing decisions during sales events.

## Features

- **Product Name Retrieval:** Extracts and records the product's name for easy identification.
- **Price Monitoring:** Captures the current price of the product daily.
- **Date Tracking:** Logs the date of each scrape to maintain a historical record.
- **Excel Integration:** Automatically appends new data to an Excel file for seamless data analysis.
- **User-Agent Customization:** Ensures reliable requests by including a User-Agent header to mimic browser behavior.

## Technologies Used

- **Python Libraries:**
  - `BeautifulSoup`: Parses HTML content for data extraction.
  - `requests`: Sends HTTP requests to fetch webpage content.
  - `datetime`: Handles date-related operations.
  - `smtplib`: (Optional) Can be used to send notifications if integrated.
  - `time`: Controls script timing for scheduled runs.
- **Excel File Management:** Stores and updates data efficiently.

## How to Use

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/vsumitwork/amazon-price-tracker.git
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Update the `url` variable in the script with the Amazon product link you wish to track.
4. Run the script manually or schedule it using a task scheduler (e.g., `cron` on Linux or Task Scheduler on Windows) to automate daily scraping.
5. Check the Excel file for updated price and date information.

## Example Output

An example row in the Excel file:
| Date       | Product Name            | Price  |
|------------|-------------------------|--------|
| 2025-01-16 | Anime T-Shirt for Men   | ₹500   |

## Prerequisites

- Python 3.7 or higher
- Basic understanding of Python and web scraping
- An active internet connection

## Notes

- This project is for educational purposes only. Ensure compliance with Amazon’s terms of service while scraping data.
- If additional features like email alerts are desired, they can be integrated using the `smtplib` library.

## Future Enhancements

- Add email notifications for price drops.
- Extend functionality to scrape multiple products concurrently.
- Implement data visualization to plot price trends.

---

Feel free to contribute or report issues by creating a pull request or opening an issue on the repository.

