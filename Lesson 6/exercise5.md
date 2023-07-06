### Activities

1. GET ​/api​/v1​/Activities
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
[
  {
    "id": 0,
    "title": "string",
    "dueDate": "2023-06-13T11:33:03.961Z",
    "completed": true
  }
]
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
[{
    "id": 30,
    "title": "Activity 30",
    "dueDate": "2023-06-14T17:33:01.961934+00:00",
    "completed": true
  }
]
```</td>
		</tr>
	</tbody>
</table>

2. POST ​/api​/v1​/Activities УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: application/json; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-13T10:08:56.335Z",
  "completed": true
```}</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-13T10:08:56.335Z",
  "completed": true
}
```</td>
		</tr>
	</tbody>

</table>

3. POST ​/api​/v1​/Activities НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: application/json; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 52523666666,
  "title": "string",
  "dueDate": "2023-06-13T10:08:56.335Z",
  "completed": true
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Error: Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c27332d212a7104f95c88cace22c3359-43ae579d1977694e-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 17."
    ]
  }
}
```</td>
		</tr>
	</tbody>

</table>

4. GET /api​/v1​/Activities​/{32}  НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities/32</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-13T11:41:52.071Z",
  "completed": true
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>404 Error: Not Found</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-1e1c2d8eb39870429f3e4edd2faded33-5c9c17ed6e0a5f49-00"
}
```</td>
		</tr>
	</tbody>
</table>

5. GET /api​/v1​/Activities​/{4} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities/4</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>-</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
[{
  "id": 4,
  "title": "Activity 4",
  "dueDate": "2023-06-13T15:40:47.4477499+00:00",
  "completed": true
}]
```</td>
		</tr>
	</tbody>
</table>

6. PUT /api​/v1​/Activities​/{3298798798535} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities/3298798798535</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Error: Not Found</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-9a679991fd7df141978f4cf4a388b36b-96c00d9297dd2146-00",
  "errors": {
    "id": [
      "The value '3298798798535' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>

7. PUT /api​/v1​/Activities​/{5} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities/5</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: application/json; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>-</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-13T11:43:14.247Z",
  "completed": true
}
```</td>
		</tr>
	</tbody>

</table>

8. DELETE  /api​/v1​/Activities​/{1} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>DELETE

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities/1</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200  Success </td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```-
```</td>
		</tr>
	</tbody>
</table>

9. DELETE
​/api​/v1​/Activities​/{2626262626} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Activities/2626262626</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-677b74899341114f99595c63057d436e-9df1e5b7fd63534e-00",
  "errors": {
    "id": [
      "The value '2626262626' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


### Authors

10. GET
​/api​/v1​/Authors
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>-</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
```</td>
		</tr>
	</tbody>
</table>


11. POST
​/api​/v1​/Authors УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
		</tr>
	</tbody>
</table>



12. POST
​/api​/v1​/Authors НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 0000000000,
  "idBook": 0,
  "firstName": "ybyftn",
  "lastName": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Error: Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-68280b62313d414c8dc98a6fb02ed30f-bef83f7a46475343-00",
  "errors": {
    "$.id": [
      "Invalid leading zero before '0'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


13. GET
​/api​/v1​/Authors​/authors​/books​/{56} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/56</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
[
  {
    "id": 166,
    "idBook": 56,
    "firstName": "First Name 166",
    "lastName": "Last Name 166"
  },
  {
    "id": 167,
    "idBook": 56,
    "firstName": "First Name 167",
    "lastName": "Last Name 167"
  }
]
```</td>
		</tr>
	</tbody>
</table>

14. GET
​/api​/v1​/Authors​/authors​/books​/{23255452454545454252454} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/23255452454545454252454</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-bcbdf1760c6d7348a0d8ed4ef00181bf-0589ad5a7671854a-00",
  "errors": {
    "idBook": [
      "The value '23255452454545454252454' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>

15. GET
​/api​/v1​/Authors​/{77} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/77</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 77,
  "idBook": 26,
  "firstName": "First Name 77",
  "lastName": "Last Name 77"
}
```</td>
		</tr>
	</tbody>
</table>

16. GET
​/api​/v1​/Authors​/{77777777777777777} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/77777777777777777</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-e59350e8456da2419b23eae266b802fc-564f7dfef7f06342-00",
  "errors": {
    "id": [
      "The value '77777777777777777' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


17. PUT
​/api​/v1​/Authors​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td> PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/59</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
		</tr>
	</tbody>
</table>

18. PUT
​/api​/v1​/Authors​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/59</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-5b0f917eba93f244b81f5ce8ad7fa033-51280d921ff72a4c-00",
  "errors": {
    "id": [
      "The value '5959595959595959' is not valid."
    ]
  }
}
````</td>
		</tr>
	</tbody>
</table>

19. 
DELETE
​/api​/v1​/Authors​/{19} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td> DELETE

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/19</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
-
```</td>
		</tr>
	</tbody>
</table>

20. DELETE
​/api​/v1​/Authors​/{id}{1919191919191919191} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/1919191919191919191</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-459b2372b8f39a4184d92dd79926384f-e6e956e214f18146-00",
  "errors": {
    "id": [
      "The value '1919191919191919191' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


### Books

21. GET
​/api​/v1​/Books
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>Authors</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>-</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  },
```</td>
		</tr>
	</tbody>
</table>


22. POST
​/api​/v1​/Books УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```</td>
		</tr>
	</tbody>
</table>



23. POST
​/api​/v1​/Books НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 5252525252,
  "idBook": 0,
  "url": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Error: Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-5f103899e4929e4198cc805c4551edd2-2f8e7fc3e68e0a47-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 16."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


24. GET
​/api​/v1​/Books​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books/96</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 96,
  "title": "Book 96",
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "pageCount": 9600,
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "publishDate": "2023-03-09T18:16:36.6238386+00:00"
}
```</td>
		</tr>
	</tbody>
</table>

25. GET
​/api​/v1​/Books​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books/9696969696969</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-e76160d1b86c5c4cac809b6c21a5213d-efa14c01f0f4294a-00",
  "errors": {
    "id": [
      "The value '9696969696969' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


26. GET
​/api​/v1​/Users​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users/8748748748745</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-679be38db58fed45adcdb69ce2230ad0-6115e7147af59147-00",
  "errors": {
    "id": [
      "The value '8748748748745' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


27. GET
​/api​/v1​/Users​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users/874</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-3a771ff949c3e242aa6835b603dd46ea-300aa7f38df77041-00"
}
```</td>
		</tr>
	</tbody>
</table>//*//

28. PUT
​/api​/v1​/Books​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td> PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books/36</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```{
 {
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-13T18:20:27.861Z"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-13T18:20:27.861Z"
}
```</td>
		</tr>
	</tbody>
</table>

29. PUT
​/api​/v1​/Books​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books/3636363617</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
"accept: */*" -H  "Content-Type: application/json; v=1.0"
```</td>
		</tr>
	</tbody>
</table>

30. 
DELETE
​/api​/v1​/Books​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td> DELETE

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books/15</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
-
```</td>
		</tr>
	</tbody>
</table>

31. DELETE
​/api​/v1​/Books​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Books/15151515156</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-9ed139e6de016a418c174e3048696fdb-89f1d1d035ffcd48-00",
  "errors": {
    "id": [
      "The value '15151515156' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>



### CoverPhotos

32. GET
​/api​/v1​/CoverPhotos
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>-</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  }
```</td>
		</tr>
	</tbody>
</table>


33.POST
​/api​/v1​/CoverPhotos УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```</td>
		</tr>
	</tbody>
</table>



34. POST
​/api​/v1​/CoverPhotos НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>POST

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```
{
  "id": 5252525252,
  "idBook": 0,
  "url": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Error: Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-263049e850109842af7c517569bdd0b0-8b6a105de9f5c24c-00",
  "errors": {
    "$.id": [
      "The JSON value could not be converted to System.Int32. Path: $.id | LineNumber: 0 | BytePositionInLine: 16."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


35. GET
​/api​/v1​/CoverPhotos​/books​/covers​/{idBook} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/56</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
[
  {
    "id": 166,
    "idBook": 56,
    "firstName": "First Name 166",
    "lastName": "Last Name 166"
  },
  {
    "id": 167,
    "idBook": 56,
    "firstName": "First Name 167",
    "lastName": "Last Name 167"
  }
]
```</td>
		</tr>
	</tbody>
</table>

36. GET
​/api​/v1​/CoverPhotos​/books​/covers​/{idBook} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/23255452454545454252454</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-bcbdf1760c6d7348a0d8ed4ef00181bf-0589ad5a7671854a-00",
  "errors": {
    "idBook": [
      "The value '23255452454545454252454' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>

37. GET
​/api​/v1​/Authors​/{77} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/77</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 77,
  "idBook": 26,
  "firstName": "First Name 77",
  "lastName": "Last Name 77"
}
```</td>
		</tr>
	</tbody>
</table>

38. GET
​/api​/v1​/Authors​/{77777777777777777} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/77777777777777777</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-e59350e8456da2419b23eae266b802fc-564f7dfef7f06342-00",
  "errors": {
    "id": [
      "The value '77777777777777777' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>


39. PUT
​/api​/v1​/Authors​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td> PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/59</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
		</tr>
	</tbody>
</table>

40. PUT
​/api​/v1​/Authors​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>PUT

</td>
	</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/59</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```</td>
	    </tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
		<td>```{
 "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-5b0f917eba93f244b81f5ce8ad7fa033-51280d921ff72a4c-00",
  "errors": {
    "id": [
      "The value '5959595959595959' is not valid."
    ]
  }
}
```</td>
	</tr>
	</tbody>
</table>

41. 
DELETE
​/api​/v1​/Authors​/{19} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td> DELETE

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/19</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
-
```</td>
		</tr>
	</tbody>
</table>

42. DELETE
​/api​/v1​/Authors​/{id}{1919191919191919191} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Authors/1919191919191919191</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-459b2372b8f39a4184d92dd79926384f-e6e956e214f18146-00",
  "errors": {
    "id": [
      "The value '1919191919191919191' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>



43. GET
​/api​/v1​/Users
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
  }
```</td>
		</tr>
	</tbody>
</table>

44. POST
​/api​/v1​/Users УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: */*" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```</td>
		</tr>
	</tbody>
</table>

45. PUT
​/api​/v1​/Users​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users/48924846848</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-88f421cc7000274297d469c59dd74024-6fa135a45726f646-00",
  "errors": {
    "id": [
      "The value '48924846848' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>

46. PUT
​/api​/v1​/Users​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>PUT

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users/83</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```</td>
		</tr>
	</tbody>
</table>

47. 
DELETE
​/api​/v1​/Users​/{id} УСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td> DELETE

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users/37</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td>"accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>200 Success</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
-
```</td>
		</tr>
	</tbody>
</table>

48. DELETE
​/api​/v1​/Users​/{id} НЕУСПЕШНЫЙ
<table>
	<tbody>
		<tr>
			<td>HTTP метод
</td>
			<td>GET

</td>
		</tr>
		<tr>
			<td>Полный URL запроса
</td>
			<td>https://fakerestapi.azurewebsites.net/api/v1/Users/37373737456</td>
		</tr>
		<tr>
			<td>Заголовки запроса</td>
			<td> "accept: */*"</td>
		</tr>
		<tr>
			<td>Тело запроса</td>
			<td>```-
```</td>
		</tr>
		<tr>
			<td>Статус-код ответа</td>
			<td>400 Bad Request</td>
		</tr>
		<tr>
			<td>Тело ответа</td>
			<td>```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-9cd5ad42031cb54b895a6dec8fb315a1-0ed87ce34146c747-00",
  "errors": {
    "id": [
      "The value '37373737456' is not valid."
    ]
  }
}
```</td>
		</tr>
	</tbody>
</table>
