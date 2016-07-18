### Class 4 Homework: Command Line Chipotle
##### Answers

1. **order_id**: the unique identifier for each order /
**quantity**: the number purchased for each item /
**item_name**: the name of item being purchased /
**choice_description**: the list of modifiers for the item purchased /
**item_price**: the total price of the item(s) being purchased
    * `head chipotle.tsv`
    * `tail chipotle.tsv`

2. The highest **order_id** value is 1834, therefore there appears to be 1834 orders.
3. This file has 4623 lines.
    * `wc -l chipotle.tsv`

4. Chicken burritos are more popular than steak burritos.
    * `grep -ic 'chicken burrito' chipotle.tsv`
        *  *output = 553*
    * `grep -ic 'steak burrito' chipotle.tsv`
        *  *output = 368*
5. Chicken burritos more often have black beans than pinto beans.
    * `grep -ic 'chicken burrito.*black beans' chipotle.tsv`
        *  *output = 282*
    * `grep -ic 'chicken burrito.*pinto beans' chipotle.tsv`
        *  *output = 105*
6. List of CSV or TSV files in **DS-SEA-3** repo (all located in the **data** subdirectory):
   * `cd .. DS-SEA-3`
   * `find . -name *.?sv`
    *   Airline_on_time_west_coast.csv
    *   airlines.csv
    *   bank-additional.csv
    *   bikeshare.csv
    *   chipotle.tsv
    *   citibike_feb2014.csv
    *   drinks.csv
    *   drones.csv
    *   hitters.csv
    *   icecream.csv
    *   imdb_1000.csv
    *   mtcars.csv
    *   NBA_players_2015.csv
    *   ozone.csv
    *   pronto_cycle_share/2015_station_data.csv
    *   pronto_cycle_share/2015_trip_data.csv
    *   pronto_cycle_share/2015_weather_data.csv
    *   rossmann.csv
    *   rt_critics.csv
    *   ms.tsv
    *   stores.csv
    *   syria.csv
    *   time_series_train.csv
    *   titanic.csv
    *   ufo.csv
    *   vehicles_test.csv
    *   vehicles_train.csv
    *   yelp.csv
7. There are approximately 85 occurances of the word "dictionary" in the **DS-SEA-3** repo.
    * `grep -ir 'dictionary' . | wc -l`


    





