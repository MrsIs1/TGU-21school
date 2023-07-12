# Задание №6. Создание SQL-запросов
## Categories

Выбрать всё, посчитать длину колонки CategoryName из Categories
![Categories](../misc/images/categories_1.png)

Выбрать 3 колонки из Categories и отфильтровать по CategoryName = Seafood
![Categories](../misc/images/categories_2.png)

Выбрать все, если в строке Description ',' встречается более 0 раз или если слово 'and' встречается более 0 раз, то вернуть Yes, иначе No, из Categories.

Так же отфильтровать по Description не является пустым либо пустой строкой.

Отсортировать по CategoryName по возрастанию.
![Categories](../misc/images/categories_3.png)
___
## Customers

Выбрать всё, посчитать длину колонки CustomerName из Customers. Отфильтровать по Country = Mexico.
![Customers](../misc/images/customers_1.png)

Выбрать все поля из Customers, где City равен London
![Customers](../misc/images/customers_2.png)

Посчитать сколько раз повторяется значение City в таблице Customers, выбрать города которые повторяются 2 или более раз. Отсортировать по убыванию.
![Customers](../misc/images/customers_3.png)
___
## Employees

Выбрать всё, посчитать длину FirstName, посчитать длину LastName, отсортировать BirthDate по убыванию.
![Customers](../misc/images/employees_1.png)

Выбрать все из Employees, исключить записи где FirstName равен Margaret. Отсортировать по возрастанию длины колонки Notes.
![Customers](../misc/images/employees_2.png)

Выбрать все, ищем значение точки в колонке Photo и добавляем 1 для того что-бы начать с последующего символа, передаем колонку в Photo и это значение в функцию Mid. 

Так же ищем есть ли слово French в колонке Notes и возвращаем Yes если оно есть либо No если его нет.

Отфильтровать BirthDate между 1960 и 1970 годами. Отсортировать по возрастанию FirstName.

![Customers](../misc/images/employees_3.png)
___
## OrderDetails
1. Выбирает все записи  из таблицы OrderDetails, где  данные строк из столбца Quantity имеют значения   от 10 до 15, и  сортирует по возрастанию по  столбцу ProductID

![OrderDetails](../misc/images/exercise6.OrderDetails.png)

2. Выбирает все записи  из таблицы OrderDetails, где  данные строк из столбца ProductID имеют значения  равные 1 и 77, и сортирует по возрастанию по  столбцу OrderDetailID

![OrderDetails](../misc/images/exercise6._OrderDetails_2.png)

3. Выбирает все записи  из таблицы OrderDetails, где  данные строк из столбца Quantity имеют значения   не равные 40, и лимит- первые 10 записей

![OrderDetails](../misc/images/exercise6._OrderDetails_3.png)

## Orders
1. Выбирает все записи  из таблицы Orders, где  данные строк из столбца CustomerID имеют значения   от 10 до 15, и данные строк из столбца EmployeeID имеют значения   от 1 до 5 и  сортирует по возрастанию по  столбцу OrderID

![Orders](../misc/images/exercise6.orders1.png)

2. Выбирает все записи  из таблицы Orders, где  данные строк из столбца CustomerID имеют значения   равны 80 и 20, и лимит 10 записей, начиная с 2

![Orders](../misc/images/exercise6._Orders_2.png)

3. Выбирает все записи  из таблицы Orders, где  данные строк из столбца CustomerID имеют значения  которые начинаются с 3, и данные строк из столбца OrderID имеют значения  которые заканчиваются - 3

![Orders](../misc/images/exercise6._Orders_3.png)

## Products
1.	Выбирает ВСЕ записи из таблицы Products, в которых SupplierID столбец имеет значение 24 , а столбец CategoryID имеет значение 5.

![Products](../misc/images/exercise6.Products_1.png)

2.	Выбирает ВСЕ записи из таблицы Products и сортирует их по столбцу CategoryID в порядке возрастания, лимит первые 5 записей.

![Products](../misc/images/exercise6.Products_2.png)

3.	Выбирает все записи из таблицы Products, где значение поля ProductName  начинается с Ge.

![Products](../misc/images/exercise6.Products_3.png)

## Shippers
1.	Выбирает ВСЕ записи из таблицы Shippers, в которых ShipperName столбец имеет значение Speedy Express' и 'Federal Shipping'

![Shippers](../misc/images/exercise6.Shippers_1.png)

2.	Выбирает ВСЕ записи из таблицы Shippers и сортирует их по столбцу ShipperID в ОБРАТНОМ порядке.

![Shippers](../misc/images/exercise6.Shippers_2.png)

3.	Выбирает все записи из таблицы Shippers, где Phone заканчивается на 1 и упорядочивает записи в порядке возрастания значений столбца ShipperID.

![Shippers](../misc/images/exercise6.Shippers_3.png)

## Suppliers
1.	Выбирает ВСЕ записи из таблицы Suppliers, в которых City столбец начинается c s и не имеет значения Salerno

![Suppliers](../misc/images/exercise6.Suppliers_1.png)

2.	Выбирает ВСЕ записи из таблицы Suppliers, и сортирует их в обратном порядке  по столбцу SupplierID, лимит первые 5 записей

![Suppliers](../misc/images/exercise6.Suppliers_2.png)

3.	Выбирает ВСЕ записи из таблицы Suppliers, в которых столбец ContactName заканчивается на е и сортируется в обратном порядке по столбцу SupplierID

![Suppliers](../misc/images/exercise6.Suppliers_3.png)
