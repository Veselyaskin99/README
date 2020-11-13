# Описание интерфейса ITS
Интерфейс предназначен для работы с методами класса [TS](https://github.com/Veselyaskin99/README/blob/main/TS.md)
## Реализация интерфейса
+ Add (TS: [TS](https://github.com/Veselyaskin99/README/blob/main/TS.md)) — функция, добавляющая т/с в базу данных. Параметр «TS» — т/с, которое необходимо добавить в БД;
+ Del (TS: [TS](https://github.com/Veselyaskin99/README/blob/main/TS.md)) — функция, удаляющая т/с из программы. Параметр «TS» — т/с, которое необходимо удалить из программы;
+ Edit (TS: [TS](https://github.com/Veselyaskin99/README/blob/main/TS.md)) — функция, редактирующая данные о т/с. Параметр «TS» — т/с, которое необходимо редактировать в БД;
+ FindByID< [TS](https://github.com/Veselyaskin99/README/blob/main/TS.md) >(ID : Integer) : TS — функция, осуществляющая поиск т/с в базе данных по ID и возвращающая найденное т/с, если такое имеется. 
+ GetID(TS: [TS](https://github.com/Veselyaskin99/README/blob/main/TS.md)) : Integer — функция, возвращающая ID определенного т/с. 
+ GetMaxID< [TS](https://github.com/Veselyaskin99/README/blob/main/TS.md) >() : Integer — функция, возвращающая ID последнего т/с в базе данных.
+ GetTS (sorting : String, ASKorDESK : string, filterA : TS, filterB : TS, count : int, page : int) : List < TS > — функция, возвращающая список т/с с заданными параметрами. Параметры: 
   - sortintg: String– отвечает, по какому полю будет сортироваться список:
   - ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
   - filterA : TS – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
   - filterB : TS – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
   - count : int – отвечает, сколько элементов необходимо показать;
   - page: int – отвечает, с какой страницы начинать поиск элементов.
