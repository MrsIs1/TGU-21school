# Задание №3. Веб-хранилища №2
## "Local Storage"
|№|Cайт| Ключ | Значение | Цель хранения данного объекта|
|------| ------ | ------ |------|-------|
| 1| https://perm.e2e4online.ru/| b24_crm_guest_utm | {"ts":1688666771,"list":{},"gclid":null} |Установлен уникальный идентификатор конкретного пользователя. |
| 2| https://www.dns-shop.ru/| cartRepositoryHash | c0ebe13d-a2a0-5be2-9adb-d19229879773 |Уникальный идентефикатор корзины |
| 3| https://sbermarket.ru/retailer_selection/all| flockapi:3274:pageViewsLog| [{"viewId":"9ddb7b50-1f47-11ee-b8cc-299328be6413","sessionId":"9ddb7b51-1f47-11ee-b8cc-299328be6413"]}] |Каталоги товаров |
| 4| https://music.yandex.ru/home| Ya_Music_Player_Volume | 1 |Увеличение громкости музыки |
| 5|https://habr.com/ru/companies/youla/articles/540768/ | rom-session-start | Mon Jul 10 2023 12:18:54 GMT+1100 (Сахалин, стандартное время) |Чтобы узнать начало сеанса|
| 6| https://sbermegamarket.ru/ | timeOnSite:activeTime | {"data":510} |Чтобы посмотреть время активности на сайте|

## "Session Storage"
|№|Cайт| Ключ | Значение | Цель хранения данного объекта|
|------| ------ | ------ |------|-------|
| 1| https://hd.kinopoisk.ru/ | tt_sessionId| "ed322596-1f45-11ee-84f0-b8cef68b52b2::uzeRTOeCDlieKmzBjUpl" |Используется социальной сетью TikTok для отслеживания использования встроенных сервисов |
| 2| https://www.dns-shop.ru/ | NRBA_SESSION_ID | b4bef2a296afa9db |Идентефикатор релевантных продуктов |
| 3| https://music.yandex.ru/home |sessionId |5762601689030105224|идентификатор сеанса |
| 4| https://www.tutu.ru/ | _ym26812653_il | "Справочная" |Раздел Справочная|
| 5| https://habr.com/ru/all/ | sessionId | 763431688961189884 |Информация об идентификаторе данного сеанса |
| 6| https://sbermegamarket.ru/ | url-history.prev | {"fullUrl":"https://sbermegamarket.ru/promo-page/zharko-vygodno-skidki-na-tovary-krasoty-i-uhoda/"} | Информация о предыдущей посещаемой странице |
___
**1. Результата выполнения команд для добавления и получения объекта в "Session Storage"**

![Session Storage Console](../misc/images/sessionStorage1.png)

**2. Состояния "Session Storage" после добавления объекта**

![Session Storage Object](../misc/images/sessionStorage2.png)

**3. Результата выполнения команд для добавления и получения объекта в "Local Storage"**

![Local Storage Object](../misc/images/exercise3.localstorage.before.png)

**4. Состояния "Local Storage" после добавления объекта**

![Session Storage Object](../misc/images/exercise3.localstorage.after.png)
