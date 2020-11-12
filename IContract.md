# Описание интерфейса IOrder
Интерфейс предназначен для работы с методами класса [Contract](https://github.com/Veselyaskin99/README/blob/main/Contract.md)

## Реализация интерфейса
+ Add (Contract: [Contract](https://github.com/Veselyaskin99/README/blob/main/Contract.md)) — функция, добавляющая контракт в базу данных. Параметр «Contract» — контракт, который необходимо добавить в БД;
+ Del (Contract: [Contract](https://github.com/Veselyaskin99/README/blob/main/Contract.md)) — функция, удаляющая контракт из программы. Параметр «Contract» — контракт, который необходимо удалить из программы;
+ Edit (Contract: [Contract](https://github.com/Veselyaskin99/README/blob/main/Contract.md)) — функция, редактирующая данные о контракте. Параметр «Contract» — контракт, который необходимо редактировать в БД;
+ FindByID< [Contract](https://github.com/Veselyaskin99/README/blob/main/Contract.md) >(ID : Integer) : Contract — функция, осуществляющая поиск контракта в базе данных по ID и возвращающая найденный Contract, если такой имеется. 
+ GetID(Contract: [Contract](https://github.com/Veselyaskin99/README/blob/main/Contract.md)) : Integer — функция, возвращающая ID определенного контракт. 
+ GetMaxID< [Contract](https://github.com/Veselyaskin99/README/blob/main/Contract.md) >() : Integer — функция, возвращающая ID последнего контракта в базе данных.
+ GetContract (sorting : String, ASKorDESK : string, filterA : Contract, filterB : Contract, count : int, page : int) : List < Contract > — функция, возвращающая список заказов с заданными параметрами. Параметры: 
   - sortintg: String– отвечает, по какому полю будет сортироваться список:
   - ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
   - filterA : Contract – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
   - filterB : Contract – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
   - count : int – отвечает, сколько элементов необходимо показать;
   - page: int – отвечает, с какой страницы начинать поиск элементов.
