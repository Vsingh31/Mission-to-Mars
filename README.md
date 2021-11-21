# Mission-to-Mars
**HTML Web scraping on Mars data to create a Flask web application using Python and MongoDB**
## Overview
The mission with this project was to learn web scraping methods to extract information from the [Mars Hemispheres](https://astrogeology.usgs.gov/search/results?q=hemisphere+enhanced&k1=target&v1=Mars) website using Chrome Developer tools to identify HTML components, Beautiful Soup/Splinter to automate a web browser and perform the scrape, MongoDB to store the data, and finally Flask to create a web application to display the data. Through the process, the goal was to develop an app to scrape the following information about the planet Mars:

* Latest News
* Featured Image
* Facts about the planet
* Images of the hemispheres
* 
### Deliverable 1 : Scrape Full-Resolution Mars Hemisphere Images and Titles
To start, I created the file "Mission_to_Mars_Challenge.ipynb" in Jupyter notebook to perform the scraping activity and Using BeautifulSoup and Splinter, I scraped  full-resolution images of Mars’s hemispheres and the titles of those images and I got the image URLs and titles for all four hemisphere images.The images of Mars’s hemispheres and the titles of those images are:-

![deliverable1](https://user-images.githubusercontent.com/90277142/142753525-ba423b4b-56ea-47ba-853e-fe3167c88beb.png)

### Deliverable 2 :  Update the Web App with Mars Hemisphere Images and Titles
we exported our Jupyter notebook file into a Python script. Using this script as the starting point, we started to define the scraping process using Visual Studio Code to edit our Python script. We added functions to scrape through the website(s) and loop through the HTML tags to return the information used to create a database to be stored in MongoDB.Using the database in Mongo, we create a Flask app to connect to the information and create our app routes. These routes help to display the information on the home page and will perform the scraping of new data using the codes that we wrote in the Python script.

Next, we integrate Mongo into the web app so that the data stored is updated every time the script, "Scraping.py" is run.
Using your Python and HTML skills, you’ll add the code you created in Deliverable 1 to your scraping.py file, update your Mongo database, and modify your index.html file so the webpage contains all the information you collected in this module as well as the full-resolution image and title for each hemisphere image.After you have scraped the data, confirm that your webpage has the full-resolution images and the titles of the four hemisphere images, like the image below.

![hemispheres](https://user-images.githubusercontent.com/90277142/142754248-aa758b35-44e2-4ad0-b01c-5898828e5bee.png)

### Deliverable 3 : Add Bootstrap 3 Components
I updated my web app to make it mobile-responsive, and added two additional Bootstrap 3 components to make it stand out.
To complete the final deliverable, the following changes were made to the Bootstrap components to customize the view of the page:

(1) I updated my index.html file so my website is mobile-responsive.I also Used the DevTools to test the responsiveness of my website by clicking Toggle Device Toolbar icon to       open the UI that enables you to simulate responsiveness.And i Chose a Mobile device(Iphone5) to test my webpage.

![mobileresponsiveness](https://user-images.githubusercontent.com/90277142/142754993-d375e709-63f9-4c61-80cf-29451f906b7e.png)




(2) Updated the color of the Jumbotron header by adding gradient color shading and changing the color of the scrape button.

original tag <div class_"jumbotron text-center"> & <a class="btn btn-primary btn-lg">
  
updated tag <div style="background:linear-gradient(to bottom, #ffcccc 15%, #e9967a 85%)!important" class="jumbotron text-center"> & <a class="btn btn-default btn-lg">
  
(3) Changed the orientation of the hemisphere images to a single ribbon by changing the grid from col-md-6 to col-md-3.  
  
(4) Updated the background color of the entire webpage by modifying the <body> tag with <body style="background-color:darksalmon; color:black">.  
  .
