## Web Scraping with Selenium
This project aims to scrape a webpage using Python's Selenium library

# Scraping imdb.com for the Best Movies and retrieving extra information on the Top 10 as well as the top romance movies

1. Initially, to showcase the ability to navigate a website and its individual webpages using Selenium, the project begins at the IMDb homepage. From there, navigation proceeds towards the Top 250 movies webpage. 

2. Basic information on the Top 250 Movies, as rated by regular IMDb voters, is then retrieved using BeautifulSoup (bs4) and saved into a dataframe. This dataframe is subsequently exported as both a CSV and an XLSX for further analysis.

3. To further showcase mastery of Selenium and web scraping, detailed information on the Top 10 movies is gathered. This involves navigating the Selenium Driver to the individual movie webpages and using BeautifulSoup (bs4) to scrape additional information. The more detailed information for the Top 10 is stored in a separate dataframe and exported into a separate CSV and XLSX. Retrieving detailed information on all movies would be too time-consuming for a demonstration such as this. However, the code could be easily adapted to retrieve information on more movies, as the retrieval code is encapsulated within functions. These functions may, unfortunately, need adjustments if IMDb alters the structure of their website.

4. Lastly, to further showcase abilities with Selenium, the filter window on IMDb is utilized to retrieve the top romance movies. It is demonstrated that previously written functions can be reused for additional scraping tasks.

**Warning! Throughout the project, IMDb has occasionally changed class and ID names of different items. Therefore, functions were written in such a manner where classes and IDs are defined only once. This ensures that if a naming change occurs, only one variable or function needs adaptation. However, this does not guard against larger structural changes to the IMDb website, implying the program requires maintenance and has a limited shelf life.**

*Note: By default, the program saves the resulting CSVs and XLSXs to the working directory. Depending on the setup and Integrated Development Environment (IDE), this may be the active directory in which the Jupyter notebook file is located or it may be the base directory. In case the CSVs or XLSXs are not found, please check the base directory* 
