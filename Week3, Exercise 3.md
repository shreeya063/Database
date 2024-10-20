1. select country.name as "country name", airport.name as "airport name" from country, airport where country.iso_country = airport.iso_country and country.name = "Iceland";
 ![1](https://github.com/user-attachments/assets/80866679-3139-4501-b1f7-7d8708e97046)

2. select airport.name as "airport name" from airport, country where airport.iso_country = country.iso_country and airport.type = "large_airport" and country.name = "France";
 ![2](https://github.com/user-attachments/assets/98498a3b-e0cb-4cc8-babc-7c94bbff41df)

3. select country.name as "country_name", airport.name as "airport_name" from country, airport where country.iso_country = airport.iso_country and country.continent = "AN";
![3](https://github.com/user-attachments/assets/ef26e7aa-c548-4a0e-9fec-fdee648ae245)

4. select airport.elevation_ft from airport, game where airport.ident = game.location and game.screen_name = "Heini";
 ![4](https://github.com/user-attachments/assets/2f3c0a7d-b235-4320-b52a-c9c33e628ba3)

5. select airport.elevation_ft*0.3048 as "elevation_m" from airport, game where airport.ident = game.location and game.screen_name = "Heini";
 ![5](https://github.com/user-attachments/assets/e46b4dbe-2318-4c26-95f0-25bf4b147dd3)

6. select airport.name as "name" from airport, game where airport.ident = game.location and game.screen_name = "Ilkka";
  ![6](https://github.com/user-attachments/assets/ca967414-e208-444d-a4f0-ea82f1a056d2)

7. select country.name as "name" from country, game, airport where country.iso_country = airport.iso_country and airport.ident = game.location and game.screen_name = "Ilkka";
 ![7](https://github.com/user-attachments/assets/fca447fe-eb30-4d62-ab25-f212b6d73f49)

8. select goal.name as "name" from goal, game, goal_reached where goal.id = goal_reached.goal_id and goal_reached.game_id = game.id and game.screen_name = "Heini";
 ![8](https://github.com/user-attachments/assets/40049548-43be-4057-90d9-971c5b4bacfd)

9. select airport.name as "name" from airport, game, goal, goal_reached where airport.ident = game.location and game.id = goal_reached.game_id and goal.id = goal_reached.goal_id and game.screen_name = "Ilkka" and goal.name = "clouds";
 ![9](https://github.com/user-attachments/assets/957a3565-3973-4226-bdfd-ed6b2a968af1)

10. select country.name as "name" from airport, country, game, goal, goal_reached where airport.ident = game.location and game.id = goal_reached.game_id and goal.id = goal_reached.goal_id and airport.iso_country = country.iso_country and game.screen_name = "Ilkka" and goal.name = "clouds";
  ![10](https://github.com/user-attachments/assets/98f90143-c014-41f2-9d52-29d49d1db2bf)
