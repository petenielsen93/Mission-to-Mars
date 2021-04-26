# Mission-to-Mars

## Overview
In this module, we created a web app that uses Beautiful Soup and Splinter to scrape the web for data, store it in a Mongo database, and display it using Flask. In our challenge, we added a new section to the web app, that scrapes the web for full resolution Mars hemisphere images and their titles, adds them to the web app, and then we added components to customize the page. 

To scrape our web data, we used Beautiful Soup and Splinter to dig into the website's HTML. Looking into our scraping.py file, we set our URL variable to the hemisphere image website, and directed the webdriver_manager to open the browser and visit the URL. After creating an empty list to hold our data, we wrote some code that navigated the website, found the image HTML tag, add the title and image URL to our list, and quit the browser.

Using our HTML file, we added the images and titles for the hemispheres in order for them to display correctly in our web app. We also edited the look of the web app so that the hemisphere pictures were spherical, and the button to scrape was made smaller. I had some difficulty in this section adding the code to loop through our database ({% for hemisphere in mars.hemispheres %}). This module was a big challenge for me as I had minimal prior experience working with HTML. 