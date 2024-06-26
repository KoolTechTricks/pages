# [YouTube](#youtube)
> Categories: Compilations

На этой странице собраны скрытые функции, полезные расширения, приложения и
альтернативы для YouTube, чтобы улучшить пользовательский опыт и исправить
надоедливые проблемы.

> flags: no_image

## [Встроенные функции](#builtin-features)

### [Таймер сна и перерывов](#sleep-timer)

В мобильном приложении можно указать время для напоминания сделать перерыв или
лечь спать.

1. Иконка профиля
2. Настройки
3. Общие
4. «Напоминать отдыхать от просмотра» и «Напоминать, что пора спать».

После настройки времени, вас будет периодически прерывать от просмотра с
напоминанием сделать перерыв или лечь спать.

Как правило, такая практика малоэффективна для борьбы с продолжительным временем
просмотра, так как можно легко скрыть напоминания. Однако, они в любом случае
могут помочь вовремя остановиться.

![Напоминание о необходимости лечь спать и сделать перерыв.](/media/youtube_sleep_timer.jpg)

### [Отключение рекомендаций](#turn-off-recomendations)

Рекомендации помогают найти новых авторов и интересный контент. Однако, иногда
они становятся причиной думскролла.

Смотреть видео можно в подписках — лента, в которой только видео от интересных
вам авторов. Но всё равно чаще всего вы оказываетесь в рекомендациях.

Можно попробовать воспользоваться расширением [Unhook](#unhook) или отключить
и очистить историю просмотра.

> [!caution]
Отключение и очистка истории просмотра необратима и приведёт к потере каналов,
на которые вы забыли подписаться.
>
> 1. [Настройки аккаунта Google](https://myaccount.google.com)
> 2. [Данные и конфиденциальность](https://myaccount.google.com/data-and-privacy)
> 3. [История YouTube](https://myactivity.google.com/activitycontrols?settings=youtube) - Отключить

### [Сочетания клавиш](#shortcuts)

На ПК есть сочетания клавиш, которые позволяют быстро выполнять определённые
действия. Некоторые из них вы уже знаете, но есть и менее известные.

- `,` или `.` — предыдущий или следующий кадр соответственно (на паузе).
- `Shift`+`,` или `Shift`+`.` — уменьшить или увеличить скорость воспроизведения
соответственно.
- `Ctrl`+`СтрелкаВлево` или `Ctrl`+`СтрелкаВправо` - перейти на предыдущий или
следующий эпизод соответственно.

Нажмите `Shift`+`/` (на латинской раскладке) или найдите пункт в меню иконки
профиля, чтобы показать все сочетания клавиш.

### [RSS-лента](#rss)

> **Основная статья:** [RSS](/wiki/rss)

Каждый канал на YouTube имеет свою RSS-ленту. Можно добавить свои любимые каналы
в приложения для чтения RSS, чтобы не пропускать их новые видео. Большинство
агрегаторов RSS позволяют располагать ленты по категориям, фильтровать статьи,
так что лента, состоящая из каналов YouTube, позволит проще ориентироваться.

Ссылка на ленту выглядит так:
`https://www.youtube.com/feeds/videos.xml?channel_id=[ID]`, где `[ID]` —
идентификатор канала. Один из способов его получения: зайти во вкладку «О
канале», нажать кнопку «Поделиться» и «Скопировать идентификатор канала». Можно
также воспользоваться различными онлайн-сервисами.

![Демонстрация копирования идентификатора канала](/media/youtube_copy_id.jpg)

![Как выглядит лента в агрегаторе RSS Guard](/media/youtube_rss.jpg)

## [Расширения](#extensions)

### [Unhook](#unhook)

> **Основная статья:** [Unhook](/wiki/unhook)

Unhook убирает отвлекающие элементы интерфейса: рекомендации и следующие видео.
Таким образом, можно отучить себя от бесконечной ленты видео и смотреть только
тех авторов, на которые вы подписаны.

![Скриншот, на котором расширение Unhook убрало все видео из главной страницы
YouTube.](/media/unhook.jpg)

- [Firefox](https://addons.mozilla.org/ru/firefox/addon/youtube-recommended-videos)
и все производные (LibreWolf, Waterfox, Floorp)
- [Chromium](https://chrome.google.com/webstore/detail/unhook-remove-youtube-rec/khncfooichmfjbepaaaebmommgaepoid)
и все производные (Google Chrome, Microsoft Edge, Brave, Opera, Vivaldi, Яндекс)

### [Return YouTube Dislike](#return-youtube-dislike)

> **Основная статья:** [Return YouTube Dislike](/wiki/return_youtube_dislike)

Это расширение возвращает счётчик дизлайков. Значения берутся из архивных данных
и экстраполированного поведения пользователей расширения. Счётчик не на 100%
точный, но показывает довольно реалистичное значение.

Счётчик дизлайков помогает правильно воспринимать видео перед его просмотром и
легко узнавать мнение зрителей.

![Видео, которое имеет большую часть дизлайков. Без расширения дизлайки не были
бы видны.](/media/return_youtube_dislike.png)

- [Firefox](https://addons.mozilla.org/ru/firefox/addon/return-youtube-dislikes)
и все производные (LibreWolf, Waterfox, Floorp)
- [Chromium](https://chrome.google.com/webstore/detail/return-youtube-dislike/gebbhagfogifgggkldgodflihgfeippi)
и все производные (Google Chrome, Microsoft Edge, Brave, Opera, Vivaldi, Яндекс)
- [Пользовательский скрипт (Tampermonkey)](https://github.com/Anarios/return-youtube-dislike/raw/main/Extensions/UserScript/Return%20Youtube%20Dislike.user.js)

### [Аватарки](#profile-pictures)

> [!note]
Данный раздел актуален только для пользователей из России.

Чтобы вернуть аватарки и картинки из постов сообщества, необходимо
перенаправлять запросы с одного CDN-сервера YouTube на другой.

1. Скачайте расширение Resource Override
([Firefox](https://addons.mozilla.org/ru/firefox/addon/resourceoverride) /
[Chromium](https://chrome.google.com/webstore/detail/resource-override/pkoacgokdfckfpndoffpifphamojphii))
2. Нажмите на иконку расширения.
3. Добавьте переадресацию с `https://yt3.ggpht.com/*` на `https://yt4.ggpht.com/*`

![Демонстрация результата конфигурации расширения Resource Override](/media/youtube_resource_override.jpg)

### [SponsorBlock](#sponsorblock)

> **Основная статья:** [SponsorBlock](/wiki/sponsorblock)

[SponsorBlock](https://sponsor.ajay.app) — расширение для пропуска раздражающих
сегментов в видео на YouTube: напоминания о подписке, интро, переход к важной
части, самореклама, спонсоры. Пользователи предлагают новые сегменты или
исправляют уже существующие, чтобы затем расширение их автоматически пропускало
для других.

![Скриншот плеера YouTube с установленным расширением SponsorBlock.
Сегменты с рекламой помечены цветом и автоматически пропускаются при их
достижении.](/media/sponsorblock.jpg)

> [!warning]
Автоматизированный пропуск рекламы может вредить доходам авторов. Подумайте о
возможности пожертвовать деньги автору или купить платную подписку.
[Подробнее](/wiki/sponsorblock#ethics)

- [Firefox](https://addons.mozilla.org/addon/sponsorblock) и все производные
(LibreWolf, Waterfox, Floorp) для ПК и Android
- [Chromium](https://chrome.google.com/webstore/detail/mnjggcdmjocbbbhaepdhchncahnbgone)
и все производные (Google Chrome, Microsoft Edge, Brave, Opera, Vivaldi, Яндекс)
- [Safari](https://github.com/ajayyy/SponsorBlock/wiki/Safari)

### [DeArrow](#dearrow)

> **Основная статья:** [DeArrow](/wiki/dearrow)

[DeArrow](https://dearrow.ajay.app) — расширение для YouTube, которое заменяет
обложки и названия видео на более правдоподобные и менее эмоциональные.
Пользователи могут предлагать свои варианты заголовков, которые затем будут
отображаться другим людям.

![Сравнение оригинальных обложек видео с обложками из DeArrow. Заменённые превью
являются моментами из видео, а названия переписаны так, чтобы можно было понять
о чём будет идти речь.](/media/dearrow.webp)

> [!note]
Официальное расширение является платным. Можно купить ключ за единоразовый
платёж. Это нужно для поддержки разработчиков и оплаты серверов. Однако вы
можете [запросить бесплатный доступ](https://dearrow.ajay.app/free).

- [Firefox](https://addons.mozilla.org/firefox/addon/dearrow) (ПК и Android)
- [Chromium](https://chrome.google.com/webstore/detail/enamippconapkdmgfgjchkhakpfinmaj)
(Google Chrome, Microsoft Edge, Brave, Opera, Vivaldi, Яндекс)
- [Safari](https://apps.apple.com/app/dearrow-for-youtube/id6451469297)

### [BlockTube](#blocktube)

[BlockTube](https://github.com/amitbl/blocktube) — расширение, которое позволяет
блокировать нежелательный контент на YouTube: видео, каналы и комментарии по
ключевым словам, Regex или функции JavaScript. Можно скрывать видео,
просмотренные более определённого процента, или по заданной общей длительности.
Кроме того, можно блокировать автоматические плейлисты (джемы), Shorts и прочие
элементы интерфейса. У каждого видео и канала будет добавлена кнопка в
контекстном меню, позволяющая добавить его в чёрный список.

Расширение полностью блокирует видео, как скрывая их с сайта, так и предотвращая
просмотр по ссылке или встроенному плееру. Такое поведение можно изменить в
настройках.

![Демонстрация экрана настроек BlockTube](/media/youtube_blocktube.jpg)

- [Firefox](https://addons.mozilla.org/firefox/addon/blocktube) и все
производные (LibreWolf, Waterfox, Floorp)
- [Chromium](https://chrome.google.com/webstore/detail/blocktube/bbeaicapbccfllodepmimpkgecanonai)
и все производные (Google Chrome, Microsoft Edge, Brave, Opera, Vivaldi, Яндекс)
- [Руководство](https://github.com/amitbl/blocktube/wiki) (англ.)

## [Утилиты](#utilities)

### [yt-dlp](#yt-dlp)

> **Основная статья:** [yt-dlp](/wiki/yt-dlp)

[yt-dlp](https://github.com/yt-dlp/yt-dlp) — универсальная программа для
скачивания видео со многих популярных сайтов: YouTube, TikTok, X (Twitter),
Reddit, VK и др. Она содержит множество полезных функций в одном месте, в том
числе скачивание плейлистов и прямых эфиров.

yt-dlp предоставляет консольный интерфейс и библиотеку Python. Вы можете
написать свою программу, которая будет использовать yt-dlp, в таком случае
воспользуйтесь
[официальной документацией](https://github.com/yt-dlp/yt-dlp#embedding-yt-dlp)
(англ.). Ниже будет представлено руководство по использованию консольного
интерфейса.

Для того, чтобы скачать видео, плейлист или стрим, нужно написать в консоли
`yt-dlp [параметры] <ссылка(и...)>`. По умолчанию будет выбрано наилучшее
качество. Поддерживается
[более 1000 сайтов](https://github.com/yt-dlp/yt-dlp/blob/master/supportedsites.md).

- `--write-thumbnail` — скачать обложку видео.
- `-S "res:480"` — указать качество (144, 480, 2160 и т.д.).
- `-x` — скачать только аудио.
- `--sponsorblock-mark КАТЕГОРИИ` — пометить сегменты
[SponsorBlock](/wiki/sponsorblock.html): `sponsor`, `intro`, `outro`,
`selfpromo`, `preview`, `interaction`, `all`, `default`.
- `--sponsorblock-remove КАТЕГОРИИ` — удалить сегменты
[SponsorBlock](/wiki/sponsorblock.html): `sponsor`, `intro`, `outro`,
`selfpromo`, `preview`, `interaction`, `all`, `default`.

> [!tip]
Используйте [FFmpeg](/wiki/ffmpeg) для конвертации полученного видео.

![Демонстрация работы yt-dlp.](/media/yt_dlp.jpg)

## [Фронтенды](#frontends)

> [!warning]
Этот раздел нуждается в обновлении.
[Узнайте как помочь](https://github.com/KoolTechTricks/pages/blob/main/CONTRIBUTING.md)

> [!caution]
Использование альтернативных фронтендов вредит авторам, так как не показывается
реклама и отсутствует статистика. Подумайте о возможности пожертвовать деньги
авторам или купить платную подписку.

YouTube можно смотреть анонимно, не подключаясь к самому YouTube напрямую. Это
необходимо для того, чтобы избежать рекламных трекеров, исключить рекомендации
или использовать альтернативный интерфейс. Например, они могут содержать
встроенные функции вышеуказанных [SponsorBlock](#sponsorblock) и
[DeArrow](#dearrow).

Здесь нет рекомендаций, только похожие видео. Поэтому необходимо подписываться
на авторов, которых вы хотите смотреть. Подписки можно экспортировать или
сохранить на сервере. Также каналы можно располагать по категориям и
подписываться на них через RSS.

Такие фронтенды с открытым исходным кодом, и их могут хостить разные люди, из-за
чего необходимо выбирать сервера для подключения.

Google не нравятся такие сервисы, поэтому они могут иногда переставать работать,
пока их не починят разработчики. При этом, они не используют API YouTube, а
значит не нарушают условия пользования.

Они также предоставляют свой API для взаимодействия с YouTube, так что можно
использовать это для простого получения данных. Ещё вы можете воспользоваться
RSS-лентами.

- [Piped](https://piped.video)
([Исходный код](https://github.com/TeamPiped/Piped),
[Сторонние приложения](https://github.com/TeamPiped/Piped#made-with-piped))
- [Invidious](https://github.com/iv-org/invidious)
([Список серверов](https://docs.invidious.io/instances))

Для автоматического перенаправления с YouTube, можно воспользоваться
расширением LibRedirect
([Firefox](https://addons.mozilla.org/firefox/addon/libredirect) /
[Chromium](https://libredirect.github.io/download_chromium.html)).

## [Альтернативы](#alternatives)

> [!warning]
Этот раздел нуждается в отдельной статье.
[Узнайте как помочь](https://github.com/KoolTechTricks/pages/blob/main/CONTRIBUTING.md)

Очень сложно заменить YouTube, так как хостинг для видео очень дорогой. Тем не
менее, существуют альтернативы, куда можно выкладывать свои видео.

[PeerTube](https://joinpeertube.org) — децентрализованная платформа для видео,
основанная на протоколе ActivityPub. Каждый может создать свой сервер, который
будет соединён со множеством других. Достаточно иметь один аккаунт на одном из
серверов, чтобы взаимодействовать с другими.
[Здесь](https://joinpeertube.org/#find-peertube-instances) можно найти список
серверов.
