# noaa-co-ops-api-water-and-wind
NOAA water and wind data for all Florida stations plus Fort Pulaski, GA and Charleston, SC  Hits the CO-OPS API every 5 minutes for water level and wind data using Actions and an R script.

Data dictionary [here](https://api.tidesandcurrents.noaa.gov/api/prod/#station).

Datum reference is MTL or mean tide level. More info on datums [here](https://tidesandcurrents.noaa.gov/datum_options.html).

```
t = Datetime in GMT
v = Observed water level (in feet)
```
