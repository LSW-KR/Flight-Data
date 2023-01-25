"""
Aviation_Performance 
> This script is using the Selenium library for Python to automate the process of scraping data from the airportal.go.kr website. It is using the Chrome webdriver to open the website, enter login credentials and navigate through the pages on the website. The script then sets the start and end date for data scraping, and calculates the date range for each iteration of the loop depending on the term type (day, week, month, or year)
The script then calls the loop_func function, which loops through the website using the calculated date range, and each iteration it downloads an excel file of the data. After that, the script uses the mariadb library to save the data in a MariaDB database.
It also uses the time and urllib libraries to handle time-related tasks and handle URLs.
It uses the pandas library to handle and manipulate data in the excel file and numpy library for mathematical operations.
It uses the os library to handle the operating system related tasks such as creating folders and files.

Stock_Reflection 
> This code retrieves stock data for specific airlines at specific intervals, and inserts it into a database.
"""
