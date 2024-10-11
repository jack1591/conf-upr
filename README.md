# Репозиторий с заданиями по конфигурационному управлению
## Загрузка репозитория на компьютер
1. Откройте терминал
2. Перейдите в папку, где вы хотите разместить проект
3. Выполните команду:
```
git clone https://github.com/jack1591/conf-upr.git
```
## Запуск программы
1. Перейти в папку build в терминале
2. Ввести следующие команды:  
При первом запуске программы:
```
cmake -G "MinGW Makefiles" ..
cmake ..
mingw32-make
```  
Запуск .exe файла:
```
./my_shell.exe
```

## Задание 1
Разработать эмулятор для языка оболочки ОС. Необходимо сделать работу
эмулятора как можно более похожей на сеанс shell в UNIX-подобной ОС.
Эмулятор должен запускаться из реальной командной строки, а файл с
виртуальной файловой системой не нужно распаковывать у пользователя.
Эмулятор принимает образ виртуальной файловой системы в виде файла формата
**tar**. Эмулятор должен работать в режиме **CLI**.
Конфигурационный файл имеет формат **toml** и содержит:  
• Имя компьютера для показа в приглашении к вводу.  
• Путь к архиву виртуальной файловой системы.  
  
Необходимо поддержать в эмуляторе команды **ls**, **cd** и **exit**, а также
следующие команды:
```
1. uniq.
2. whoami.  
3. find.
``` 
Все функции эмулятора должны быть покрыты тестами, а для каждой из
поддерживаемых команд необходимо написать 2 теста.
