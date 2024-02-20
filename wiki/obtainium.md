# [Obtainium](#obtainium)
> Categories: Android

[Obtainium](https://github.com/ImranR98/Obtainium#readme) — приложение для
Android, которое позволяет получать обновления напрямую от разработчиков.
Поддерживаются многие источники: GitHub, F-Droid, GitLab, Codeberg, APKPure и
другие.

![Obtainium](/media/obtainium.png)

## [Применение](#utilization)

Многие разработчики приложений с открытым исходным кодом публикуют обновления в
репозитории на GitHub, GitLab, Codeberg и др. Однако обычно там нет
автоматической проверки наличия обновлений как в Google Play или
[F-Droid](/wiki/f-droid). Хоть и установка приложений из таких каталогов
удобная и популярная, всё же имеется ряд небольших проблем:

- Разработчики вынуждены ждать проверки перед публикацией обновлений в Google
Play.
- Приложения из официального каталога F-Droid собраны другими людьми, а не
разработчиками, из-за чего обновления задерживаются и версии приложений
отличаются.
- В Google Play и F-Droid есть не все приложения.
- Google Play есть не на всех прошивках Android.

Установка приложений напрямую от разработчиков решает эти проблемы, а Obtainium
позволяет проверять наличие обновлений из таких источников как GitHub. Вы
сможете получать официальные самые последние версии автоматически. Поддержка
многих источников, в том числе F-Droid, избавит от необходимости иметь несколько
установленных магазинов приложений на устройстве.

## [Установка](#installation)

Скачайте Obtainium с
[GitHub](https://github.com/ImranR98/Obtainium/releases/latest)
([app-release.apk](https://github.com/ImranR98/Obtainium/releases/latest/download/app-release.apk)),
затем оно будет проверять наличие обновлений самого себя.

Приложение также доступно в
[F-Droid](https://f-droid.org/packages/dev.imranr.obtainium.fdroid).

## [Использование](#usage)

> **Основная статья:**
[Obtainium Wiki](https://github.com/ImranR98/Obtainium/wiki) (англ.)

### [Добавить приложение](#add-app)

Во вкладке "Добавить" в поле "URL-источник приложения" вставьте ссылку на
репозиторий с приложением, которое вы хотите установить. Вы также можете
воспользоваться поиском внутри Obtainium, чтобы быстро найти нужное приложение.
Если ссылка корректная и содержит релизы, то Obtainium попытается его скачать и
установить. Вам потребуется разрешить установку из неизвестных источников.

Приложение появится в общем списке и будет периодически проверяться на наличие
обновлений (частоту проверки и поведение можно настроить). Приложения можно
разбить по категориям.

При частой проверке можно столкнуться с ограничением. Можно ввести API-ключ
GitHub, чтобы увеличить лимит запросов.

### [Импорт/Экспорт](#importexport)

Список установленных приложений и настройки можно экспортировать. Для этого
зайдите в соответствующую вкладку и выберите каталог для экспорта. Файл JSON
можно экспортировать вручную или автоматически при внесении изменений.
Соответствующая кнопка позволит импортировать данные.

Также доступен импорт из списка URL и репозиториев, помеченных звёздочкой на
GitHub.

Пока что нет возможности автоматически определить уже установленные приложения.
[Статус](https://github.com/ImranR98/Obtainium/issues/163)

## [Исправление проблем](#troubleshooting)

- Баг-трекер на [GitHub](https://github.com/ImranR98/Obtainium/issues)