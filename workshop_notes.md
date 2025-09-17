Project_name : Gaming clube

Entites:
1. Member 
2. Recharge
3. Game
4. Transcation
5. Collection

Table_name :
1. members(id int primarykey autoincremrnt, name varchar not null, phone big int not null, balance float, joining_date date)
2. recharges(id int primarykey autoincremrnt, member_id foringekey, amount float, date date) ---> date is rechargerd date
3. games(id int primarykey autoincremrnt, name varchar unique, price int not null, discription varchar)

assingment: duration, status(active or inactive), minimum_player_count, maximum_player_count, player_count_multipe

4. transcations(id int primarykey autoincrement, memberid foringekey, gameid foringekey, amount int, date date)
5. collections(id int primarykey autoincrement, amount int, date date)

#cascading: if the date is deleted in one table the date reclated to this date shuold be deleted 