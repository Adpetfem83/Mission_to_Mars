# Mission-to-Mars
#### *HTML Web scraping on Mars data to create a Flask web application using Python and MongoDB*

## Overview
This project is made up of a Python script to scrape text and images from different websites pertaning to Mission to Mars. With this in mind, I created a Flask web application with a rendered HTML template designed using Bootstrap to display all the data in a central location without having to gather it manually. The data displayed was scraped and stored in a non-relational Mongo database. In addition, I connected the scraping script so that each time a button is clicked, the scraping occurs once again, the database equally get updated, and new data is displayed. However, there is a condition for the button to work; HTML components I used for scraping the webpages must remain the same. Therefore, by using Bootstrap's grid system, I created a responsive web app that could allow any device to view it. 

## Resources used
- Web pages scraped: 
  - https://data-class-mars.s3.amazonaws.com/Mars/index.html
  - https://spaceimages-mars.com
  - https://galaxyfacts-mars.com
  - https://marshemispheres.com/
  - 
- Software packages used include:
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


The final outcome of this project was a fully-functional web application that is created with Flask that included images, a table with information about Mars in comparison to Earth, and the latest article title and short description scraped from the NASA's webpage. Meanwhile, each time "Scrape New Data" button is clicked, new information is updated on both the website and the MongoDB.

![MongoDB_Mars_ss](https://github.com/Adpetfem83/Mission_to_Mars/blob/main/Images/Screen%20Shot%202022-11-24%20at%209.06.29%20AM.png)

The scrape included a `news_title` with its brief explanation (`news_paragraph`), a `featured_image`, a table HTML component stored in `facts`, and four picture thumbnails, with their titles, of the different Mars' hemispheres stored in `hemispheres`. 

Furthermore, as database is updated each time new data is scraped, it is also saved with a "last_modified" date to know last time the button was clicked, this is shown at the bottom of the query results below. In this case, it was on November 24th, 2022. 

