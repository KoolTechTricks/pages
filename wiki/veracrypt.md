+++
title = 'VeraCrypt'
categories = ['files', 'security']
publishDate = '2023-11-24T17:43:45Z'
lastmod = '2023-12-24T14:31:54Z'
summary = """Программа для шифрования дисков с открытым исходным кодом для \
Windows, macOS и Linux. С помощью неё можно создать виртуальное хранилище в \
виде файла, которое можно смонтировать как диск, а также зашифровать целый \
раздел. Шифрование происходит на лету при записи и чтении файлов."""
cover = '/media/veracrypt.jpg'
featured = true
+++

# VeraCrypt
{{< categories >}}

[VeraCrypt](https://veracrypt.fr) — программа для шифрования дисков с
[открытым исходным кодом](https://veracrypt.fr/code/VeraCrypt) для Windows,
macOS и Linux. С помощью неё можно создать виртуальное хранилище в виде файла,
которое можно смонтировать как диск, а также зашифровать целый раздел.
Шифрование происходит на лету при записи и чтении файлов.

![Скриншот программы VeraCrypt](/media/veracrypt.jpg)

## Применение

Очень важно хранить личные данные (пароли, коды восстановления, документы) в
зашифрованном виде. В случае несанкционированного доступа (утеря или кража
устройства, вирус удалённого доступа) злоумышленник не сможет получить вашу
ценную информацию и воспользоваться ею для своей выгоды.

VeraCrypt позволяет создать надёжное зашифрованное хранилище, которое удобно
используется как виртуальный накопитель. Можно читать и записывать файлы как
обычно, пока в фоне они шифруются.

## Устройство

Из [документации](https://veracrypt.fr/ru/Introduction.html):

> <...> Шифрование на лету означает, что данные автоматически зашифровываются
непосредственно перед записью их на диск и расшифровываются сразу же после их
считывания, то есть без какого-либо вмешательства пользователя. Никакие данные,
хранящиеся в зашифрованном томе, невозможно прочитать (расшифровать) без
правильного указания пароля/ключевых файлов или правильных ключей шифрования.
Полностью шифруется вся файловая система (имена файлов и папок, содержимое
каждого файла, свободное место, метаданные и др.). Файлы можно копировать со
смонтированного тома VeraCrypt и на него точно так же, как и при использовании
любого обычного диска (например, с помощью перетаскивания). <...>
>
> Обратите внимание: VeraCrypt никогда не сохраняет на диске никаких данных в
незашифрованном виде – такие данные временно хранятся только в ОЗУ (оперативной
памяти). Даже когда том смонтирован, хранящиеся в нём данные по-прежнему
остаются зашифрованными. При перезагрузке Windows или выключении компьютера том
будет размонтирован, а хранящиеся в нём файлы станут недоступными (и
зашифрованными). Даже в случае непредвиденного перебоя питания (без правильного
завершения работы системы), хранящиеся в томе файлы останутся недоступными (и
зашифрованными). Чтобы получить к ним доступ вновь, нужно смонтировать том (и
правильно указать пароль и/или ключевой файл).

## Установка

### Windows

Вы можете скачать установщик с
[официального сайта](https://veracrypt.fr/en/Downloads.html) или с помощью
[winget](/wiki/winget): `winget install veracrypt`.

### macOS

Скачайте с [официального сайта](https://veracrypt.fr/en/Downloads.html).

### Linux

Установите с помощью пакетного менеджера:

- Debian/Ubuntu/Mint: `sudo apt install veracrypt`
- Fedora: `sudo dnf install veracrypt`
- Arch Linux: `sudo pacman -S veracrypt`

### Мобильные устройства

На данный момент нет планов по разработке официального приложения VeraCrypt
для мобильных устройств. Однако, существуют сторонние приложения:

Android:

- EDS: [https://sovworks.com/eds/](https://sovworks.com/eds)

iOS:

- Disk Decipher: [https://disk-decipher.app/](https://disk-decipher.app)
- Crypto Disks:
[https://itunes.apple.com/us/app/crypto-disks-store-private/id889549308](https://itunes.apple.com/us/app/crypto-disks-store-private/id889549308)

## Использование

> **Смотрите также:** Документация
([англ.](https://veracrypt.fr/en/Documentation.html)/[рус.](https://veracrypt.fr/ru/Documentation.html))
{.related}

### Создание тома

{{< blockquote >}}
> [!warning]
В этом разделе не будет полностью описан процесс создания тома, для полного
руководства настоятельно рекомендуется ознакомиться с
[документацией](https://veracrypt.fr/ru/Beginner%27s%20Tutorial.html).
{{< /blockquote >}}

Для начала необходимо создать том, в котором будут храниться зашифрованные
данные. Нажмите на соответствующую кнопку, чтобы запустить Мастер создания
томов.

Типы томов:

- **Зашифрованный файл-контейнер:** виртуальный диск внутри файла, который
можно смонтировать как настоящий диск.
- **Раздел или диск без системы:** зашифровать весь внутренний или внешний
накопитель (флешку).
- **Раздел или диск с системой:** зашифровать диск, где установлена Windows.
Перед каждой загрузкой нужно будет вводить пароль для доступа к ОС.

Размер тома является постоянной величиной. Вы можете создать динамический том,
но он будет растягиваться до максимального значения и не будет уменьшаться.

Необходимо выбрать хороший пароль для тома. Вы можете записать пароль и
сохранить в надёжном месте, чтобы не забыть его и навсегда потерять доступ к
файлам на этом томе, но в таком случае вы должны быть уверены, что никто
сможет получить доступ к этому паролю и тем самым расшифровать ваше хранилище.

Последний этап — форматирование тома. Хаотично перемещайте мышь в пределах окна
мастера создания томов в течение хотя бы 30 секунд. Чем дольше вы будете
перемещать мышь, тем значительнее повысите надёжность ключей шифрования.

Для завершения нажмите кнопку **Разметить**. Будет создан файл в ранее
указанном месте. Этот файл и будет являться зашифрованным контейнером.

### Монтирование тома

В главном меню нужно выбрать слот подключения (букву диска), а затем файл или
устройство, которое является зашифрованным томом.

После нажатия кнопки **Смонтировать** появится окно ввода пароля. В
определённых случаях, здесь могут потребоваться дополнительные параметры.

После успешного ввода пароля в указанный слот (букву диска) будет смонтирован
зашифрованный контейнер VeraCrypt, на который можно скопировать файлы, а затем
читать их.

{{< blockquote >}}
> [!warning]
После того, как вы скопируете существующие незашифрованные файлы на том
VeraCrypt, вы должны надёжно удалить (затереть) исходные незашифрованные файлы.
Удаление через интерфейс операционной системы лишь разрешит запись данных
заместо удалённых файлов, поэтому их можно будет восстановить. Для надёжного
стирания существуют специальные программы.
{{< /blockquote >}}

После завершения работы с томом, вы можете его размонтировать, в таком случае
содержимое станет недоступным, пока вы не введёте пароль. Размонтирование
происходит автоматически при выключении или перезагрузки компьютера.
