## FIRST SQL ASSIGNMENT

SELECT * FROM Purchasing.PurchaseOrderHeader 
--4,012 rows were returned showing 13 columns (plus serial number making it 14 cloumns)
![First SELECT Command](https://user-images.githubusercontent.com/69041949/188934728-4aadb96c-db1d-4bf6-b170-06206b6b3a70.jpg)


SELECT VendorID, OrderDate FROM Purchasing.PurchaseOrderHeader
--8,024 rows were returned showing only VendorID and OrderDate columns alone (the serial number were also shown to depict orderliness)
![Second SELECT Command](https://user-images.githubusercontent.com/69041949/188935109-333a0d34-9760-4fdb-b1dc-863eed7b7ea1.jpg)

SELECT * FROM Purchasing.PurchaseOrderHeader
WHERE Status=4
ORDER BY OrderDate DESC
--3,689 rows were filtered from Line 1 command, showing the entities with '4' as their status; the Order date were presented in descending order (with the most recent order at the top of the table)
![Third SELECT Command](https://user-images.githubusercontent.com/69041949/188935337-6b0d2acf-e2dd-4394-b05f-24ee4c822f6c.jpg)
