
# Build Hotel Database Using Web Scrapping

## Hotel Pricing Estimation Database
  In this project, I scraped the listings on booking.com from March 20 to March 25, for three different popular vacation locations in California – San Diego, Los Angeles, and Yosemite National Park. Below are five processes to complete the task. <br>
  
  Firstly, I used Selenium to open a browser and manually navigate to booking.com. By doing so, I found that booking.com is not actively detecting Selenium and hence it is a good target for web scrapping. <br>
  
  Secondly, I leveraged Selenium to automate the search procedures, including typing in the trip destination, selecting the check-in and check-out dates, and ultimately reaching the result pages. I then saved the first 5 result pages for each of the three locations to disk. <br>
  
  Thirdly, I utilized BeautifulSoup to pulled out the saved pages and parsed out critical information including location, hotel name, link, distance from center, price, review score, number of reviews, star ratings, free breakfast, and free cancellation options. <br>
  
  The fourth step I took was to query each hotel address’s geolocation via the API provided by positionstack.com. <br>
  
  Lastly, I created a MongoDB collection and store it as a JSON file. <br>
