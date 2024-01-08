# Dynamic web scraping with selenium
This Jupyter Notebook file demonstrates an example of performing web scraping on a dynamically loaded product sales and review website. It serves as a reference for how to use the selenium library and not to be copied as all websites are different in their structure. 
# How to set up
1) Check your Google Chrome version
2) Download the corresponding Google Chrome Driver from https://chromedriver.chromium.org/downloads
3) Ensure that Jupyter Notebook and Python3 is installed
4) Install the selenium library on your terminal using pip install selenium
# How to understand
To retrieve a piece of information from a website, the HTML of the website must be accessed to extract its necessary information through the following methods:
1) find_element(By.___, "HTML selector"): retrieves the first element on the web page
2) find_elements(By.___, "HTML selector"): retrieves all the elements on the web page
3) WebDriverWait(driver, time).until(EC.presence_of_element_located((By.___, "HTML selector"))

The HTML selector commonly includes but is not exhaustive to: CLASS_NAME, XPATH, CSS_SELECTOR, TAG_NAME.

time.sleep(seconds) is set to allow the web page to render its information completely.

driver.execute_script("arguments[0].scrollIntoView({block: 'center'});", variable) scrolls the web page until the variable is in the middle of your computer screen.

variable.click() simulates a human mouse click on the web page element retrieved from any of the methods above.
