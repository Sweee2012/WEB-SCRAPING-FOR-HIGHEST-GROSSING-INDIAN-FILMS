# WEB-SCRAPING-FOR-HIGHEST-GROSSING-INDIAN-FILMS
This project scrapes the list of highest-grossing Indian films from Wikipedia using the `pandas` library. It extracts the first table from the page, which includes details like box office earnings and release years. The data is loaded into a pandas Data Frame for easy analysis and manipulation. This project demonstrates a simple approach to scraping the list of the highest-grossing Indian films using the `pandas` library in Python. 

The code:

```python
import pandas as pd
pd.read_html('https://en.wikipedia.org/wiki/List_of_highest-grossing_Indian_films')[0]
```

1. **Importing `pandas`:** The `pandas` library is imported to handle data in a structured format (DataFrames), which makes it easier to analyze and manipulate.
   
2. **Scraping Data with `read_html()`:** The `pd.read_html()` function is used to scrape all the tables from the provided Wikipedia page (https://en.wikipedia.org/wiki/List_of_highest-grossing_Indian_films), which contains information about Indian films and their worldwide box office earnings.

3. **Selecting the First Table:** The function returns a list of DataFrames (one for each table found on the page). `[0]` is used to select the first table, which contains the list of highest-grossing Indian films, including details like the movie titles, worldwide box office earnings, release years, and more.

**How It Works:**

The project leverages the pandas.read_html() function, which extracts all the tables from a given URL and converts them into pandas DataFrames. By selecting the first table from the Wikipedia page, the project isolates the data of interest (highest-grossing Indian films). This approach makes it incredibly simple and efficient to scrape structured data from websites. This minimalistic code is an efficient way to scrape, extract, and analyze data about the highest-grossing Indian films, which can be further processed for insights or other applications.

---
