1. select country.name from country where country.iso_country in (select airport.iso_country from airport where airport.name like "Satsuma%");
   ![1](https://github.com/user-attachments/assets/713b0523-617b-45f7-9eee-f1e7676077af)

2. select name from airport where airport.iso_country in (select country.iso_country from country where name = "Monaco");
   ![2](https://github.com/user-attachments/assets/4c1c974f-9212-4f8b-8b75-1b9d7048f618)

3. select screen_name from game where game.id in (select game_id from goal_reached where goal_id in ( select id from goal where name = "Clouds"));
  ![3](https://github.com/user-attachments/assets/6bd7bafe-1e32-45e6-8127-9bc3337bcc0b)

4. select name from country where iso_country not in (select iso_country from airport);
  ![4](https://github.com/user-attachments/assets/cc278945-599e-4d6f-a255-4411e9f38d24)

5. select name from goal where id not in (select goal_id from goal_reached where game_id in ( select id from game where screen_name = "Heini")); 
  ![5](https://github.com/user-attachments/assets/0738c9fe-c18c-495b-bb7b-fa7aa5026259)


