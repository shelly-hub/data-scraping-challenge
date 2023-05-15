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
