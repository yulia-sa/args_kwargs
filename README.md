# Задание 1:

Создать приложение телефонная книга. 
Класс Contact имеет следующие поля:
- имя, фамилия, телефонный номер - обязательные поля;
- избранный контакт - необязательное поле. По умолчанию False;
- дополнительная информация (email, список дополнительных номеров, ссылки на соцсети) — необходимо использовать *args, **kwargs.

Переопределить "магический" метод str для красивого вывода контакта. Вывод контакта должен быть следующим:

```#!bash

jhon = Contact('Jhon', 'Smith', '+71234567809', telegram='@jhony', email='jhony@smith.com')
print(jhon)
    
Вывод:

Имя: Jhon
Фамилия: Smith
Телефон: +71234567809
В избранных: нет
Дополнительная информация:
	 telegram : @jhony
	 email : jhony@smith.com
   
```

Класс PhoneBook:
- название телефонной книги - обязательное поле;
- телефонная книга должна работать с классами Contact.

Методы:

- вывод контактов из телефонной книги;
- добавление нового контакта;
- удаление контакта по номеру телефона;
- поиск всех избранных номеров;
- поиск контакта по имени и фамилии.

# Задание 2: 

Разработать свою реализацию функции print - adv_print. Она ничем не должна отличаться от классической функции кроме трех новых необязательных аргументов:

- start - с чего начинается вывод. По умолчанию пустая строка;
- max_line - максимальная длин строки при выводе. Если строка превыщает max_line, то вывод автоматически переносится на новую строку;
- in_file - аргумент, определяющий будет ли записан вывод ещё и в файл.
