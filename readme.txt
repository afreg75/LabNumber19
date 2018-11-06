1. SELECT * FROM customers;
2. SELECT country FROM customers;
3. SELECT customerid FROM customers WHERE customerid RLIKE 'BL';
4. SELECT * FROM orders LIMIT 100;
5. SELECT * FROM customers  WHERE postalcode IN (1010, 3012, 12209, 05023);
6. SELECT * FROM orders WHERE shipregion IS NOT NULL;
7. SELECT * FROM customers ORDER BY country; SELECT * FROM customers ORDER BY city;   SELECT * FROM orders ORDER BY shipcountry;  SELECT * FROM orders ORDER BY shipcity; 
8. INSERT INTO customers (customerid, companyname, contactname, contacttitle, address, city, region, postalcode, country, phone, fax)
   values("darn","Adan" , "Adan fregoso", "Manager", "14500 Zona" , "Plymouth", "MI", "48175","USA", "245678987", "234567897");
9. 	UPDATE orders SET shipregion ='Eurozone' WHERE shipcountry='France';
10. DELETE FROM `order details` WHERE quantity = 1;
11. SELECT max(quantity), MIN(quantity), AVG(quantity) FROM `order details` `order details`;
12. SELECT max(quantity), MIN(quantity), AVG(quantity) FROM `order details` GROUP BY orderid;]
13. SELECT * FROM orders WHERE orderID =10290 
14. SELECT * FROM orders INNER JOIN customers ON orders.EmployeeID = EmployeeID;  SELECT * FROM orders left JOIN customers ON orders.EmployeeID = EmployeeID;
	SELECT * FROM orders Right JOIN customers ON orders.EmployeeID = EmployeeID;
15. SELECT * FROM northwind.employees WHERE reportsto is NULL;
16. SELECT FirstName FROM employees WHERE Reportsto = (SELECT EmployeeID From employees WHERE FirstName = "Andrew");

