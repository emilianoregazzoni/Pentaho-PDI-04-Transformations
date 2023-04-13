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
I need to specify the route of the excel, in this case I will load the Accounting plan information.

![image](https://user-images.githubusercontent.com/20979227/230802419-56fc3629-077c-4020-aca6-a8bad7b87a7c.png)

Load the excel page:

![image](https://user-images.githubusercontent.com/20979227/230802508-21455c1d-254a-4b1f-bf73-298960d5ae5f.png)

After that I should specify that the file contains the headers, so I check "Header"

![image](https://user-images.githubusercontent.com/20979227/230802563-4d5a1bb0-3e6f-4a07-9ced-e9f02833e970.png)

Then if I search on "Fields" sheet I can see the headers of the file:

![image](https://user-images.githubusercontent.com/20979227/230802578-0cdcfebd-00e9-4fba-9ff5-e60c13dbf097.png)

And then if I click on "Preview rows" button I see the information from the excel:

![image](https://user-images.githubusercontent.com/20979227/230802617-32ba4cb2-f699-43ee-b0cb-3690b16b5ff2.png)

The information:

![image](https://user-images.githubusercontent.com/20979227/230802692-d1027053-c848-4faf-a33d-0302a8b94bf7.png)

Once I finished I need to create an incremental ID for the each item in the "Plan de cuentas", for do this, I will need to add a component Secuence.

![image](https://user-images.githubusercontent.com/20979227/231904660-4c51a141-4f38-46ed-81c5-91f89b8b5009.png)

I indicate that it stats with 1 and increment by 1.

After run I have the items with their corresponding Id.

![image](https://user-images.githubusercontent.com/20979227/231904738-a1eebcc2-20c3-4928-b45e-3c5bf516fa6f.png)




