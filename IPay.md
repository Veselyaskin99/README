# Описание интерфейса IPay
Интерфейс предназначен для работы с методами класса [Pay](https://github.com/Veselyaskin99/README/blob/main/Pay.md)
## Реализация интерфейса
+ Add (Pay: [Pay](https://github.com/Veselyaskin99/README/blob/main/Pay.md)) — функция, добавляющая оплаты в базу данных. Параметр «Pay» — оплата, которую необходимо добавить в БД;
+ GetPay (sorting : String, ASKorDESK : string, filterA : Pay, filterB : Pay, count : int, page : int) : List < [Pay](https://github.com/Veselyaskin99/README/blob/main/Pay.md) > — функция, возвращающая список платежей с заданными параметрами. Параметры: 
   - sortintg: String– отвечает, по какому полю будет сортироваться список:
   - ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
   - filterA : Pay – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
   - filterB : Pay – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
   - count : int – отвечает, сколько элементов необходимо показать;
   - page: int – отвечает, с какой страницы начинать поиск элементов.



