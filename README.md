# Web Scraping and Data Extraction Project

## Objective

The goal of this project is to extract information about the top 50 movies with the best average rating from a specific web page and save the data in both a CSV file and a SQLite database.

## Web Page URL

- [100 Most Highly-Ranked Films](https://web.archive.org/web/20230902185655/https://en.everybodywiki.com/100_Most_Highly-Ranked_Films)

## Data to Extract

- Average Rank
- Film Title
- Year

## Tools and Libraries

- **requests**: For fetching the web page content
- **BeautifulSoup**: For parsing HTML and extracting data
- **csv**: For saving data to a CSV file
- **sqlite3**: For saving data to a SQLite database

## Steps

1. **Fetch the Web Page**: Use `requests` to retrieve the HTML content of the page.
2. **Parse HTML**: Use `BeautifulSoup` to analyze the HTML structure and locate the relevant data.
3. **Extract Data**: Identify and extract the Average Rank, Film Title, and Year for each movie.
4. **Save to CSV**: Write the extracted data to a CSV file named `top_50_films.csv`.
5. **Save to Database**: Insert the data into a SQLite database file named `Movies.db`, under a table named `Top_50`.

## Output

- **CSV File**: `top_50_films.csv`
- **SQLite Database File**: `Movies.db` with table `Top_50`

## Usage

To run the web scraping script, execute the following command:

```bash
python webscraping_movies.py
