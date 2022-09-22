## SQL ASSIGNMENT

SELECT *
FROM Person.Person
WHERE FirstName LIKE '%d' AND (LastName LIKE '%r' OR LastName LIKE '%m')

![3rd-1st](https://user-images.githubusercontent.com/69041949/191631755-50d44fc7-ab1d-46cb-9a84-8ba20da12969.jpg)


SELECT TOP 10 *
FROM Purchasing.PurchaseOrderDetail
WHERE YEAR(DueDate) > 2011 AND OrderQty > 4
ORDER BY OrderQty

![3rd-2nd](https://user-images.githubusercontent.com/69041949/191631864-f8a1e4ab-faee-46cc-8854-296f4d653261.jpg)


SELECT OrderQty, ReceivedQty, UnitPrice, OrderQty -ReceivedQty AS UndeliveredQty, (OrderQty - ReceivedQty) * UnitPrice AS RefundAmount
FROM Purchasing.PurchaseOrderDetail
WHERE OrderQty > ReceivedQty

![3rd-3rd](https://user-images.githubusercontent.com/69041949/191631958-fc232bab-623e-4085-b223-f6ebed931ced.jpg)


SELECT BusinessEntityID
FROM Person.Person
EXCEPT
SELECT BusinessEntityID
FROM Person.PersonPhone

![3rd-4th](https://user-images.githubusercontent.com/69041949/191632046-fb618024-b6d4-48cc-bb00-ef54728279d8.jpg)



SELECT BusinessEntityID
FROM Person.Person
INTERSECT
SELECT BusinessEntityID
FROM Person.PersonPhone

![3rd-5th](https://user-images.githubusercontent.com/69041949/191632115-4da0d40e-b1e4-4f64-b1bb-b8bb897b7529.jpg)
