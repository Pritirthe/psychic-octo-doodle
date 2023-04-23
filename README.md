# psychic-octo-doodle
To design and develop a Data Acquisition and Pre-processing Pipeline 

Link to the repository https://github.com/Pritirthe/psychic-octo-doodle/blob/main/PythonAssignment2.ipynb

In this assignment we are using the web scraping for data acquisition from IMDB top 100 movie list and the link is: https://www.imdb.com/search/title/?groups=top_100&sort=user_rating,desc

Data Acquisition - Alphonsa John

The Data Acquisition (web scraping) code is done by Alphonsa John. In this IMDb Top 100 website we can seen top 100 movies details like the movie name, year of release, rating, and so on. For scraping we import the library called BeautifulSoup. The scraping code written with in the function called as get_data() with two parameters and they are url of the site and number of pages. This website is provide lots of information about each and every movie but we scrape only seven data from it and they are Rank, Name, Year, Rating, Metascore, Duration in mins, and Director name. Apart from any data from scrping we can append to the database directely.

Data Analysis - Priti Tirthe

Priti Tirthe have mainly work on data analysis pipeline, we connected the sql to database created using create_engine and connect it to con using sqlite3. Execute query with rs and save the result of the query in DataFrame df. Here we have import SQLITE3 and write the four queries which include finding movie name start with The and rating above 8, also movies information between 2010 to 2020 order descent to know recent movies and movies group by director and with count arrange in descending order. Also, movie with metascore above 80 order by rating in descending order.

Data Pre-processing - Tulika

I (Tulika) have worked on the pre-processing of the data and established the connection with Database. The dataset is nearly flawless and only little data cleaning was necessary. The values seem in line and there are no missing or invalid values in the dataset. We have dropped the id column and replaces all spaces with underscores and also removed the occurance of "(" and ")", by replacing them with strings. We used MongoDB Atlas to connect to Python using PyMongo library. The connection process involves creating a MongoClient object and we have specified the connection details such as credentials in the code. Also, PFB the same:
DB NAME: Jisons, COLLACTION NAME: movies and CREDS ( ID- tulikayadav16, PWD: 1WgLZ0xLWIAXPvJe  )
We have made sure in the code to drop the exixting collection using drop_collection. Pandas library has been used to perform the filtering, cleaning task.
