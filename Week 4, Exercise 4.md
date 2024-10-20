1. select country.name as "country name", airport.name as "airport name" from country inner join airport on country.iso_country = airport.iso_country where airport.iso_country = "FI" and scheduled_service = "yes";
![1](https://github.com/user-attachments/assets/4408f5a5-cc1e-4306-bf51-d936630cf462)
2. select screen_name, name from airport inner join game on airport.ident = game.location;
![2](https://github.com/user-attachments/assets/3f943bd2-04b3-44f2-a946-af1d3c7bc420)
3. select screen_name, coountry.name as "name" from game inner join airport on airport.ident = game.location inner join country on country.iso_country = airport.iso_country;
![3](https://github.com/user-attachments/assets/581c8fdc-1ba7-4c23-aadf-7b88908c7ff5)
4. select name, screen_name from airport left join game on airport.ident = game.location where airport.name like "%Hels%";
![4](https://github.com/user-attachments/assets/e0eb4332-1b82-46c2-b3c5-6793e8cfa970)
5.select name, screen_name from goal left join goal_reached on goal.id = goal_reached.goal_id left join game on game.id = goal_reached.game_id;
![5](https://github.com/user-attachments/assets/33839743-06fc-4f59-a917-62cb5e43fbcf)

