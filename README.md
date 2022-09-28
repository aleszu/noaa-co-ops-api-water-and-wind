# noaa-co-ops-api-water-and-wind
NOAA water and wind data for all Florida stations plus Fort Pulaski, GA and Charleston, SC  Hits the CO-OPS API every 5 minutes for water level and wind data using Actions and an R script.

Data dictionary [here](https://api.tidesandcurrents.noaa.gov/api/prod/#station).

Datum reference is MTL or mean tide level. More info on datums [here](https://tidesandcurrents.noaa.gov/datum_options.html).

```
t = Datetime in GMT
v = Observed water level (in feet)
```

Stations being tracked:

```
id	gauge	wind
8720030	Fernandina Beach, FL	Y
8720218	Mayport, FL	Y
8720219	Dames Point, FL	N
8720226	Southbank Riverwalk, St Johns River, FL	N
8720357	I-295 Buckman Bridge, FL	Y
8721604	Trident Pier, Port Canaveral, FL	Y
8722670	Lake Worth Pier, Atlantic Ocean, FL	Y
8722956	South Port Everglades, FL	Y
8723214	Virginia Key, Biscayne Bay, FL	Y
8723970	Vaca Key, Florida Bay, FL	Y
8724580	Key West, FL	Y
8725110	Naples, Gulf of Mexico, FL	Y
8725520	Fort Myers, FL	Y
8726384	Port Manatee, FL	N
8726520	St. Petersburg, Tampa Bay, FL	Y
8726607	Old Port Tampa, FL	Y
8726674	East Bay, FL	N
8726724	Clearwater Beach, FL	Y
8727520	Cedar Key, FL	Y
8728690	Apalachicola, FL	Y
8729108	Panama City, FL	Y
8729210	Panama City Beach, FL	Y
8729840	Pensacola, FL	Y
8670870	Fort Pulaski, GA	Y
8665530	Charleston, SC	Y![image](https://user-images.githubusercontent.com/6544861/192830150-fe2508b8-2dee-4d19-bf16-a3ebc7bbd761.png)

```
