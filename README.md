# NOAA water and wind data for all Florida stations plus Fort Pulaski, GA and Charleston, SC
Hits the CO-OPS API every 5 minutes for water level and wind data using Actions and an R script.

Data dictionary [here](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html).

Datum reference is MTL or mean tide level. More info on datums [here](https://tidesandcurrents.noaa.gov/datum_options.html).

For water levels: 

```
t = Datetime in GMT
v = Observed water level (in feet)
s = Sigma - Standard deviation of 1 second samples used to compute the water level height
f = Data Flags - in order of listing:
    -- (O) Count of number of 1 second samples that fall outside a 3-sigma band about the mean
    -- (F) A flag that when set to 1 indicates that the flat tolerance limit was exceeded
    -- (R) A flag that when set to 1 indicates that the rate of change tolerance limit was exceeded
    -- (L) A flag that when set to 1 indicates that either the maximum or minimum expected water level height limit was exceeded 
q = Quality Assurance/Quality Control level
    -- p = preliminary
    -- v = verified 
```

For wind: 

```
t =	Time - Date and time of the observation
s =	Speed - Measured wind speed
d =	Direction - wind direction in degrees
dr= Direction - wind direction in text
g =	Gust - Measured wind gust speed
f =	Data Flags - in order of listing:
    -- (X) A flag that when set to 1 indicates that the maximum wind speed was exceeded
    -- (R) A flag that when set to 1 indicates that the rate of change tolerance limit was exceeded 
```

Stations being tracked:

|	id	|	gauge	|	wind	|
|	---	|	---	|	---	|
|	8720030	|	Fernandina Beach, FL	|	Y	|
|	8720218	|	Mayport, FL	|	Y	|
|	8720219	|	Dames Point, FL	|	N	|
|	8720226	|	Southbank Riverwalk, St Johns River, FL	|	N	|
|	8720357	|	I-295 Buckman Bridge, FL	|	Y	|
|	8721604	|	Trident Pier, Port Canaveral, FL	|	Y	|
|	8722670	|	Lake Worth Pier, Atlantic Ocean, FL	|	Y	|
|	8722956	|	South Port Everglades, FL	|	Y	|
|	8723214	|	Virginia Key, Biscayne Bay, FL	|	Y	|
|	8723970	|	Vaca Key, Florida Bay, FL	|	Y	|
|	8724580	|	Key West, FL	|	Y	|
|	8725110	|	Naples, Gulf of Mexico, FL	|	Y	|
|	8725520	|	Fort Myers, FL	|	Y	|
|	8726384	|	Port Manatee, FL	|	N	|
|	8726520	|	St. Petersburg, Tampa Bay, FL	|	Y	|
|	8726607	|	Old Port Tampa, FL	|	Y	|
|	8726674	|	East Bay, FL	|	N	|
|	8726724	|	Clearwater Beach, FL	|	Y	|
|	8727520	|	Cedar Key, FL	|	Y	|
|	8728690	|	Apalachicola, FL	|	Y	|
|	8729108	|	Panama City, FL	|	Y	|
|	8729210	|	Panama City Beach, FL	|	Y	|
|	8729840	|	Pensacola, FL	|	Y	|
|	8670870	|	Fort Pulaski, GA	|	Y	|
|	8665530	|	Charleston, SC	|	Y	|

