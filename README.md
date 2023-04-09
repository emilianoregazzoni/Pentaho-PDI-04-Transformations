# Pentaho-PDI-04-Transformations
Pentaho PDI Trasnformations project is a small project about doing ETL works with Spoon.


First of all I have to understand the script provided by instructor. 
It's about an accouting system with people and vouchers related. The database works with 5 main tables:

![image](https://user-images.githubusercontent.com/20979227/230801509-480d83da-2c8f-4341-884d-5bc2480e7517.png)

It also has the relationships between the tables. The pk and fk are at the end of the script:

![image](https://user-images.githubusercontent.com/20979227/230801637-b00cc0fa-4861-4f23-b5bc-af4a04175bc1.png)

After review the script I should go to Postgres admin (PG admin), paste the code and run it. Now I can see the tables I'll be working on

![image](https://user-images.githubusercontent.com/20979227/230801956-f2c66527-e755-4928-b787-e9af0fa88bcb.png)

In my first step I want to load the information from excels files into the database previosuly created. For this, I need to create a first step to load an excel file that some transformations later will be in the database system.

![image](https://user-images.githubusercontent.com/20979227/230802312-7f4ece20-1d01-41a8-a0c9-64f6ccef31e8.png)

Double click to config the step:

![image](https://user-images.githubusercontent.com/20979227/230802419-56fc3629-077c-4020-aca6-a8bad7b87a7c.png)

