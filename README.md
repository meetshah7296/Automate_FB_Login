# Automate_FB_Login
Automation Script to Login to Facebook

We use selenium here to open the site of our requirement (in this case Facebook) and there we inspect element across email box, password box and login button to find id of them.

Using find_element_by_id() function provided by selenium module, we can find the required element (username box, password box, login button)
Using send_keys() function, provided by selenium module, we will send the data into the box.

Installing third party modules required: Selenium 

Additional Requirement : geckodriver for firefox and 
                         chromedriver for chrome
Importing necessary modules
  Selenium : to automate browser
  Time : to pause running of script for some seconds as browsers try to detect automation stuff if we input too fast

Taking username and password as input from user

Using input() function and passing prompt message as argument.

Opening browser and required website

webdriver.Chrome() will open new window of chrome. We will save it’s object in variable named driver.

Now using get function we will open up Facebook website.

Finding element for sending data and Sending input

Use inspect element tool on the element of browser of which you want to find id. In this case we will inspect username box, password box, login button to find their id. And then use this id combining with selenium function find_element_by_id() to find it across web page and save it in variables for later use. Then by using send_keys() we will send data across the elements found previously.

Closing the browser 

After all of the above steps we have to quit the session and will be achieved by using driver.quit().

Note: Here driver is the name of variable you chose for webdriver.Chrome().
