1. update game set co2_consumed = co2_consumed + 500, location = (select ident from airport where municipality = "Nottingham" and ident = "EGBN") where screen_name = "Vesa" and location = "EGCC"; select * from game;
   ![7 1](https://github.com/user-attachments/assets/5b34252b-48c7-41bf-87d9-3010bb5032fa)
