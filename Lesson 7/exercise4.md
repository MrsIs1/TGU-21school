# Отчет о проделанных проверках

1. Метод __GET​/api​/v1​/Activities__

URL  https://fakerestapi.azurewebsites.net/api/v1/Activities

Ождаемый результат  200 ок, тест успешно пройден.

__Заголовок запроса__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Postman-Token: e8ad9d17-a93e-4634-9559-d969f0be7628
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
Отсутствует

__Заголовок ответа__

```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Wed, 21 Jun 2023 20:10:35 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

__Тело ответа__
Отсутствует

2. Метод __(POST)/api​/v1​/Activities__ Позитив

URL https://fakerestapi.azurewebsites.net/api/v1/Activities

Ождаемый результат  200 ок, тест успешно пройден.

__Заголовок запроса__

```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:24:07 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```


__Тело запроса__

`{"id":0,"title":"string","dueDate":"2023-06-21T20:12:24.942Z","completed":true}`

__Заголовок ответа__

```
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 247ceecf-5a5d-43ee-9b01-077b978cd2c3
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело ответа__

```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-21T20:12:24.942Z",
  "completed": true
}
```

3. Метод __(POST)/api​/v1​/Activities__ Удалить тело

URL https://fakerestapi.azurewebsites.net/api/v1/Activities

Ождаемый результат  400 плохой ввод..

__Заголовок запроса__

```
Content-Length: 0
Date: Fri, 23 Jun 2023 21:30:47 GMT
Server: Kestrel
```
__Тело запроса__

Отсутствует

__Заголовок ответа__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 1cccf979-6bcd-4132-8cd0-c7496d0872cd
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
__Тело ответа__

Отсутствует

4. Метод __(POST)/api​/v1​/Activities__ Негативный

URL https://fakerestapi.azurewebsites.net/api/v1/Activities

Ождаемый результат  400 плохой ввод..

__Заголовок запроса__

```
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 292ea73b-d391-41c7-a4c0-ef93bfce2aa2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```
__Тело запроса__

```
{
  "id": 7482448784512,
  "title": "string",
  "dueDate": "2023-06-21T20:12:24.942Z",
  "completed": true
}
```

__Заголовок ответа__

```
Content-Length: 0
Date: Fri, 23 Jun 2023 21:33:13 GMT
Server: Kestrel
Allow: DELETE, GET, PUT
```
__Тело ответа__

Отсутствует

5. Метод __(GET)/api​/v1​/Activities​/{id}__

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id}}

Ождаемый результат  200 ок, тест успешно пройден.

__Заголовок запроса__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 8cc7ca34-19df-4ac2-8c82-0c8a78df61da
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
Отсутствует

__Заголовок ответа__

```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:48:30 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

__Тело ответа__
`{"id":27,"title":"Activity 27","dueDate":"2023-06-25T00:48:30.7982593+00:00","completed":false}`

6. Метод __(GET)/api​/v1​/Activities​/{id}__Негатив

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/15

Ождаемый результат  200 ок, тест успешно пройден.

__Заголовок запроса__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: ae1724d6-ee3a-45a8-9ec7-7208ea6a2fb4
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
Отсутствует

__Заголовок ответа__

```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:44:08 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

__Тело ответа__
`{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-4d61ef2a859ee34197979a33e07dbfeb-67c064366d3b3b49-00"}`

7. Метод __(GET)/api​/v1​/Activities​/{id}__Отрицательное

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id_minus}}

Ождаемый результат  200 ок, тест успешно пройден.

__Заголовок запроса__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 8494eb0f-3c81-42b6-af81-6818bec9e1b8
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
Отсутствует

__Заголовок ответа__

```
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:46:11 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

__Тело ответа__
`{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.4","title":"Not Found","status":404,"traceId":"00-d4ee55713ec9fe468ea57bd9a6cde834-148806fd1e808149-00"}`


8. Метод __(PUT)/api​/v1​/Activities​/{id}__Успешно

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id}}

Ождаемый результат  200 ок, тест успешно пройден.

__Заголовок запроса__

```
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 0b7e1051-1e27-43ec-8465-64997c7f5002
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-23T21:07:43.578Z",
  "completed": true
}
```


__Заголовок ответа__

```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:54:29 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

__Тело ответа__
`{"id":0,"title":"string","dueDate":"2023-06-23T21:07:43.578Z","completed":true}}`



9. Метод __(PUT)/api​/v1​/Activities​/{id}__Отрицательное

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id_nigga}}

Ождаемый результат  404 ок, yt yfqlty.

__Заголовок запроса__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 3a3bbb94-e53b-4489-9683-ea91eacf6cac
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
Отсутствует


__Заголовок ответа__

```
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 21:59:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
```

__Тело ответа__
`{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.13","title":"Unsupported Media Type","status":415,"traceId":"00-dc28a28b662a18408ed01a1fb88e2d1b-74f64e30fa49fe4b-00"}`

10. Метод __(PUT)/api​/v1​/Activities​/{id}__Отрицательное

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id}}

Ождаемый результат  400 ок, gkj[jq ddj;].

__Заголовок запроса__

```
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 9f5c578c-8571-46ed-8ffd-5a1473f0442a
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
```
{
  "id": 89,
  "title": "string",
  "dueDate": "2023-06-23T21:07:43.578Z",
  "completed": true
}
```


__Заголовок ответа__

```
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 22:01:56 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
```

__Тело ответа__
`{"id":89,"title":"string","dueDate":"2023-06-23T21:07:43.578Z","completed":true}`

11. Метод __(DELETE)/api​/v1​/Activities​/{id}__Успешно

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id}}

Ождаемый результат  404 ок, не наййден.

__Заголовок запроса__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: f6045448-a6fc-42d7-a398-decc00221855
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
Отсутствует

__Заголовок ответа__

```
Content-Length: 0
Date: Fri, 23 Jun 2023 22:04:05 GMT
Server: Kestrel
api-supported-versions: 1.0
```

__Тело ответа__
Отсутствует


12. Метод __(DELETE)/api​/v1​/Activities​/{id}__Отрицательное

URL https://fakerestapi.azurewebsites.net/api/v1/Activities/{{activity_id_minus}}

Ождаемый результат  400 ок, gkj[jq ddjl].

__Заголовок запроса__

```
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: df0d1633-1083-448d-b67d-6eda6ff63740
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
```


__Тело запроса__
Отсутствует

__Заголовок ответа__

```
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 22:05:50 GMT
Server: Kestrel
Transfer-Encoding: chunked
```

__Тело ответа__
`{"type":"https://tools.ietf.org/html/rfc7231#section-6.5.1","title":"One or more validation errors occurred.","status":400,"traceId":"00-7d556ec011db0f44b4024881885c2e8b-8fbb5dcc27aee249-00","errors":{"id":["The value '7482448784512' is not valid."]}}`


## Authors

**_1. Authors. Запрос данных с указанного ресурса (GET) /api/v1/Authors_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors<br>
**Ожидаемый результат**  код статуса 200 ок - успешно, получение списка авторов<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: f8284393-5ab3-4492-a242-9d3f95e9fac6
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:42:11 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
Отсутствует<br>


**_2. Authors. Запрос для создания данных(POST) /api/v1/Authors_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors<br>
**Ожидаемый результат**  код статуса 200 ок - успешно<br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 6cd72068-3427-4357-b188-c792ad27ba29
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id": 610,
  "idBook": 1,
  "firstName": "user1",
  "lastName": "user1"
}
````
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:16:24 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
{
    "id": 610,
    "idBook": 1,
    "firstName": "user1",
    "lastName": "user1"
}
````


**_3. Authors. Запрос для создания данных(POST) /api/v1/Authors neg_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors <br>
**Ожидаемый результат**  код статуса 400  Bad Request <br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a6c6272c-fd43-43d1-b6d6-97df57a9c37f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````
**Тело запроса**<br>
````
{
  "id": null,
  "idBook": 0,

  "firstName": "string",
  "lastName": "string"
}
````
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 21:25:11 GMT
Server: Kestrel
Transfer-Encoding: chunked

````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-07e10c8c8417164ea8ad5e367d1fc97c-af9c55fd0cf78846-00",
    "errors": {
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
}
````



**_4. Просмотр автора определенной книги (GET) api/v1/Authors/authors/books/15_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/{{Authors_id}} <br>
**Ожидаемый результат**  код статуса 200 ок - успешно, получение списка авторов книги 15<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 19743297-8b58-440e-8bf9-66dab7e2f7b2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:33:47 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0

````
**Тело ответа**<br>
````
[
    {
        "id": 40,
        "idBook": 15,
        "firstName": "First Name 40",
        "lastName": "Last Name 40"
    },
    {
        "id": 41,
        "idBook": 15,
        "firstName": "First Name 41",
        "lastName": "Last Name 41"
    }
]
````


**_5. Просмотр автора определенной книги (GET)api/v1/Authors/authors/books/12345678900_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/{{Authors_bad_id}} <br>
**Ожидаемый результат**  код статуса 400 Bad Request <br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: ad03b392-6b3b-495a-a643-0af1295a5144
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 21:38:51 GMT
Server: Kestrel
Transfer-Encoding: chunked

````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-a704e5daf2c4df4abb01e456d1b884d0-7bb40f57d2a3ed47-00",
    "errors": {
        "idBook": [
            "The value '12345678900' is not valid."
        ]
    }
}
````



**_6. Authors.Просмотр автора определенной книги (GET)/api/v1/Authors/authors/books/201_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/{{Authors_bug_id}} <br>
**Ожидаемый результат**  код статуса 404 Not Found<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: ab5c4b03-3707-43be-ba7d-09b64888f455
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:45:31 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
Отсутствует<br>



**_7. Authors.Просмотр определенного автора (GET)/api/v1/Authors/15_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_id}} <br>
**Ожидаемый результат**  код статуса 200 ок - успешно<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 6de1182e-9dd7-43e2-ad91-11a1ce67f138
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:48:55 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
{
    "id": 15,
    "idBook": 5,
    "firstName": "First Name 15",
    "lastName": "Last Name 15"
}
````


**_8. Authors.Просмотр определенного автора (GET) /api/v1/Authors/700_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_not_id}} <br>
**Ожидаемый результат**  код статуса 404Not Found<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 2bd18c8d-202d-4e39-94a0-661764ceb7b0
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:52:00 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
    "title": "Not Found",
    "status": 404,
    "traceId": "00-c9484b2baf77ef49bbc8aea42a53d0bc-5316a7902739d747-00"
}
````


**_9. Authors. Обновление определенного автора  (​PUT)/api/v1/Authors/15_**<br>
**URL**  https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_id}}<br>
**Ожидаемый результат**  код статуса 200 ок - успешно<br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 4977f0e4-204b-439c-80a4-fe892a34c3a3
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
````
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 21:54:34 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
{
    "id": 0,
    "idBook": 0,
    "firstName": "string",
    "lastName": "string"
}
````


**_10. Authors. Обновление определенного автора  (​PUT)/api/v1/Authors/700_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_not_id}} <br>
**Ожидаемый результат**  код статуса 400 Bad Request<br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 3e2d7369-f48b-4ecf-9610-e5cafed407f4
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id":  ,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
````
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 21:57:43 GMT
Server: Kestrel
Transfer-Encoding: chunked
````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-136a487a56bc344db92322864e3d3ef6-1a27b8dd920bab4b-00",
    "errors": {
        "$.id": [
            "',' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
        ]
    }
}
````


**_11. Authors. Удалить определенного автора DELETE/api/v1/Authors/700_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_not_id}} <br>
**Ожидаемый результат**  код статуса 200 ок - успешно<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 678a4bac-bd0e-44d2-8e12-f1933ef149b2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Length: 0
Date: Thu, 22 Jun 2023 22:01:01 GMT
Server: Kestrel
api-supported-versions: 1.0
````
**Тело ответа**<br>
Отсутствует<br>


**_12. Authors. Удалить определенного автора (DELETE)/api/v1/Authors/12345678900_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_bad_id}}  <br>
**Ожидаемый результат**  код статуса 400 Bad Request<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: aa8ba64b-30b3-47c1-bca7-28026bf858c8
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Thu, 22 Jun 2023 22:02:56 GMT
Server: Kestrel
Transfer-Encoding: chunked
````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-dc931209ade9d34093581f1eec41a0c8-eac484913bbbd44c-00",
    "errors": {
        "id": [
            "The value '12345678900' is not valid."
        ]
    }
}
````

## CoverPhotos


**_1. CoverPhotos. Запрос данных с указанного ресурса (GET)/api/v1/CoverPhotos_** <br>
**URL**https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos  <br>
**Ожидаемый результат**  код статуса 200 ок - успешно, получение списка обложек<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 0bf6c861-480f-4163-94ef-e1d4c62ca03d
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 18:10:21 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
    {
        "id": 1,
        "idBook": 1,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
    },
    {
        "id": 2,
        "idBook": 2,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"
  ````      

**_2. CoverPhotos. Запрос для создания данных(POST)/api/v1/CoverPhotos_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos <br>
**Ожидаемый результат**  код статуса 201 Created <br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: fddfb2ae-9f8b-4b19-b89d-96a87db363ff
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
````
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 18:15:16 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
`````
{
    "id": 0,
    "idBook": 0,
    "url": "string"
}
`````



**_3.CoverPhotos. Запрос для создания данных(POST)/api/v1/CoverPhotos _**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos <br>
**Ожидаемый результат**  код статуса 400 Bad Request<br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a5883dc7-1c9a-4d11-83b5-de8f2f827aa1
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{

 "id": 0,

 "idBook": 12345678900,

 "url": "string"

}
````
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 18:21:08 GMT
Server: Kestrel
Transfer-Encoding: chunked
````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-2e31cd5cffb53a41b34e1bfae130f365-1639d30ec520064a-00",
    "errors": {
        "$.idBook": [
            "The JSON value could not be converted to System.Int32. Path: $.idBook | LineNumber: 4 | BytePositionInLine: 22."
        ]
    }
}
````

**_4. CoverPhotos. Просмотр обложки определенной книги (GET)api/v1/CoverPhotos/books/covers/15_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/{{Authors_id}} <br>
**Ожидаемый результат**  код статуса 200 ок - успешно<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: d6af18c0-6489-4b09-8b94-679f26bdc79b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 18:27:12 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
[
    {
        "id": 15,
        "idBook": 15,
        "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 15&w=250&h=350"
    }
]
````

**_5. CoverPhotos.Просмотр обложки определенной книги (GET)api/v1/CoverPhotos/books/covers/12345678900_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/{{Authors_bad_id}} <br>
**Ожидаемый результат**  код статуса 400 Bad Request<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a7226bb8-8bae-4f6f-aa30-759b81a33749
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 18:29:28 GMT
Server: Kestrel
Transfer-Encoding: chunked
````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-997405e1a326c342b6142dd92319b9d2-539f9da827e3344a-00",
    "errors": {
        "idBook": [
            "The value '12345678900' is not valid."
        ]
    }
}
````


**_6. CoverPhotos.Просмотр обложки определенной книги (GET)api/v1/CoverPhotos/books/covers/201_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/{{Authors_bug_id}} <br>
**Ожидаемый результат**  код статуса 404 Not Found<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: dcec667b-a229-4b2e-bde8-011bbb8ad6ec
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 18:32:47 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
Отсутствует<br>



**_7. CoverPhotos.Просмотр определенной обложки(GET)api/v1/CoverPhotos/15_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{Authors_id}} <br>
**Ожидаемый результат**  код статуса 200 ок - успешно<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 8dbf0f5d-3bce-4d38-8f7e-254ca45a4014
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 18:35:30 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
{
    "id": 15,
    "idBook": 15,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 15&w=250&h=350"
}
````



**_8. CoverPhotos.Просмотр определенной обложки (GET)api/v1/CoverPhotos/201_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{Authors_bug_id}} <br>
**Ожидаемый результат**  код статуса 404 Not Found<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 0d9d629d-07fe-4450-8f90-74e9334bbeef
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 18:37:20 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
    "title": "Not Found",
    "status": 404,
    "traceId": "00-9983c9ee75be4a419b52d9b4d22b6cbe-2a40ed68b26e7e40-00"
}
````


**_9. CoverPhotos. Обновление определенной обложки (​PUT)/api/v1/CoverPhotos/15_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{Authors_id}} <br>
**Ожидаемый результат**  код статуса 200 ок - успешно<br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 91bd298c-03ad-4f27-a80e-fa8d23747374
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id": 0,
  "idBook": 0,
  "url": "user2"
}
````
**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 18:40:07 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
````
{
    "id": 0,
    "idBook": 0,
    "url": "user2"
}
````


**_10. CoverPhotos. Обновление определенной обложки  (​PUT) /api/v1/CoverPhotos/200_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/200 <br>
**Ожидаемый результат**  код статуса 400 Bad Request<br>
**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 31e87197-b913-4b76-8636-34f94cd69411
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id":  ,
  "idBook":  null,
  "url": "string"
}
````
**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 18:43:03 GMT
Server: Kestrel
Transfer-Encoding: chunked
````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-14a7a0561ae22644a7cb10aebd57274c-f5bdb2b292397d4a-00",
    "errors": {
        "$.id": [
            "',' is an invalid start of a value. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
        ]
    }
}
````


**_11. CoverPhotos. Удалить определенную обложку (DELETE)/api/v1/CoverPhotos/201_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{Authors_bug_id}} <br>
**Ожидаемый результат**  код статуса 204<br>
**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: e4c39ba0-8221-4c9d-b3a7-7d0c513574c7
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>
**Заголовок ответа**<br>
````
Content-Length: 0
Date: Fri, 23 Jun 2023 18:46:02 GMT
Server: Kestrel
api-supported-versions: 1.0
````
**Тело ответа**<br>
Отсутствует<br>


**_12. CoverPhotos. Удалить определенную обложку (DELETE)/api/v1/CoverPhotos/12345678900_**<br>
**URL** https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/{{Authors_bad_id}} <br>
**Ожидаемый результат**  код статуса 400 Bad Request<br>

**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 024fc7b3-fb59-4c96-98ee-6b42ce65a3ce
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````

**Тело запроса**<br>
Отсутствует<br>

**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 18:48:05 GMT
Server: Kestrel
Transfer-Encoding: chunked
````

**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-cdbc4a8b65d08c49bcaa55852f2882ed-1efcad9dc7c2f04c-00",
    "errors": {
        "id": [
            "The value '12345678900' is not valid."
        ]
    }
}
````


## Books

**_1. Books. Запрос данных с указанного ресурса (GET) /api/v1/Books_**<br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Books<br>


**Ожидаемый результат**  код статуса 200 ок - успешно, получение списка книг<br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 3b281d78-16c5-42cb-a683-a7adf404fa6c
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Thu, 22 Jun 2023 20:42:11 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````


**Тело ответа**<br>
```
[
    {
        "id": 1,
        "title": "Book 1",
        "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
        "pageCount": 100,
        "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
        "publishDate": "2023-06-22T19:37:11.342326+00:00"
    }
] 
```


**_2. Books. Запрос для создания данных(POST) /api/v1/Books_**<br>

**URL** //fakerestapi.azurewebsites.net/api/v1/Books<br>


**Ожидаемый результат**  код статуса 200 ок - успешно<br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: e8ea36b2-7c2e-402d-b42f-7c34a7602af4
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
````
{
  "id": 1,
  "title": "The last book",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T19:52:57.251Z"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 19:31:01 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````


**Тело ответа**<br>
````
{
  "id": 1,
  "title": "The last book",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T19:52:57.251Z"
}
````


**3. Books. Запрос для создания данных(POST) /api/v1/Books**<br>

**URL** {{url}}/api/v1/Books?id={{id_add_new}} <br>


**Ожидаемый результат**  код статуса 201 Created <br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a0e115a1-7305-46e1-98e7-e2d73ce87072
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````


**Тело запроса**<br>
````
{
  "id": 44444,
  "title": "The last book",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T19:52:57.251Z"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 19:32:04 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````


**Тело ответа**<br>
````
{
    "id": 44444,
    "title": "The last book",
    "description": "string",
    "pageCount": 0,
    "excerpt": "string",
    "publishDate": "2023-06-21T19:52:57.251Z"
}
````


**4. Books. Запрос для создания данных (POST) /api/v1/Books**<br>

**URL** {{url}}/api/v1/Books/api/v1/Books <br>


**Ожидаемый результат**  код статуса 404 Not Found <br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: e2776911-f1be-4882-a312-76fa92aca519
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
````
{
  "id": null,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T19:52:57.251Z"
}
````


**Заголовок ответа**<br>
````
ontent-Length: 0
Date: Fri, 23 Jun 2023 20:03:26 GMT
Server: Kestrel

````
**Тело ответа**<br>
отсутствует <br>


**5**. Books. Выбор определенной книги (GET) api/v1/Books/15<br>

**URL** {{url}}/api/v1/Books/?id={{Authors_id}} <br>


**Ожидаемый результат**  код статуса 200 ок - успешно, получение списка книг <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 1e81c9ae-8799-4f85-b4c0-0dd1b4a4928c
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 20:11:45 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````


**Тело ответа**<br>
````
[
    {
        "id": 1,
        "title": "Book 1",
        "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
        "pageCount": 100,
        "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
        "publishDate": "2023-06-22T20:11:46.5259885+00:00"
    }
]
````


**_6. Books. Выбор определенной книги (GET). Негатив_**<br>

**URL** {{url}}/api/v1/Books/{id}?id=-15 <br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 709b924d-b0f6-45c6-b1ad-c429fe9e487f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````
**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 20:17:54 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-8f4cfdb31e3f9b44a6254eaa019b839f-464c1ec5f7f5f540-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
````


**_7. Books. Выбор определенной книги GET/api/v1/Books/4444444444_**<br>

**URL** {{url}}/api/v1/Books/{id}?={{id_wrong}} <br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 463e0578-0e5e-44a5-9bd4-462e0fef690b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
ontent-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 20:26:21 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-6433618870f9a84ea20247b95a890199-a41289cbff19ba45-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
```


**_8. Books. Выбор созданной книги GET/api/v1/Books_**<br>

**URL** {{url}}/api/v1/Books/{id}?id={{id_add_new}} <br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: c567a5e5-7fb4-4aae-bd8d-15275651b4f6
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 20:36:07 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3e7c2f054c7b914aad28bf0c59891582-117122c462bcea46-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
````


**9_. Books. Обновление определенной книги  (​PUT) /api/v1/Books/{id}**<br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_not_id}} <br>


**Ожидаемый результат**  код статуса 400 Bad request <br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a7f63221-9bba-4714-b339-f2f8a7c51637
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
```
{
  "id": 15,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T23:07:20.063Z"
}
```


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 20:46:14 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-f5133d852927b74d9c34410ef25ce925-90241acd79ce5f41-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
````


**_10. Books. Обновление определенной книги  (​PUT). Негатив/api/v1/Books_**<br>

**URL**  {{url}}/api/v1/Books/{15}?id={{Authors_id}}<br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 659937c1-d3ba-48e4-b308-9a41cda53db0
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
````
{
  "id": 44444,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T23:07:20.063Z"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 20:56:57 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-681b1a429d18324f97759a19d8f6546a-3def7f82e8d1624c-00",
    "errors": {
        "id": [
            "The value '{15}' is not valid."
        ]
    }
}
````


**_11. Books. Обновление определенной книги. PUT/api/v1/Books_**<br>


**URL** {{url}}/api/v1/Books/{id}?id=-15 <br>


**Ожидаемый результат**  код статуса 400 Bad Request<br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 21718403-29b9-4aef-b2d4-53462fa37e3c
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
````
{
  "id": -15,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T23:07:20.063Z"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 21:01:22 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
  "id": -15,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-21T23:07:20.063Z"
}
````

**_12. Books. Удалить определенную книгу. DELETE/api/v1/Books_**<br>
**URL** {{url}}/api/v1/Books/{id}?={{id_delete_pos}} <br>


**Ожидаемый результат**  код статуса 200 ок - успешно <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a0c87bce-1411-4856-b8be-ac2989ef587b
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>

**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 21:10:26 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
Отсутствует 
<br>


**_13. Books. Удалить определенную книгу. DELETE/api/v1/Books/12345678900_**<br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_bad_id}}  <br>


**Ожидаемый результат**  код статуса 400 Bad Request<br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: e154463a-291e-4d33-86f6-a08af9962837
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 21:15:36 GMT
Server: Kestrel
Transfer-Encoding: chunked
````

**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-2ee863e6c2d3934595d595a97b9deeaf-34739ca89e1c9e4c-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
````


**_14. Books. Удалить определенную книгу. DELETE/api/v1/Books/300_**<br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Authors/{{Authors_bad_id}}  <br>
**Ожидаемый результат**  код статуса 400 Bad Request<br>

**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 5ec0cb0d-cba0-4153-86e1-b653f2a29536
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 21:20:33 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-b7d85c73845e34448cacfd8efd1296f8-5f45c2c6f9d48f4f-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
````


## Users

**_1. Users. Запрос данных с указанного ресурса (GET) /api/v1/Users_**<br>

**URL** {{url}}/api/v1/Users <br>


**Ожидаемый результат**  код статуса 200 ок - успешно, получение списка пользователей <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 7f641501-7e36-49c2-9c5e-f0f33b0da4d4
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:25:23 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````
**Тело ответа**<br>
```
    {
        "id": 1,
        "userName": "User 1",
        "password": "Password1"
    },
    {
        "id": 2,
        "userName": "User 2",
        "password": "Password2"
    },       
```

**_2. Users. Запрос для создания данных(POST) /api/v1/Users_**<br>

**URL** {{url}}/api/v1/Users?={{id post}} <br>


**Ожидаемый результат**  код статуса 200 ок - успешно <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: a52ca5da-4a08-45f1-8e3d-00bf147a4de9
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
````
{
  "id": 1,
  "userName": "string",
  "password": "string"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:45:49 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````


**Тело ответа**<br>
````
{
    "id": 1,
    "userName": "string",
    "password": "string"
}
````


**_3. Users. Запрос для создания данных. POST/api/v1/Users_** <br>

**URL** {{url}}/api/v1/Books?id={{id_add_new}} <br>


**Ожидаемый результат**  код статуса 201 Created <br>


**Заголовки запроса**<br>
````


User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: ffc37529-7aa7-4952-bd11-d81a9303e4b9
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````


**Тело запроса**<br>
````
{
  "id": 44444,
  "userName": "string",
  "password": "string"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 21:53:06 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0

````


**Тело ответа**<br>
````
{
    "id": 44444,
    "userName": "string",
    "password": "string"
}
````


**_4. Users. Запрос для создания данных. POST/api/v1/Users_**<br>

**URL** {{url}}/api/v1/Users?=null <br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 54a816bc-6bad-40d7-88fd-c6fdc7af98d4
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````


**Тело запроса**<br>
````
{
  "id": null,
  "userName": "string",
  "password": "string"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 21:57:57 GMT
Server: Kestrel
Transfer-Encoding: chunked

````
**Тело ответа**<br>
```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3495eea08cbd7f42b47d60a6741c7485-ee89df6faa482a43-00",
    "errors": {
        "$.id": [
            "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 1 | BytePositionInLine: 12."
        ]
    }
} 
```
<br>


**_5. Users. Выбор определенного пользователя. GET/api/v1/Users/10_**<br>

**URL** {{url}}/api/v1/Users?=10 <br>


**Ожидаемый результат**  код статуса 200 ок - успешно, получение списка книг <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 7bcd231c-8011-4350-9b17-5481726731cd
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 22:28:09 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0

````


**Тело ответа**<br>
````
[
    {
        "id": 1,
        "userName": "User 1",
        "password": "Password1"
    },
    {
        "id": 2,
        "userName": "User 2",
        "password": "Password2"
    }
]
````


**_6. Users. Выбор определенного пользователя. Негатив. (GET)/api/v1/Users/-10_**<br>

**URL** {{url}}/api/v1/Users/{id}?=-10 <br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 979280fe-387c-444e-8034-f6de81ee5935
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive

````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 22:45:56 GMT
Server: Kestrel
Transfer-Encoding: chunked


````
**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-fd0de82199086645a1ce8936633ff8da-c25112e478eba746-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
````



**_7. Users. Выбор определенного пользователя GET/api/v1/Users_**<br>

**URL** {{url}}/api/v1/Users/{id}?=4444444444 <br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: d17768ab-9228-44c6-b7a5-9bb6c67dff10
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 23:32:10 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>

```
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-b3f89922fa99b04d862c5fafda75af51-70308bd79d3ff046-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
```

 
**_8. Users. Выбор созданного пользователя GET/api/v1/Users_**<br>

**URL** {{url}}/api/v1/Books/{id}?id={{id_add_new}} <br>


**Ожидаемый результат**  код статуса 400 Bad Request <br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: c567a5e5-7fb4-4aae-bd8d-15275651b4f6
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 20:36:07 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-3e7c2f054c7b914aad28bf0c59891582-117122c462bcea46-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
````


**_9. Users. Обновление определенного пользователя ​PUT/api/v1/Users_** <br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/{{Authors_id}} <br>


**Ожидаемый результат**  код статуса 200 ок - успешно<br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: d8faced2-2524-4c66-9098-4e58369df413
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id": 15,
  "userName": "Petrov",
  "password": "@"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/json; charset=utf-8; v=1.0
Date: Fri, 23 Jun 2023 23:08:12 GMT
Server: Kestrel
Transfer-Encoding: chunked
api-supported-versions: 1.0
````


**Тело ответа**<br>
````
{
    "id": 15,
    "userName": "Petrov",
    "password": "@"
}
````

**_10. Users. Обновление определенного пользователя  ​PUT/api/v1/Users_** <br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/{id}?id={{Authors_id}} <br>


**Ожидаемый результат**  код статуса 400 Bad Request<br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: c33cd1e2-b17e-42a9-8101-d447a7e493b4
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
````
{
  "id": 44444,
  "userName": "string",
  "password": "string"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 23:03:24 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-caf384660bc6b140ab206e2687bdb4ad-f201ec0aef527c48-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}

````


**_11. Users. Обновление определенного пользователя PUT/api/v1/Users_** <br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/{id}?=-15 <br>


**Ожидаемый результат**  код статуса 400 Bad Request<br>


**Заголовки запроса**<br>
````
Content-Type: application/json
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: edeeea30-9e43-446b-9404-c6babdb93976
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
````
{
  "id": -15,
  "userName": "string",
  "password": "string"
}
````


**Заголовок ответа**<br>
````
Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 22:42:23 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````
{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-6440e33df3ae1b4c832046fab5127002-53cd9d12c63cfd41-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}

````


**_12. Users. Удалить определенного пользователя (DELETE)/api/v1/Users/15_** <br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/10 <br>


**Ожидаемый результат**  код статуса 200 ок - успешно<br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: d8aaed6d-1a2e-4269-83a2-da4ef983ab2f
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````
**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Length: 0
Date: Fri, 23 Jun 2023 22:20:09 GMT
Server: Kestrel
api-supported-versions: 1.0
````


**Тело ответа**<br>
Отсутствует<br>


**_13. Users. Удалить определенного пользователя (DELETE)/api/v1/Users/12345678900_** <br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/{{Authors_bad_id}} <br>


**Ожидаемый результат**  код статуса 400 Bad Request<br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 913dacc5-3459-444f-905b-689493e94ac2
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````


**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````


Content-Type: application/problem+json; charset=utf-8
Date: Fri, 23 Jun 2023 21:42:36 GMT
Server: Kestrel
Transfer-Encoding: chunked
````


**Тело ответа**<br>
````

{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-653a2bdd3ae3a94aaa06501846b344d2-71f556e6d22ebe41-00",
    "errors": {
        "id": [
            "The value '12345678900' is not valid."
        ]
    }
}
````


**_14. Users. Удалить определенного пользователя (DELETE)/api/v1/Users/300_** <br>

**URL** https://fakerestapi.azurewebsites.net/api/v1/Users/{{id_delete_neg}} <br>


**Ожидаемый результат**  код статуса 400 Bad Request<br>


**Заголовки запроса**<br>
````
User-Agent: PostmanRuntime/7.32.3
Accept: */*
Cache-Control: no-cache
Postman-Token: 8fe1fe42-7bf2-4430-8473-95d495a24a01
Host: fakerestapi.azurewebsites.net
Accept-Encoding: gzip, deflate, br
Connection: keep-alive
````

**Тело запроса**<br>
Отсутствует<br>


**Заголовок ответа**<br>
````
Content-Length: 0
Date: Fri, 23 Jun 2023 21:32:34 GMT
Server: Kestrel
api-supported-versions: 1.0
````
**Тело ответа**<br>

```{
    "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
    "title": "One or more validation errors occurred.",
    "status": 400,
    "traceId": "00-82e0b9c595686c488c0318b38eeb6754-ea4c1a4646f8da4a-00",
    "errors": {
        "id": [
            "The value '{id}' is not valid."
        ]
    }
}
```
