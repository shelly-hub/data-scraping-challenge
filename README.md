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
  - Some data presented in webpage can be complex, needs more to for extraction and processed

## Project Method

### Installation
1. Install ChromeDriver from the chrome website and follow its instructions
2. Set up path to the local folder
3. In the terminal, install following packages:
   - pip install "splinter[selenium4]"
   - pip install bs4
   - pip install html5lib
   - pip install lxml
 
