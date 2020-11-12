# Описание интерфейса IWorker

Интерфейс предназначен для работы с методами класса [Worker](https://github.com/Veselyaskin99/README/blob/main/Worker.md))
## Реализация интерфейса

- Add (Worker: [Worker](https://github.com/Veselyaskin99/README/blob/main/Worker.md)) — функция, добавляющая работника в базу данных. Параметр «Worker» — работник, которого необходимо добавить в БД;
- Del (Worker: [Worker](https://github.com/Veselyaskin99/README/blob/main/Worker.md)) — функция, удаляющая работника из программы. Параметр «Worker» — работник, которого необходимо удалить из программы;
- Edit (Worker: [Worker](https://github.com/Veselyaskin99/README/blob/main/Worker.md)) — функция, редактирующая данные о работнике. Параметр «Worker» — работник, которого необходимо редактировать в БД;
- FindByID< [Worker](https://github.com/Veselyaskin99/README/blob/main/Worker.md) >(ID : Integer) : Worker — функция, осуществляющая поиск работника в базе данных по ID и возвращающая найденного работника, если такой имеется. 
- GetID(Worker: [Worker](https://github.com/Veselyaskin99/README/blob/main/Worker.md)) : Integer — функция, возвращающая ID определенного работника. 
- GetMaxID< [Worker](https://github.com/Veselyaskin99/README/blob/main/Worker.md) >() : Integer — функция, возвращающая ID последнего работника в базе данных.
- Get Worker (sorting : String, ASKorDESK : string, filterA : Worker, filterB : Worker, count : int, page : int) : List < Worker > — функция, возвращающая список работников с заданными параметрами. Параметры: 
   - sortintg: String – отвечает, по какому полю будет сортироваться список:
   - ASKorDESK : string – отвечает, по возрастанию или убыванию будут сортироваться элементы;
   - filterA : Worker – отвечает за фильтрацию, включает в себя левую границу интервала значений фильтра;
   - filterB : Worker – отвечает за фильтрацию, включает в себя правую границу интервала значений фильтра; 
   - count : int – отвечает, сколько элементов необходимо показать;
   - page: int – отвечает, с какой страницы начинать поиск элементов.
