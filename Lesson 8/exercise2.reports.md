# Баг-репорт

## Баг №1 
**Заголовок:** Ошибка  в JS-коде при нажатии на кнопку «Корзина»	
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Minor   
3. **Шаги к воспроизведению:** 
-  Нажать кнопку «Корзина» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Код состояния : Type Error: DDManager Custom Event "Clicked ToCart Button (Desktop + Mobile Main Icon)" Error 
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)
## Баг №2 
**Заголовок:** Ошибка в JS-коде при нажатии на кнопку «Мега Выгода»
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Minor   
3. **Шаги к воспроизведению:** 
-  Нажать кнопку «Мега Выгода» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Код состояния : TypeError: DDManager Custom Event "Viewed Campaign" Error
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)
## Баг №3 
**Заголовок:** Ошибка в JS-коде при обновлении главной страницы
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Minor   
3. **Шаги к воспроизведению:** 
-  Нажать на значок «Обновить» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Код состояния : Uncaught (in promise) TypeError: NetworkError when attempting to fetch resource.
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)	
## Баг №4
**Заголовок:**  Ошибка запроса CORS при нажатии на кнопку «Войти»	
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Trivial   
3. **Шаги к воспроизведению:** 
-  Нажать кнопку «Войти» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Запрос из постороннего источника заблокирован: Политика одного источника запрещает чтение удаленного ресурса на https://cms-res.online.sberbank.ru/sberid/BlackList/Button/No_Button.json. (Причина: не удалось выполнить запрос CORS).
- Код состояния: (null).
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)
## Баг №5 
**Заголовок:** Ошибка «downloadable font» при обновлении главной страницы
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Trivial  
3. **Шаги к воспроизведению:** 
-  Нажать на значок «Обновить» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Код состояния : downloadable font: download failed (font-family: "SB Sans Text" style:normal weight:400 stretch:100 src index:0): bad URI or cross-site access not allowed source: https://extra-cdn.sbermegamarket.ru/static/dist/fonts/SBSansText-Regular.5faf51.woff2
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)
## Баг №6
**Заголовок:**  Ошибка  отправки запроса на vk.com нажатии на кнопку «О компании»
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Minor   
3. **Шаги к воспроизведению:** 
-  Нажать на  кнопку «О компании»
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Код состояния : Запрос из постороннего источника заблокирован: Политика одного источника запрещает чтение удаленного ресурса на «https://vk.com/rtrg?p=VK-RTRG-1421183-77G99&products_event=view_other&price_list_id=1&e=1&i=0&metatag_url=%2F%2Fsbermegamarket.ru%2Finfo%2Fabout-sbermegamarket-ru%2F&metatag_title=%D0%9E%20%D0%BA%D0%BE%D0%BC%D0%BF%D0%B0%D0%BD%D0%B8%D0%B8%20-%20%D0%9C%D0%B0%D1%80%D0%BA%D0%B5%D1%82%D0%BF%D0%BB%D0%B5%D0%B9%D1%81%20SberMegaMarket.ru». (Причина: Учётные данные не поддерживаются, если заголовок CORS «Access-Control-Allow-Origin» установлен в «*»).
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)
## Баг №7
**Заголовок:**  Ошибка «Open api access error» при нажатии на кнопку «О компании»
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Minor   
3. **Шаги к воспроизведению:** 
-  Нажать на  кнопку «О компании»
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Код состояния : Open api access error
```
v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    onerror https://vk.com/js/api/openapi.js?169:672
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    (Асинхронный: EventHandlerNonNull)
    u https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    d https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    v https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    makeRequest https://vk.com/js/api/openapi.js?169:678
    ProductEvent https://vk.com/js/api/openapi.js?169:3137
    onViewedOther https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    onViewedOther https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    onViewedOther https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    onViewedPage https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    s https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    (Асинхронный: setTimeout handler)
    l https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    onViewedPage https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    trackEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:2
    pushEventQueue https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    o https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    s https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireEvent https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireUnfiredEvents https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    fireUnfiredEvents https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    push https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1
    W https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    Q https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    te https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    setLocationInfo https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    fetchCurrentLocation https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    fetchLocationData https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    identifyRegion https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    mounted https://extra-cdn.sbermegamarket.ru/static/dist/main.e882a233.js:1
    nn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    zn https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
    insert https://extra-cdn.sbermegamarket.ru/static/dist/node_modules.22ca0abc.js:2
```
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)
## Баг №8
**Заголовок:**  Ошибка в JS-коде при нажатии на кнопку «Стать продавцом»
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Minor   
3. **Шаги к воспроизведению:** 
-  нажать на кнопку «Стать продавцом»
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- Код состояния : Uncaught (in promise) TypeError: e is null
```
getSize https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11701079/build/release/full-1b941bd197f0d84fee6bfcf6d459d2c67bb8a127.js:1420
    v https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11701079/build/release/full-1b941bd197f0d84fee6bfcf6d459d2c67bb8a127.js:606
    J https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11701079/build/release/full-1b941bd197f0d84fee6bfcf6d459d2c67bb8a127.js:618
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:64
    promise callback* https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:64
    n https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:1
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:1
    <anonymous> https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:1
full-1b941bd197f0d84fee6bfcf6d459d2c67bb8a127.js:1420:3317
    getSize https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11701079/build/release/full-1b941bd197f0d84fee6bfcf6d459d2c67bb8a127.js:1420
    v https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11701079/build/release/full-1b941bd197f0d84fee6bfcf6d459d2c67bb8a127.js:606
    J https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11701079/build/release/full-1b941bd197f0d84fee6bfcf6d459d2c67bb8a127.js:618
    <анонимный> https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:64
    (Асинхронный: promise callback)
    <анонимный> https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:64
    n https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:1
    <анонимный> https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:1
    <анонимный> https://main-cdn.sbermegamarket.ru/upload/static_pages/2/9d/7de/29d7de3dfd35374d497c997004241940/desktop/js/desktop.js:1
```
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)
## Баг №9
**Заголовок:** Ошибка запроса POST при нажатии на кнопку «Корзина»	
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Trivial  
3. **Шаги к воспроизведению:** 
-  Нажать кнопку «Корзина» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- ошибка запроса POST https://sbermegamarket.ru/api/fl?u=6efd37c0-6ff6-11ed-a2cf-b37c7b2b7873&cfidsw-smm=77C+2Jv/EZWcVV/YiIZWQO68FjdJwyu8M5Dw/+H7esdzV97FUaNBqPmUUoop8viaw1Kld33zpXMA/9YQLU85XyWce2AKxasq8BhCPMpsG/jiX9RZ2yDuigdM0XYppmNAnOvlFhVpHh6qQS0n2mOTJHe+hwnulEy4Avy0pf9u
- код ответа 400 (Bad Request)
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)	
## Баг №10
**Заголовок:**  Ошибка запроса POST при нажатии на кнопку «Войти»	
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Trivial   
3. **Шаги к воспроизведению:** 
-  Нажать кнопку «Войти» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
- ошибка запроса POST https://stream.datago.ru/mp/collect?tid=UA-89387429-1 
- код ответа 404(Not Found)
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)	
## Баг №11
**Заголовок:**  Ошибка запроса GET при нажатии на кнопку «Войти»	
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Trivial  
3. **Шаги к воспроизведению:** 
-  Нажать кнопку «Войти» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
5.  **Фактический результат:** 
-  ошибка запроса GET https://online.sberbank.ru/CSAFront/api/oidc/sbid?client_id=52cd75e2-76e1-43ba-ade6-938b2c7d4e7a 
- код ответа 400(Bad Request)
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)	
## Баг №12
**Заголовок:**  Ошибка во время загрузки ресурсов «server responder with a status of 502» при нажатии на кнопку «QR-код»	
1.  **Предшествующие условия**:
- Открыт сайт https://sbermegamarket.ru/ 	
- Открыта вкладка "Console" (Консоль) в DevTools
2. **Серьезность:** Minor   
3. **Шаги к воспроизведению:** 
-  Нажать кнопку «QR-код» 
4.  **Ожидаемый результат:** 
-  Во вкладке "Console" (Консоль) в DevTools отсутствуют ошибки
4.  **Фактический результат:**
- ошибка запроса GET https://sbermegamarketru.webim.ru/button.php 
- код ответа 502 Bad Gateway
6. **Окружение:** Windows 10 Pro (Firefox Browser.Версия 114.0.2 (64-разрядный)

## Баг №13.  Неуспешный запрос на вход в личный кабинет
	
|URL|	https://online.sberbank.ru/CSAFront/api/oidc/sbid?client_id=52cd75e2-76e1-43ba-ade6-938b2c7d4e7a|
|------------|-----------------|
|Описание|	Неуспешный запрос на вход в личный кабинет|
|Приоритет	| высокий    |
|Серьезность|	значительная|
|Окружение|Mozilla/5.0 (Windows NT 8.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0|
|Предусловия|</li><li>Открыта страница https://sbermegamarket.ru/ |

|Шаги	|Ожидаемый результат|Фактический результат	|
|-------|--------|------|
|1. Нажать кнопку "Войти"|Откроется окно регистрации|Окно регистрации открыто  |
|2. Отправить GET запрос|Запрос успешно оправлен на сервер|Запрос успешно отправлен  |
|3. Проверить код состояния |Код состояния **200**|Код состояния **400**  |


## Баг №14.  Баг нагрузки
	
|URL|	https://widget-api.uxfeedback.ru/v1/widgets/giev56vba9hzuzxxffkx31vr?uid=baf72140-09b6-11ee-98e4-fb8085bcb306&uidType=old&userHash=ca9f17ba4286d605d9ccc24b636c3ee4|
|------------|-----------------|
|Описание|	Ошибка при выборе большого количества товаров|
|Приоритет	| высокий    |
|Серьезность|	значительная|
|Окружение|Mozilla/5.0 (Windows NT 8.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0|
|Предусловия|</li><li>Открыта страница https://sbermegamarket.ru/ |

|Шаги	|Ожидаемый результат|Фактический результат	|
|-------|--------|------|
|1. Открыть каталог | Каталог открыт |  Каталог открыт |
|2. Выбрать категорию товаров "Красота"|Открыта страница с карточками товаров выбранной категории|Открыта страница с карточками товаров выбранной категории |
|3. Выбрать категорию товаров "Лицо"  |Открыта страница с карточками товаров выбранной категории|Открыта страница с карточками товаров выбранной категории |
|4. Продолжать выбирать товары| Открыты карточки разных товаров |  Долго открывается карточка товара |
|5. Проверить код состояния |Код состояния **200**|Код состояния **429 (Слишком много запросов)**  |

## Баг №15.  Ошибка определения продавца
	
|URL|	 https://yastatic.net/s3/front-maps-static/maps-front-jsapi-v2-1/2.1.79-11532562/build/release/full-2e211ea3bc39b6696fa8e65a7c24d6a38733cebe|
|------------|-----------------|
|Описание|	Ошибка определения продавца|
|Приоритет	| высокий    |
|Серьезность|	значительная|
|Окружение|Mozilla/5.0 (Windows NT 8.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0|
|Предусловия|</li><li>Открыта страница https://sbermegamarket.ru/ |

|Шаги	|Ожидаемый результат|Фактический результат	|
|-------|--------|------|
|1. В хеддере сайта нажать кнопку "Стать продавцом" | Откроется страница СберМагаМакрет ПРО |  Открыта страница СберМагаМакрет ПРО   |
|2. Пройти регистрацию|Регистрация пройдена  |Регистрация пройдена   |
|3. Проверить код состояния |Код состояния **200**|Код состояния **Error (Е равно null)**  |  

## Баг №16.  Неуспешный запрос на cdn.ddmanager.ru
	
|URL|	 https://cdn.ddmanager.ru/ddm-initialization/f72a2e9d-633c-4ab0-9cff-2c32b4d5cad6.js:1|
|------------|-----------------|
|Описание|	Ошибка при загрузке ресурсов|
|Приоритет	| средний    |
|Серьезность|	незначительная|
|Окружение|Mozilla/5.0 (Windows NT 8.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0|
|Предусловия|</li><li>Открыта страница https://sbermegamarket.ru/ |

|Шаги	|Ожидаемый результат|Фактический результат	|
|-------|--------|------|
|1. Нажать кнопку "Акции" | Откроется страница с акциями СберМегаМаркет |  Открыта страница с акциями СберМегаМаркет |
|2. Проверить код состояния |Код состояния **200**|Код состояния **Error (Ошибка пользовательского события DDManager)**  |

## Баг №17.  Заблокированный запрос
	
|URL|	https://extra-cdn.sbermegamarket.ru/static/dist/main.564c87f0|
|------------|-----------------|
|Описание|	Ошибка при выборе товара|
|Приоритет	| высокий    |
|Серьезность|	значительная|
|Окружение|Mozilla/5.0 (Windows NT 8.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0|
|Предусловия|</li><li>Открыта страница https://sbermegamarket.ru/ |

|Шаги	|Ожидаемый результат|Фактический результат	|
|-------|--------|------|
|1. Открыть каталог | Каталог открыт |  Каталог открыт |
|2. Выбрать категорию товаров|Открыта страница с карточками товаров выбранной категории|Открыта страница с карточками товаров выбранной категории |
|3. Проверить код состояния |Код состояния 200|Код состояния **Error (Заблокированный запрос)**  |

## Баг №18.  Ошибка синтаксического анализа XML
	
|URL|	https://sbermegamarket.ru/api/fl?u=6efd37c0-6ff6-11ed-a2cf-b37c7b2b7873&cfidsw-smm=%2BJgl5ml7SrZsfAl9yTI2VLxr3qHP2fm3DRMq0yFpWtUropEjH2iprD%2FnS8zRz0zuay5%2BC6mVN%2BYi9t1dX1oqaIyZFwrrzo3NGl7oBl81SmBcRZUsPaL%2Fqjx1RL%2BYwrr9s5b%2F52ejQpW3nw1reZrCLybo306fyJnIeaObniM%3D|
|------------|-----------------|
|Описание|	Ошибка синтаксического анализа XML|
|Приоритет	| низкий     |
|Серьезность|	тривиальная|
|Окружение|Mozilla/5.0 (Windows NT 8.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/114.0|
|Предусловия|</li><li>Открыта страница https://sbermegamarket.ru/ |

|Шаги	|Ожидаемый результат|Фактический результат	|
|-------|--------|------|
|1. Открыть каталог | Каталог открыт |  Каталог открыт |
|2. Выбрать категорию товаров|Открыта страница с карточками товаров выбранной категории|Открыта страница с карточками товаров выбранной категории |
|3. Проверить тег |Тег: **/meta** |Тег: **null**  |

