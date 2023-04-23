# psychic-octo-doodle
To design and develop a Data Acquisition and Pre-processing Pipeline 
Link to the repository https://github.com/Pritirthe/psychic-octo-doodle/blob/main/PythonAssignment2.ipynb
In this assignment we are using the web scraping for data acquisition from IMDB top 100 movie list and the link is: https://www.imdb.com/search/title/?groups=top_100&sort=user_rating,desc
Data Acquisition - Alphonsa John
In this website we can seen top 100 movie details like name, year of release, rating, and so on. 
The Data Acquisition (web scraping) code is done by Alphonsa John. For scraping import the library called BeautifulSoup. The scraping code written with in the function called as get_data()with two parameters are url and number of pages. From this website we scrape only 7 data and they are Rank, Name, Year, Rating, Metascore, Duration in mins, and Director name.
Data Analysis - Priti Tirthe
Priti Tirthe have mainly work on data analysis pipeline, we connected the sql to database created using create_engine and connect it to con using sqlite3. Execute query with rs and save the result of the query in DataFrame df. Here we have import SQLITE3 and write the four queries which include finding movie name start with The and rating above 8, also movies information between 2010 to 2020 order descent to know recent movies and movies group by director and with count arrange in descending order. Also, movie with metascore above 80 order by rating in descending order.
