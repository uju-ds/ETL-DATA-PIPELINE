# ETL-DATA-PIPELINE
Build an ETL Data pipeline extracting weather data via OpenWeather API (Python/PostgreSQL/SQL)

Building a data pipeline that pulls weather data from the OpenWeather API and loads it into a database involves several key steps. 
I'll walk you through the process and describe each stage, from setting up the API call to storing the data in a database.

# Steps to Build the Weather Data Pipeline
1. Set Up the Environment
You need to set up your development environment with the necessary tools and libraries: I used Jupyter notebook

Programming Language: Python is commonly used due to its libraries for API calls and database interaction.
Libraries:
requests for making API calls.
pandas for handling and cleaning the data.
sqlalchemy for connecting to and interacting with the database.
psycopg2 for PostgreSQL support (or an appropriate driver for your database).

2. Transform the Data 
In this step, you may need to transform the data before loading it into your database.

Convert timestamps into a specific format.
Convert temperature from Fahrenheit to Celsius (though the OpenWeather API can return temperatures in Celsius).
change the data from semi strutured (Json) to structured data(dataframe)

3. Load the Data in the Database
To store the data in the database, you will use SQLAlchemy along with pandas to directly load the data into a PostgreSQL database.
