select max(elevation_ft) from airport;
![1](https://github.com/user-attachments/assets/6c1cde45-51ce-45fb-99af-c4ac4e91c7ef)

select continent, count(*) from country group by continent;
![2](https://github.com/user-attachments/assets/f929d891-4557-44d1-b842-c389fd33ad95)

select screen_name, count(*) from game left join goal_reached on id = game_id group by screen_name;
![3](https://github.com/user-attachments/assets/8c63f060-732d-41de-aa68-5107d589d610)

select screen_name from game where co2_consumed = (select min(co2_consumed) from game);
![4](https://github.com/user-attachments/assets/32e6e75a-7f36-4bd2-838b-44c0cbf169ac)

select country.name, count(airport.id) as "count(*)" from country left join airport on country.iso_country = airport.iso_country group by country.name order by count(airport.id) desc limit 50;
![5](https://github.com/user-attachments/assets/b4cf57f9-0749-4130-9687-bf16443ac00f)

select country.name from country left join airport on country.iso_country = airport.iso_country group by country.name having count(airport.id) > 1000;
![6](https://github.com/user-attachments/assets/fda0b5ce-ad6c-4297-a987-f88656d345d1)

select name from airport where elevaton_ft in (select max(elevation_ft) from airport); 
![7](https://github.com/user-attachments/assets/75d5420a-ba17-4f54-85bb-48fe34e0d202)

select country.name from country join airport on country.iso_country = airport.iso_country where elevation_ft in (select max(elevation_ft) from airport);
![8](https://github.com/user-attachments/assets/a3a65a63-0aeb-49ee-ad66-0e3526fab1a5)

select count(goal_id) as "count(*)" from goal_reached join game on goal_reached.game_id = game.id where screen_name = "Vesa";
![9](https://github.com/user-attachments/assets/720706c0-c6cc-4fea-96a1-230980d7ed42)

select name from airport where latitude_deg in(select min(latitude_deg) from airport);
![10](https://github.com/user-attachments/assets/5df01d3d-9fa1-4a22-86af-a3c2634640fb)
