+++
title = 'Syncthing'
categories = ['files']
publishDate = 2023-10-07T18:33:37Z
lastmod = 2023-12-24T14:11:38Z
description = """Программа для синхронизации файлов между двумя и более \
устройствами в режиме реального времени."""
cover = '/media/syncthing.jpg'
featured = true
+++

# Syncthing
{{< categories >}}

[Syncthing](https://syncthing.net) — программа для синхронизации файлов между
двумя и более устройствами в режиме реального времени.

![Скриншот веб-интерфейса Syncthing](/media/syncthing.jpg)

## Применение

Syncthing позволяет синхронизировать различные файлы: фото, видео или документы.
Синхронизация происходит автоматически в режиме реального времени, так что любые
изменения практически сразу же появятся на связанных устройствах.

Можно сделать систему резервного копирования как на локальное устройство, так и
на сервер.

Это свободная программа с
[открытым исходным кодом](https://github.com/syncthing/syncthing), поэтому
возможно создать свою локальную экосистему, которую никто не сможет вам
ограничить, так как вы имеете полный контроль над ней.

## Установка

### ПК

Скачать программу для Windows, Linux, macOS можно на
[официальном сайте](https://syncthing.net/downloads) или
[GitHub](https://github.com/syncthing/syncthing/releases). После установки она
работает в фоне, а веб-интерфейс доступен по адресу `http://localhost:8384/`.

Если вы хотите индикатор в трее и отдельный графический интерфейс, то
понадобятся сторонние программы:

- [SyncTrayzor](https://github.com/canton7/SyncTrayzor/releases) для Windows
- [Syncthing Tray](https://github.com/Martchus/syncthingtray/releases) для Linux
- [Syncthing](https://github.com/syncthing/syncthing-macos/releases) для macOS

### Мобильное устройство

Приложение для Android вы можете скачать из
[Google Play](https://play.google.com/store/apps/details?id=com.nutomic.syncthingandroid)
или [F-Droid](https://f-droid.org/packages/com.nutomic.syncthingandroid).

На iOS нет официального приложения, но есть стороннее
[Möbius Sync](https://apps.apple.com/us/app/mobiussync/id1539203216).

## Использование

### Запуск

Если вы используете консольный интерфейс, то вам потребуется добавить программу
в автозапуск, чтобы она работала в фоне после включения компьютера. На Linux
можно включить сервис `syncthing.service`. Веб-интерфейс доступен по адресу
`http://localhost:8384/`.

При использовании графического интерфейса (например, SyncTrayzor или приложения
для мобильных устройств), настройка должна произойти автоматически. Однако, всё
равно могут возникнуть проблемы. В таком случае, вам потребуется изучить логи.

> [!tip]
Синхронизация может не работать, если включён файервол.

### Добавление устройств

Чтобы добавить устройство, необходимо ввести ID или сканировать QR-код. ID можно
найти в меню. Обратите внимание, что устройства должны находиться в одной
локальной сети.

### Добавление общих папок

Чтобы начать синхронизировать файлы, нужно добавить общие папки. Всё содержимое
в них будет передаваться к каждому устройству и наоборот.

Папки состоят из ярлыка (отображаемое имя), ID (одинаковый для каждого
устройства) и путь. Дополнительно можно включить фильтры, систему версий и
правила синхронизации.

После добавления общей папки, нужно её назначить каждому устройству, с которыми
хотите синхронизировать содержимое. Для этого отметьте нужные устройства и с
этих устройств разрешите доступ. Вам будет предложена та же самая настройка
папки, где нужно указать путь.

## Исправление проблем

- [Форум](https://forum.syncthing.net)

## Смотрите также

- [Официальная документация](https://docs.syncthing.net/intro/getting-started.html)
(англ.)
- [Syncthing на Arch Wiki](https://wiki.archlinux.org/title/Syncthing) (англ.)
