# database-checkpoint

**Challenge 1 - All of the vacation destinations.**

  * Query: vacations=# SELECT name  FROM destinations;
  * Result: ![](./result_images/Challenge1.PNG)

**Challenge 2 - All destinations where you can swim at the beach.**
  * Query: vacations=# SELECT name FROM destinations WHERE has_beaches='true';
  * Result: ![](./result_images/Challenge2.PNG)

**Challenge 3 - All destinations where the average temperature is over 60 degrees.**
  * Query: vacations=# SELECT name FROM destinations WHERE average_temp>60;
  * Result: ![](./result_images/Challenge3.PNG)

**Challenge 4 - All destinations where you can swim at the beach AND go to the mountains.**
  * Query: vacations=# SELECT name FROM destinations WHERE has_beaches ='true' AND has_mountains='true';
  * Result: ![](./result_images/Challenge4.PNG)

**Challenge 5 - All destinations where flights cost less than $500 and you can hike in the mountains.**
  * Query: vacations=# SELECT name FROM destinations WHERE cost_of_flight<500 AND has_mountains='true';
  * Result: ![](./result_images/Challenge5.PNG)

**Challenge 6 - Add an entry for The Bahamas, where the average temperature is 78, it has beaches but no mountains, and the flights cost $345.**
  * Query: vacations=# INSERT INTO destinations(name, average_temp, has_beaches, has_mountains, cost_of_flight) VALUES('The Bahamas', 78, true, false, 345);
  * Result: ![](./result_images/Challenge6.PNG)

**Challenge 7 - Turns out, the cost of flights to New Zealand has increased! Update New Zealand's entry for flight cost to $1000.**
  * Query: vacations=# UPDATE destinations SET cost_of_flight = 1000 WHERE name='New Zealand';
  * Result: ![](./result_images/Challenge7.PNG)

**Challenge 8 - Turns out, Minnesota isn't a vacation destination. Please delete it from the database.**
  * Query: vacations=# DELETE FROM destinations WHERE name='Minnesota';
  * Result: ![](./result_images/Challenge8.PNG)

**Challenge 9 - When the data set was written, the author mistakently wrote "England" when they actually meant "Scotland". Please update that entry in the database.**
  * Query: vacations=# UPDATE destinations SET name ='Scotland' WHERE name='England';
  * Result: ![](./result_images/Challenge9.PNG)