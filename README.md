# SQLAlchemy-challenge

#Part 1: Analyzed and Explored the Climate Data by using Python and SQLAlchemy to do a basic climate analysis and data exploration on the database. Used SQLAlchemy ORM queries, Pandas, and Matplotlib for the follwing: 
 

1. Used the SQLAlchemy create_engine() function to connect to SQLite database.

2. Used the SQLAlchemy automap_base() function to reflect tables into classes, and then save references to the classes named station and measurement.

3. Linked Python to the database by creating a SQLAlchemy session.

4. Performed a precipitation analysis and then a station analysis by completing the steps in the following two subsections.

#Precipitation Analysis

1. Find the most recent date in the dataset.

2. Using that date, get the previous 12 months of precipitation data by querying the previous 12 months of data.

3. Select only the "date" and "prcp" values.

4. Load the query results into a Pandas DataFrame. Explicitly set the column names.

5. Sort the DataFrame values by "date".

6. Plot the results by using the DataFrame plot method.

7. Use Pandas to print the summary statistics for the precipitation data.

#Station Analysis

1. Design a query to calculate the total number of stations in the dataset.

2. Design a query to find the most-active stations (that is, the stations that have the most rows). To do so, complete the following steps:
  * List the stations and observation counts in descending order.
  * Find which station id has the greatest number of observations?

3. Design a query that calculates the lowest, highest, and average temperatures that filters on the most-active station id found in the previous query.

4. Design a query to get the previous 12 months of temperature observation (TOBS) data. To do so, complete the following steps:
   * Filter by the station that has the greatest number of observations.
   * Query the previous 12 months of TOBS data for that station.
   * Plot the results as a histogram with bins=12, as the following image shows:

5. Close your session.

   #Part 2: Design Your Climate App
Designed a Flask API based on the developed queries. Created routes with Flask for the following:

   * Start at the homepage.
   * List all the available routes.
   * Convert the query results from your precipitation analysis (i.e. retrieve only the last 12 months of data) to       a dictionary using date as the key and prcp as the value.
   * Return a JSON list of stations from the dataset.
   * Query the dates and temperature observations of the most-active station for the previous year of data.
   * Return a JSON list of temperature observations for the previous year.
   * Return a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a           specified start or start-end range.
   * For a specified start, calculate TMIN, TAVG, and TMAX for all the dates greater than or equal to the start           date.
   * For a specified start date and end date, calculate TMIN, TAVG, and TMAX for the dates from the start date to         the end date, inclusive.


