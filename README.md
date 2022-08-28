# Missions_to_Mars

#### *HTML Web scraping on Mars data to create a Flask web application using Python and MongoDB

## Project Overview
---
This project uses Python script to scrape text images and images from several web site that discuss the mission to mars.  I creaated the flask web application to render an html template designed using Bootstrap to display all the data in a single location saving time not having to gather the information manaully from multiple web sites. The scraped data and display was stored in a non-relational Mongo database. Additionally, I was able to connect the scraping script so that each time a button was clicked, the scraping occured once again updating the database. This button only works under the condition that these webpages don't change their HTML components I used for scraping. By using Bootstrap's grid system I was able to create a responsive web app that could accomodate to any device people view it from.

## Reqources
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

The final product was a fully-functional web application creted with Flask that included images, a table with information about Mars in comparison to Earth, and the latest article title and short description scraped from the NASA's webpage. Each time we click on the "Scrape New Data" button new information will be updated on both the website and the MongoDB.

![MongoDB_Mars_ss](https://user-images.githubusercontent.com/83378141/126407244-089f0eb3-181d-4711-bef3-8ea0df916835.png)

The scrape included a `news_title` with its brief explanation (`news_paragraph`), a `featured_image`, a table HTML component stored in `facts`, and four picture thumbnails, with their titles, of the different Mars' hemispheres stored in `hemispheres`. 

### The End
