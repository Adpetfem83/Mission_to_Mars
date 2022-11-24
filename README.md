# Mission-to-Mars
#### *HTML Web scraping on Mars data to create a Flask web application using Python and MongoDB*

## Overview
This project consisted on a Python script to scrape text and images from various websites that talked about Mission to Mars. Then, I created a Flask web application with a rendered HTML template designed using Bootstrap to display all the data in a central location without having to gather it manually. The data scraped and displayed was stored in a non-relational Mongo database. Additionally, I was able to connect the scraping script so that each time a button was clicked, the scraping occured once again, the database got updated, and new data was displayed. This button only works under the condition that these webpages don't change their HTML components I used for scraping. And lastly, by using Bootstrap's grid system I was able to create a responsive web app that could accomodate to any device people view it from. 

## Resources 
- Web pages scraped: 
  - https://data-class-mars.s3.amazonaws.com/Mars/index.html
  - https://spaceimages-mars.com
  - https://galaxyfacts-mars.com
  - https://marshemispheres.com/
- Software:
  - Python
  - Jupyter Notebook
  - Pandas, BeautifulSoup, Splinter, ChromeDriverManager, Flask, PyMongo
  - MongoDB
  - HTML5
  - Bootstrap 3

## Summary
![WebApp_ss](https://user-images.githubusercontent.com/83378141/126406623-e456cc0a-2828-44f9-9383-9512e3350608.png)

*Viewing it from an Iphone:*

![Screen Shot 2022-11-24 at 7 38 40 AM](https://user-images.githubusercontent.com/83378141/126408492-1cf71aed-dcb2-4992-8dab-cce986f0c76f.png)
![Screen Shot 2022-11-24 at 7 38 59 AM](https://user-images.githubusercontent.com/83378141/126408500-488d129b-a195-4a74-8071-412ba22fe992.png)


The final product was a fully-functional web application creted with Flask that included images, a table with information about Mars in comparison to Earth, and the latest article title and short description scraped from the NASA's webpage. Each time we click on the "Scrape New Data" button new information will be updated on both the website and the MongoDB.

![MongoDB_Mars_ss](https://github.com/Adpetfem83/Mission_to_Mars/blob/main/Images/Screen%20Shot%202022-11-24%20at%209.06.29%20AM.png)

The scrape included a `news_title` with its brief explanation (`news_paragraph`), a `featured_image`, a table HTML component stored in `facts`, and four picture thumbnails, with their titles, of the different Mars' hemispheres stored in `hemispheres`. 

In addition, the database will be updated and each time new data is scraped it will be saved with a "last_modified" date to know when was the last time, as you can see in the bottom of the query results. In this case, it was on July 7th of 2021. 

