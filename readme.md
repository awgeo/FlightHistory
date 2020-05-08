# FlightHistory - cabin crew roster

Looking for a good data set to play with in Tableau, I got a hold of my partner's flight history as Cabin Crew for Virgin Atlantic. It's a fascinating data set, documenting 700 international flights over seven years (on which I've bagged myself a few spare seats!). 

### Data preparation
The notebooks and files in this GitHub repo describe the workflow required to prepare the data for vizualisation. 

The data is provided in two parts. First, data spanning Oct 2012 - Oct 2019 are provided in a series of Excel files ("Historical Crew Data"). Second, more recent but less detailed flight data (up to end-March 2020) is parsed from an iCalendar (.iCal) file. The data are combined and reconciled with Python/Pandas, along with additional geographical information (including airport lat/long) and distances calculated between origin/destination airports.

The final time-series data (output to 'flight_history_combined.xlsx') allows us to filter and categorise data on aircraft type, airport code, city, country, distance, flight time, shifts/blocks and roster periods. 

### Data vizualisation
Interactive plots published on Tableau Public: https://public.tableau.com/profile/alan.wilson7526#!/

Example - number of flights per aircraft type:

![](tableau_plots/Example_flights-per-aircraft-type.JPG)

Preview of final data set:

![](tableau_plots/Example_combined-data-set.JPG)
