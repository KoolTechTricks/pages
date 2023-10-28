# Интерфейс командной строки
> guides

**Интерфейс командной строки** *(англ. Command line interface, CLI)* — способ
взаимодействия с программой посредством отправки текстовых команд в консоль
(терминал).

!noimage

## Применение

Некоторые программы (зачастую полезные инструменты и утилиты) не имеют
графического интерфейса. Чтобы ими воспользоваться, необходимо открыть консоль
и ввести команды. Обычно их используют как основу (библиотеку) для других
программ, или создают графический интерфейс. Например, можно написать скрипт,
использующий определённую программу с заданными параметрами.

Привычные программы с графическим интерфейсом могут иметь дополнительный
консольный интерфейс. Обычно, это параметры запуска, которые изменяют поведение
программы. Запуск программы через консоль даёт возможность просматривать логи в
реальном времени, что может быть полезно для обнаружения ошибок и исправления
проблем.

## Использование

### Эмулятор терминала

Эмулятор терминала выступает в качестве интерфейса для взаимодействия с
терминалом.

В Windows можно использовать стандартную программу `cmd`, но в современных
версиях рекомендуется [Windows
Terminal](https://apps.microsoft.com/detail/windows-terminal/9N0DX20HK701).

В Linux эмулятор терминала обычно предустановлен вместе со средой рабочего
стола. Для Gnome это GNOME Terminal, для KDE — Konsole.

В Android можно использовать [Termux](https://termux.dev).

### Оболочка

Оболочка *(Shell)* интерпретирует введённые команды. Они используют собственные
языки программирования, на которых можно писать скрипты. Также они позволяют
использовать какие-либо функции, сокращения, операторы.

В Windows по умолчанию используется оболочка cmd.exe, но ещё имеется
PowerShell.

В UNIX-подобных системах стандартом является bash, но есть возможность
использовать другие оболочки, например zsh, fish.

### Запуск программ

Для запуска любой программы необходимо указать путь к ней. Возможно,
потребуется указать его в кавычках, чтобы не было проблем со спецсимволами
(пробел). Это может быть как полный путь с началом в корневой директории, так и
относительный — с началом в текущей директории.

Перемещаться по директориям можно при помощи команды `cd` *(change directory —
изменить директорию)*, или можно сразу открыть терминал в папке, написав `cmd`
в строке пути проводника в Windows.

![Использование программы через полный путь и
относительный.](/media/cli_usage.jpg)

### Параметры

После исполняемого файла можно указывать параметры. Они обычно разделяются
через пробел и начинаются с дефиса. Чтобы узнать, какие есть параметры, нужно
написать `--help` или `-h`. С большей вероятностью будет выведена помощь, но
если её нет, то придётся обращаться к документации и интернету.

![Использование параметров для отображения версии и
помощи](/media/cli_options.jpg)

В Linux есть программа `man` *(manual — руководство)*. Если указать после неё
какую-либо программу, то, при наличии, отобразится подробная информация в
удобном виде.

### Переменные среды

Переменные среды *(Environment variables)* изменяют поведение программ
аналогично параметрам. Отличие в том, что их нужно указывать перед программой
в начале в формате `название=значение`. Обычно, названия именуются прописными
буквами, так как зачастую это константы, которые не должны изменяться во время
работы программы.

Переменные среды можно установить на уровне текущей сессии терминала или всей
системы, чтобы указанные настройки применялись для будущих вызовов программ.

### Path

Чтобы постоянно не указывать путь к нужной программе, существует переменная
`PATH`, которая содержит список директорий. Если вы пишете название программы,
то оболочка проходится по всем директориям в списке, чтобы найти исполняемый
файл с введённым названием.

Вы можете добавить свою директорию в переменную Path, чтобы запускать свои
программы из любого места.

#### Windows

1. Найдите в поиске "Изменение системных переменных среды" (или можно сразу
"Изменение переменных среды текущего пользователя" для пропуска 2-го пункта и
прав администратора). Также можно нажать `Win`+`R` и ввести
`SystemPropertiesAdvanced.exe`.
2. В открывшемся окне нажмите "Переменные среды".
3. Сверху появятся переменные для пользователя, а снизу — для системы. Можно
проделать операцию для текущего пользователя.
4. Нажмите два раза по переменной Path и добавьте путь к нужной папке.
5. Сохраните изменения и перезапустите окна командной строки. Также может
понадобиться перезайти в сессию.

![Добавление директории в переменную среды Path в
Windows.](/media/cli_path_windows.png)

#### Linux

Переменную PATH можно вывести командой `echo $PATH`. Чтобы добавить туда
какую-либо директорию, нужно написать `export PATH=/путь/к/папке:$PATH`.
Команда `export` устанавливает значение переменной, `PATH` — название
переменной, `/путь/к/папке` — директория, `$PATH` — значение переменной до
изменения.

Это изменение будет активно только в текущей сессии терминала. Чтобы сделать
его постоянным, необходимо добавить эту команду в конец файла конфигурации
оболочки (`~/.bashrc` для bash). Переменная `$HOME` содержит путь к домашней
директории текущего пользователя, можно писать её вместо `/home/user`.

![Добавление директории в переменную среды Path в
Linux.](/media/cli_path_linux.png)