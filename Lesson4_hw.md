#Lesson 4 Homework: Command Line Chipotle
##1. 
Answer - The data file represents the total or a subset of all individual orders at a Chipotle for a given day.
Code - Downloaded the Chipotle.tsv file to my local folder C:\users\willpran\Desktop\DS Class\Homework and then used head chipotle.tsv and "tail chipotle.tsv
##2. 
There appear to be 1,834 orders. 
I used tail chipotle.tsv to go to the bottom and then looked at the max file
##3.
There are 4,623 lines in the file.
wc chipotle.tsv is the code to describe the file.
##4.
Chicken is a more popular burrito choice. Chicken burrito shows 553 times and steak shows 368 times
I first counted the number of times of "chicken burrito" and "steak burrito" show in the file and then saved each one to a tsv file
$ grep -i "chicken burrito" chipotle.tsv >> chicken_burrito.tsv
$ grep -i "steak burrito" chipotle.tsv >> steak_burrito.tsv
I then ran wc on each tsv to count the number of lines
##5. 
Chicken have black beans more often than pinto beans
I ran the following code to create a black bean file and then count the number of lines in it
$ grep -i "black beans" chipotle.tsv > chicken_black_beans.tsv
$ wc chicken_black_beans.tsv
I ran the following code to create a pinto bean file and then count the number of lines in it
$ grep -i "pinto beans" chipotle.tsv > chicken_pinto_beans.tsv
$ wc chicken_pinto_beans.tsv
##6.
I found all of the csv files by running $ find . -name .csv
The csv list includes:
./data/airlines.csv
./data/Airline_on_time_west_coast.csv
./data/bank-additional.csv
./data/bikeshare.csv
./data/citibike_feb2014.csv
./data/drinks.csv
./data/drones.csv
./data/hitters.csv
./data/icecream.csv
./data/imdb_1000.csv
./data/mtcars.csv
./data/NBA_players_2015.csv
./data/ozone.csv
./data/pronto_cycle_share/2015_station_data.csv
./data/pronto_cycle_share/2015_trip_data.csv
./data/pronto_cycle_share/2015_weather_data.csv
./data/rossmann.csv
./data/rt_critics.csv
./data/stores.csv
./data/syria.csv
./data/time_series_train.csv
./data/titanic.csv
./data/ufo.csv
./data/vehicles_test.csv
./data/vehicles_train.csv
./data/yelp.csv
 I found all of the tsv files by running $ find . -name .tsv
./data/chipotle.tsv
./data/sms.tsv
##7. 
Dictionary shows 170 times.
I first created a file with all of the occurences of dictionary in it by running $ grep -r -i dictionary.
I created a file with all of the occurences of dictionary by running grep -r -i dictionary . > dictionary_count.txt.
I then counted the number of times dictionary shows in that file dictionary_count.txt by running wc -l dictionary_count.txt.


