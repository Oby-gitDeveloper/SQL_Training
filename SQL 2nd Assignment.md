## SQL QUERIES

SELECT ProductID, Name FROM Production.Product
WHERE Name like 'Chain%'
-- 5 rows are returned

![2nd Assignment_1st_Query](https://user-images.githubusercontent.com/69041949/190236838-c9e276fc-1db5-4ca6-be4b-12f1d3633f7f.jpg)


SELECT BusinessEntityID, FirstName, MiddleName, LastName FROM Person.Person
WHERE MiddleName LIKE 'E%' OR MiddleName LIKE 'B%' 
-- 1110 rows are returned

![2nd Assignment_2nd_Query](https://user-images.githubusercontent.com/69041949/190237360-3d36f7fb-5a52-4729-a7b8-8d09c2c2319d.jpg)


SELECT OrderDate FROM Sales.SalesOrderHeader
WHERE OrderDate BETWEEN '2011-09-01' AND '2011-09-30'
-- 157 rows are returned

![2nd Assignment_3rd_Query](https://user-images.githubusercontent.com/69041949/190240032-22793b8c-c0b3-42d4-9254-45c9b6717030.jpg)

SELECT SalesOrderID, OrderDate, TotalDue FROM Sales.SalesOrderHeader
WHERE OrderDate BETWEEN '2011-09-01' AND '2011-09-30' AND TotalDue >1000
-- 138 rows are returned

![2nd Assignment_4th_Query](https://user-images.githubusercontent.com/69041949/190240870-41a41f86-f680-424e-a7a3-758082ed8d9c.jpg)


SELECT SalesOrderID, OrderDate, TotalDue FROM Sales.SalesOrderHeader
WHERE OrderDate BETWEEN '2011-09-01' AND '2011-09-30' AND TotalDue >1000
-- 9 rows are returned

![2nd Assignment_5th_Query](https://user-images.githubusercontent.com/69041949/190241701-3c82371a-670d-4d5a-b5b8-af11ac6a07df.jpg)
