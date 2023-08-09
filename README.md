
Aviation_Performance 
> This script is using the Selenium library for Python to automate the process of scraping data from the airportal.go.kr website. It is using the Chrome webdriver to open the website, enter login credentials and navigate through the pages on the website. The script then sets the start and end date for data scraping, and calculates the date range for each iteration of the loop depending on the term type (day, week, month, or year)
The script then calls the loop_func function, which loops through the website using the calculated date range, and each iteration it downloads an excel file of the data. After that, the script uses the mariadb library to save the data in a MariaDB database.
It also uses the time and urllib libraries to handle time-related tasks and handle URLs.
It uses the pandas library to handle and manipulate data in the excel file and numpy library for mathematical operations.
It uses the os library to handle the operating system related tasks such as creating folders and files.

Stock_Reflection 
> This code is used to scrape historical stock data for a list of airline companies listed on the KRX stock exchange, and then store that data in a MariaDB database. The code uses the FinanceDataReader library to scrape the stock data, and the mariadb library to connect to and interact with the database.
The code begins by importing the necessary libraries and defining some variables such as KRX as Stock Listing, start and end date for stock data, corporation stock list and their codes, etc.
>The code then defines a number of functions:
>>The make_sql() function is used to create an SQL query that will be used to insert data into the database.
>>The db_connect() function is used to connect to the MariaDB database.
>>The que_sql() function is used to execute the SQL query and insert the data into the database.
>>The main() function is the main driver of the code. This function iterates through the corporation stock list and their codes, scrapes the historical stock data for each company using the FinanceDataReader library, formats the data into a pandas dataframe, and then inserts the data into the MariaDB database using the que_sql() function.

>This code can be used to scrape historical stock data for any list of companies, not just airline companies. To do this, the user would need to modify the "corp_dict" variable with the appropriate company codes and names, and adjust the stock data start and end date accordingly. The user also needs to make sure that the MariaDB credentials match their database's credentials.

