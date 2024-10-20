Exercise 2
3. SELECT name
   FROM airport
   WHERE iso_country = "FI" 
   ORDER BY name;
![E2-3](https://github.com/user-attachments/assets/9b5ec4a7-5f10-4384-80d1-f92fac5465b9)

4. SELECT name, type
  FROM airport
    WHERE iso_country = 'FI'
ORDER BY type, name;
 ![E2-4](https://github.com/user-attachments/assets/8da2f5f9-4ee8-45b6-8e7d-ea5d279e403c)

5. SELECT name
  FROM country
  WHERE name like 'F%';
![E2-5](https://github.com/user-attachments/assets/362c9906-d526-4952-825f-df82b8f2d3fe)

6. SELECT name
   FROM country
  WHERE name like "%f%";
 ![E2-6](https://github.com/user-attachments/assets/576d0201-92b1-4bf4-9fe8-0f3887a19e65)

7. select location
   FROM game 
   WHERE screen_name= 'Vesa';
![E2-7](https://github.com/user-attachments/assets/92667185-cf96-428b-b5ff-4c093d2b35e3)

Exercise 3
1. SELECT country.name as"country name", airport.name as"airport name"
  FROM airport, country
  WHERE airport.iso_country = country.iso_country and country.name = "Iceland";
![E3-1](https://github.com/user-attachments/assets/d1cd8d1f-c553-47eb-8e4e-82257a17a52f)

3. SELECT country.name as country_name, airport.name as airport_name
  FROM airport, country
  WHERE airport.iso_country=country.iso_country and country.continent = "AN";
![E3-3](https://github.com/user-attachments/assets/617d516e-b8b2-494e-8e7e-d2d0b79109d8)

8. SELECT name
   FROM goal, goal_reached, game
   WHERE game.id = game_id and goal.id = goal_id and screen_name = "Heini";
![E3-8](https://github.com/user-attachments/assets/38f4fe03-22f2-4151-876f-628ef3516883)
