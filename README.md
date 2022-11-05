#LR6
Лабораторная работа №6

Цель лабораторной работы: изучение базовых возможностей системы управления версиями,опыт работы с Git Api, опыт работы с локальными и удаленным репозиторием.
## Ход работы:
#### 1. Создание репозитория
Создаем репозиторий в личном хранилище репозиториев через форк.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/1.jpg)
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/2.jpg)
#### 2. Настройка клиент git
В коносли Git Bash используем команды git config --global user.name и git config --global user.email для настройки клиента Git и вводим свои данные от GitHub.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/3.jpg)
#### 3. Клонирование удаленного репозитория на компьютер
Клонируем репозиторий, используя команду git clone и переходим в директорию.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/5.jpg)
#### 4. Добавление файла через интерфейс GitHub
Добавляем файл addFile через интерфейс GitHub. Переходим в директорию LR6 командой cd LR6 для дальнейшей работы с файлами.Подтягиваем изменения в локальный репозиторий командой git pull.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/6.jpg)
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/7.jpg)
#### 5. Получение всей истории операций
Получаем историю всех операций для каждой из веток.
#### 6. Получение последних изменений
Получаем историю последних двух операций для каждой из веток, используя команду git log.
Просмотрим существующие ветки в текущем репозитории командой git branch.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/8.jpg)

Перейдем в ветку branch1 командой git checkout branch1.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/10.jpg)
Посмотрим коммиты ветки branch1 с помощью команды git log.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/11.jpg)
Рассмотрим последние 3 коммита и внесенную ими разницу на уровне строк с помощью команды  git log -p -3.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/12.1.jpg)
Вернемся в ветку master.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/13.jpg)

Посмотрим состояние репозитория (отслеживаемые, изменённые, новые файлы и пр.) с помощью git status, добавим в индекс указанный файл командой git add mergefile.txt и проверим отслеживается ли файл.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/14.jpg)
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/15.jpg)
#### 7. Слияние в ветку master
Выполним слияние в ветку master. Оставляем коммит при помощи команды git commit -m "слияние веток".
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/16.jpg)
#### 8. Удаление побочной ветки
Удаляем побочную ветку после успешного слияния при помощи команды git branch -d branch1.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/17.jpg)
#### 9. Фиксирование изменений
Создадим изменения и комментарии для них. Создавать будем текстовые файлы прямо в терминале. Для создания текстовика используем команду echo ТЕкст для первого изменения > change1.txt, зафиксируем его git add change1.txt. Оставим комментарий git commit -m "изменене 1". Повторим все то же самое еще раз, только название указываем другое - change2.txt. 
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/19.jpg)
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/20.jpg)
Посмотрим комментарии.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/21.jpg)
#### 10. Откат коммита
Делаем откат коммита. Вводим git reset --HEAD~1.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/22.1.jpg)
#### 11. Создание ветки
Создаем ветку report для отчета и перейдем в нее, вводя команду git branch.
![](https://raw.githubusercontent.com/sushanura/LR6/master/screenshots/23.jpg)
#### 12. Отчет
Оформляю отчёт в VS Code с расширением Markdown Preview Enhanced файла README.md.

###Логи команд:
* git config --global user.name "В1441 SushkovaAS"
* git config --global user.email "nurasush2003@yandex.ru"
* git config --list
* git clone 
* cd LR6
_/Добавление файл addFile через интерфейс GitHub/_
* git pull
* git log
* git log -p -3
* git checkout branch1
* git log
* git checkout branch1
* git log
* git log -p -3
* git checkout master
* git status
* git add mergefile.txt
* git status
* git commit -m "слияние веток"
* git branch -d branch
* git branch

* echo Текст для первого изменения > change1.txt
* git add change1.txt
* git status
* git commit -m "изменение 1"
_/изменение в файле change1.txt/_

* echo Текст для второго изменения > change2.txt
* git add change2.txt
* git status
* git commit -m "изменение 2"
_/изменение в файле change2.txt/_

* git log -3
* git reset HEAD~1
* git branch
* git branch branch2
* git branch
* git pull

Вывод:
Я изучил базовые возможности системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием.