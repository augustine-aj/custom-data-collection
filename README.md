# custom-data-collection

# Flipkart Review Scraper

## Overview
This project is a web scraping tool that extracts customer reviews from Flipkart product pages using Selenium and XPath. The scraped data includes customer ratings, review titles, review text, reviewer names, locations, and likes/dislikes. The extracted information is stored in a CSV file for further analysis.

## Features
- Scrapes customer reviews and related data from Flipkart.
- Uses XPath to locate elements on the page.
- Supports pagination to scrape multiple pages of reviews.
- Saves the collected data into a CSV file.

## Technologies Used
- **Python**: Programming language used for the scraper.
- **Selenium**: For browser automation and web scraping.
- **Pandas**: For data handling and exporting to CSV.
- **XPath**: For navigating the HTML structure of the Flipkart page.

## Getting Started

### Prerequisites
- **Python 3.x** must be installed on your system.
- **ChromeDriver** should match your Chrome browser version. Download it from [ChromeDriver Download](https://sites.google.com/chromium.org/driver/) and place the path in the script.

## How It Works
- **Browse the Website**: The script opens the specified Flipkart product review page.
- **Get Elements**: It retrieves reviews using pre-defined XPath for various elements like ratings, review titles, and text.
- **Pagination**: The script automatically navigates to the next page of reviews.
- **Simulate Clicks**: It can simulate user actions to expand additional review details if needed.
- **Save to CSV**: All the collected data is saved into `review_data.csv`.

## Example Output
The output will be stored in `review_data.csv` with columns such as:
- `customer_rating`
- `customer_reviewTitle`
- `customer_review`
- `customer_name`
- `customer_place`
- `customer_postedDate`
- `customer_reviewLikes`
- `customer_reviewDislikes`

## Future Improvements
- Handle dynamic loading of reviews more robustly.
- Extract additional data points, such as images or verified purchase statuses.
- Enhance error handling and logging mechanisms.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Thanks to the Selenium community for their invaluable resources and support.
- Flipkart for providing publicly accessible review data.

