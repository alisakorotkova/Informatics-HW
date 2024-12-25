## Разминка (не нужно вставлять в отчет) - Поиск слова в файле

1. Создайте новый файл
```
touch mytext.txt
```

2. Откройте файл в текстовом редакторе (например, `nano mytext.txt`) и вставьте в него следующий текст:
   
```
This is a sample text file.
It contains some words.
Let's try to find the word 'text' in this file.
The word file is present here as well.
We are learning how to use grep command.
```
Сохраните файл и закройте редактор.

3. Выполнение поиска с помощью комманды. В терминале введите команду:
```
grep "text" mytext.txt
```

Команда должна вывести строки, содержащие слово “text”:
```
This is a sample text file.
Let's try to find the word 'text' in this file.
```


## Задание - Поиск с использованием опций и регулярных выражений
 
Для выполнения данного задания необходимо ознакомиться с различными доступными опциями для команды `grep` и изучить использование регулярных выражений.

1. Создайте новый текстовый файл с именем `data.txt` и вставьте в него следующий текст:
```
user1:password123:John Doe:john.doe@example.com:123-456-7890
user2:secretPass:Jane Smith:jane.smith@example.org:987-654-3210
admin:admin123:Administrator:admin@localhost:555-555-5555
guest:welcome:Guest User:guest@example.net:111-222-3333
user3:mySecurePassword:Bob Williams:bob.w@example.com:444-444-4444
user4:pass1234:Alice Brown:alice.b@example.com:555-666-7777
john.doe@example.com was seen online
bob.w@example.com logged in
jane.smith@example.org - registered
```
 - **Поиск пользователей:**
Используя grep, выведите все строки из data.txt, которые представляют собой записи пользователей (т.е. начинаются с user). И посчитайте их

- **Поиск электронной почты:**
Используя grep и регулярные выражения, найдите и выведите все электронные адреса из data.txt.

- **Поиск номеров телефонов:**
Используя grep и регулярные выражения, найдите и выведите все номера телефонов из data.txt в формате XXX-XXX-XXXX.

- **Фильтрация пользователей:**
Используя grep с опциями -v и -i, выведите все строки из data.txt, которые не содержат слово “admin” (без учета регистра).

- **Комбинирование с cut:**
Используя grep и cut, выведите только имена пользователей (третье поле) из записей пользователей в data.txt. Разделителем в data.txt является :.

- **Сложный шаблон:**
Используя grep и регулярные выражения, найдите и выведите все строки из data.txt, которые начинаются с “user” и заканчиваются на цифру.

## Материалы для решения лабораторной работы
**Теория по grep**
- https://www.gnu.org/software/grep/manual/grep.html
- https://www.opennet.ru/man.shtml?topic=grep&category=1
- https://selectel.ru/blog/tutorials/grep-command-in-linux/

**Теория по регулярным выражениям**
- https://habr.com/ru/articles/349860/
