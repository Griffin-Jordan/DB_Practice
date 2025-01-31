# DB_Practice
This is an exercise to learn about building a DB and creating tables with Primary and foreign keys. The DB created is one that I made up for an imaginary toy company. This was meant to learn new skills for creating a Database and learning how it works as well as using it to practice some tableau techniques with the new DB. The database is called Myshop and is composed of 4 tables.



A description of the tables is as follows:


<br />

**client**:

  clientID(String): Primary key and the ID for each client in the DB.
  
  Company(String): The name fo the client.
  
  City(String): The city where the client company is located.
  
  Address(String): The address to the company where the products will shipped.


  <br />

**employee**:

  employeeID(String): Primary key and the our shops employee's ID. Note that these employees are all salesman.
  
  FirstName(String): Employees first name.
  
  LastName(String): Employees last name.
  
  Age(INT): Employees age.


  <br />

**wharehouse**:

  productID(String): Primary key and our products ID we use to identify what was sold to the clients.
  
  product_name(String): the name of the toy.
  
  price(float): the price of the toy.


  <br />

**orders**:

  orderID(String): Primary key and is the ID for an order put in for a client who is buying toys.
  
  units(INT): the quantity of the toy that the client wants.
  
  clientID(String): Foreign key from **client** using clientID and it is the ID of the client that is ordering toys.
  
  productID(String): Foreign key from **wharehouse** using productID and it is the ID of the product that the client is ordering.
  
  SellerID(String): Foreign key from **employee** using employeeID and it is the name of the employee that made the sale.

  Date(date): This is the date that the order was made.
  
  
  


<img width="424" alt="Screenshot 2025-01-31 at 9 06 40 AM" src="https://github.com/user-attachments/assets/6f3bf70b-6d51-4aea-a11a-3ac3909b1e35" />


The image above shows the ER Diagram of the tbales which are connected through foreign keys by each table to show the relationship of the tabes.
