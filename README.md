# data-scraping-challenge

## Project Aim
To learn web-scraping using python code through identifying HTML elements on a page. Web scraping involved collecting data, organising, extracting anf storing data, then analysing through visualisation of data. 

## Project Descriptions
This project extracts information of data through both autamated browsing with Splinter and HTML parsing with Beautiful Soup. The project is separated into 2 parts. 

 - One is using Mars News website to extract news article information such as titles and preview text in the webpage. 
 - Second is using Mars Temperature Data site to extract HTML tables into pandas dataframe. 
 
 ### Advantages of Web Scraping
  - Can be fast and efficient
  - Can extract same information through multiple pages at once
  - Useful for big data collectors
 
 ### Disadvantages
  - Not all websites can be used for scraping, need to check the legal requirement and protection polies
  - If webpage changes over time, code needs to get updated
  - Some data presented in webpage can be complex, needs more time for extraction and processed

## Project Method

### Installation
     1. Install ChromeDriver from the chrome website and follow its instructions
     2. Set up path to the local folder
     3. In the terminal, install following packages:
        - pip install "splinter[selenium4]"
        - pip install bs4
        - pip install html5lib
        - pip install lxml

### Scrape Title and Preview Text from Mars News Article
    1. Import dependencies such as Browser and BeautifulSoup
    2. create the URL link to visit chrome website
    3. Once on the webpage, right-click to go to inspect to direct to HTML element page. 
    4. Find the code on HTML element page for the title of each articles, and its preview text
    5. Identify the tags and classes for title and preview text, using find() function
    6. Create an empty list to store results by using combination of For loop method and list dictionary
    7. Optional: to create a Json file to view the scraped data

### Scrape and Analyse Mars Weather Data
   1. Same method as above, import dependencies and set up URL link and visit the website
   2. Instead of using Pandas, pd.read_html, this project continues to use python BeautifulSoup method to extract data.
   3. Here using For loop method looping through enumerate rows to obtain data for multiple columns
   4. After scraping table data, convert it into dataframe
   5. Data types also need to be converted as datetime, integer and float 
   6. Then begin the analysis using pandas
   7. Temperatures data vs Month are plotted to identify coldest and warmest months across the Martian Months
   8. The distance between 2 peaks of the minimum temperature indicates the equaivalent of terrestrial days to one Martian year
   9. Dataframe is then saved to csv file as mars.csv

## Reference
   - AttributeError: 'NoneType' object has no attribute 'text'. Web scraping indeed with Python [duplicate].(29/Jan/2020). Stack Overflow. Retrieved on 14/May/2023, from:<https://stackoverflow.com/questions/59960321/attributeerror-nonetype-object-has-no-attribute-text-web-scraping-indeed-w>
   - How to scrape second column from table.(9/Mar/2019). Stack Overflow. Retrieved on 14/May/2023, from:<https://stackoverflow.com/questions/55082199/how-to-scrape-second-column-from-table>
   - Convert float64 column to int64 in Pandas.(13/May/2017). Stack Overflow. Retrieved on 14/May/2023, from:<https://stackoverflow.com/questions/43956335/convert-float64-column-to-int64-in-pandas>
   - Pandas Count Unique Values in Column.(17/01/2023). SparkBy{Examples}. Retrieved on 14/May/2023, from:<https://sparkbyexamples.com/pandas/pandas-count-unique-values-in-column/>
   - pandas.DataFrame.sort_values.(2023). Pandas. Retrieved on 14/May/2023, from:<https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.sort_values.html>
   - How to save scraped data to JSON in Python.(20/Apr/2022)/ Stack Overflow. Retrieved on 15/May/2023, from:<https://stackoverflow.com/questions/71940341/how-to-save-scraped-data-to-json-in-python>
   - Module 11 - Data Collection Course Modules (4/5/2023). Monash University - Data Analytics Bootcamp
