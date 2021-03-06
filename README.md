


## World Kitchen
---

<!-- TOC -->
- [World Kitchen](#world-kitchen)
   - [Team Members](#team-members)
   - [Description of Application](#description-of-application)
   - [The Schema For the Database (The Table Definitions)](#the-schema-for-the-database-the-table-definitions)
   - [Explanation of Where the App is doing create, read, update, and delete](#explanation-of-where-the-app-is-doing-create-read-update-and-delete)
   - [Entity Relationship Diagram (ERD)](#entity-relationship-diagram-erd)
   - [Video Demonstration of the Application](#video-demonstration-of-the-application)




<!-- /TOC -->

---

### Team Members
---
- *Yuming Cui*
- *WenKai Fang*
- *Yunzhi Tang*



### Description of Application
---

> An easier way to figure out which dish you want best for the next meal

- The customer can see the menu of food from 5 different contries, also the picture and the comment about the dishes.
- The manager can login to the website, change the infomation of the dishes, add dishes and delete the dishes. 




### The Schema For the Database (The Table Definitions)
---

1. **China**
```sql
" CREATE TABLE `worldkitchen`.`China` (\rn\" +
" `id` NUMBER NOT NULL, \r\n" +
" `Menu` VARCHAR(35) NOT NULL, \r\n" +
" `Price` NUMBER NOT NULL, \r\n" +
" `Ingredients` VARCHAR (256) NOT NULL, \r\n" +
" `Sauce` VARCHAR (35) NOT NULL, \r\n"+ 
" `PRIMARY KEY (`id`) \r\n" )
```

2. **Italia**
```sql
" CREATE TABLE `worldkitchen`.`Italia` (\rn\" +
" `id` NUMBER NOT NULL, \r\n" +
" `Menu` VARCHAR(35) NOT NULL, \r\n" +
" `Price` NUMBER NOT NULL, \r\n" +
" `Ingredients` VARCHAR (256) NOT NULL, \r\n" +
" `Sauce` VARCHAR (35) NOT NULL, \r\n"+ 
" `PRIMARY KEY (`id`) \r\n" )
```

3. **Japan**
```sql
" CREATE TABLE `worldkitchen`.`Japan` (\rn\" +
" `id` NUMBER NOT NULL, \r\n" +
" `Menu` VARCHAR(35) NOT NULL, \r\n" +
" `Price` NUMBER NOT NULL, \r\n" +
" `Ingredients` VARCHAR (256) NOT NULL, \r\n" +
" `Sauce` VARCHAR (35) NOT NULL, \r\n"+ 
" `PRIMARY KEY (`id`) \r\n" )
```

4. **Thailand**
```sql
" CREATE TABLE `worldkitchen`.`Thailand` (\rn\" +
" `id` NUMBER NOT NULL, \r\n" +
" `Menu` VARCHAR(35) NOT NULL, \r\n" +
" `Price` NUMBER NOT NULL, \r\n" +
" `Ingredients` VARCHAR (256) NOT NULL, \r\n" +
" `Sauce` VARCHAR (35) NOT NULL, \r\n"+ 
" `PRIMARY KEY (`id`) \r\n" )
```

5. **Vietnam**
```sql
" CREATE TABLE `worldkitchen`.`Vietnam` (\rn\" +
" `id` NUMBER NOT NULL, \r\n" +
" `Menu` VARCHAR(35) NOT NULL, \r\n" +
" `Price` NUMBER NOT NULL, \r\n" +
" `Ingredients` VARCHAR (256) NOT NULL, \r\n" +
" `Sauce` VARCHAR (35) NOT NULL, \r\n"+ 
" `PRIMARY KEY (`id`) \r\n" )
```





### Explanation of Where the App is doing create, read, update, and delete
---

- **Create** 
   1. Create countries, for example "China", "Italia". 
   2. Create a new country, clicking on the `Create a new Cuisine Table` button, a new table will be created using create function. 
      
- **Read**
   1. Read `Menu`, `Price`, `Ingredients` by manager from one table.
   2. Read `Menu`, `Price`, `Ingredients` by customer from one table.
   3. Display all dishes from 5 countries by manager. 
   4. Display all dishes from 5 countries by customer.
   
- **Update**
   1. Create a new row in a table, this can only be done by manager.
   2. Change the price of a dish in a table, this can only be done by manager.
   
 - **Delete**
   1. Delete a country table.
   2. Delete a dish inside a country table.
   3. Delete a column, for example price, and ingredients inside a country table.
   
   
### Entity Relationship Diagram (ERD)


