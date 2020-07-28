CREATE TABLE Sales (Customer_Name VARCHAR2(30), Product_Name VARCHAR2(30), Amount NUMBER(3), Vendor_Name VARCHAR2(30))


INSERT ALL
INTO Sales (Customer_Name, Product_Name, Amount, Vendor_Name) VALUES ('Sharafali','Shoes',100.24,'Bata')
INTO Sales (Customer_Name, Product_Name, Amount, Vendor_Name) VALUES ('Aakash','Bags',203.45,'Bata')
INTO Sales (Customer_Name, Product_Name, Amount, Vendor_Name) VALUES ('Jobin','Perfumes',102.00,'Archies')
INTO Sales (Customer_Name, Product_Name, Amount, Vendor_Name) VALUES ('Divya','Books',119.00,'Archies')
INTO Sales (Customer_Name, Product_Name, Amount, Vendor_Name) VALUES ('Ganesh','Pens',302.00,'Archies')
SELECT * FROM DUAL;

SELECT * FROM Sales

SELECT row_number() over (order by Customer_Name) as Order_Number, 
Customer_Name, 
Product_Name, 
Amount, 
Vendor_Name 
FROM Sales


SELECT row_number() over (order by Vendor_Name) as Order_Number,
row_number() over (partition by Vendor_Name order by Customer_Name) as Vendor_Number,
Customer_Name, 
Product_Name, 
Amount, 
Vendor_Name 
FROM Sales

SELECT rank() over (partition by Vendor_Name order by Vendor_Name) as Vendor_Number, 
Customer_Name, 
Product_Name, 
Amount, 
Vendor_Name 
FROM Sales

