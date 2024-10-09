# Brewery Data Scraping Project

This project scrapes brewery data from the [Brewers Association](https://www.brewersassociation.org) and extracts key information such as company name, phone number, website, brewery type, and address details. The data is then organized into a structured format using Python and stored as a CSV file for further analysis. \n The idea was to use scrapy to scrape the website, I however played arounf with the developer tools and noticed a json file containing all the data needed. \n this was then used for my GET request instead of using scrapy

## Project Structure

### Notebooks
- `scrape_brewery.ipynb`: This notebook contains the code to scrape and process brewery data.

### Output
- `BreweryData.csv`: The final dataset with the relevant brewery details extracted from the JSON source.

## Data Extracted

The following fields are extracted from the Brewers Association JSON data:

- `company_name`: Name of the brewery
- `company_phone`: Phone number of the brewery
- `company_website`: Website of the brewery (if available)
- `company_type`: Type of the brewery (e.g., Microbrewery, Brewpub, etc.)
- `company_city`: City where the brewery is located
- `company_state`: State where the brewery is located
- `company_street`: Street address of the brewery
- `company_streetCode`: Street code (state code)
- `Data extracted was stored into the 'BreweryData.csv' file

## Installation

To run the notebook and scrape the brewery data, you need the following libraries installed:

```bash
pip install requests pandas
```

## Usage

1. Clone the repository and open the Jupyter notebook.
2. Run the notebook cells sequentially to:
   - Fetch the brewery data from the Brewers Association API.
   - Extract the relevant fields using helper functions.
   - Store the extracted data into a CSV file for further analysis.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
