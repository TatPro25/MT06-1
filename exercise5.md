## Задание №5. 
## Знакомство с функционалом Swagger
\
___1. GET ​/api​/v1​/Activities___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
3. Заголовки запроса: accept: text/plain; v=1.0
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
  {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-21T20:17:04.7535621+00:00",
    "completed": false
  },
  {
    "id": 2,
    "title": "Activity 2",
    "dueDate": "2023-06-21T21:17:04.7535642+00:00",
    "completed": true
  }
```
___  

___2. POST​/api​/v1​/Activities___
1. HTTP-метод: POST
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
3. Заголовки запроса: "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса:
```
{
  "id":34,
  "title": "string",
  "dueDate": "2023-06-22T09:30:53.266Z",
  "completed": true
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 34,
  "title": "string",
  "dueDate": "2023-06-22T09:30:53.266Z",
  "completed": true
}
```
___

___3. POST ​/api​/v1​/Activities___
1. HTTP-метод: POST
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities
3. Заголовки запроса: "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id":08760,
  "title": "string",
  "dueDate": "2023-06-22T09:30:53.266Z",
  "completed": true
}
```
5. Статус-код ответа: 400
6. Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-404194a03ac45942a716bc8cb25605ac-92d36faccc11074a-00",
  "errors": {
    "$.id": [
      "Invalid leading zero before '8'. Path: $.id | LineNumber: 1 | BytePositionInLine: 8."
    ]
  }
}
```
___

___4. GET ​/api​/v1​/Activities​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/654
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 400
6. Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-2007b76ec3a72d439e0b173bc23128be-4c3731902e99864f-00"
}
```
___

___5. GET ​/api​/v1​/Activities​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/4
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа: 
```
{
  "id": 4,
  "title": "Activity 4",
  "dueDate": "2023-06-22T15:20:30.5141147+00:00",
  "completed": true
}
```
___

___6. PUT ​/api​/v1​/Activities​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/204
3. Заголовки запроса: "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-22T11:22:51.332Z",
  "completed": true
}
```
5. Статус-код ответа: 200
6. Тело ответа: 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-22T11:22:51.332Z",
  "completed": true
}
```
___

___7. PUT ​/api​/v1​/Activities​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/090909090909090
3. Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-22T11:22:51.332Z",
  "completed": true
}
```
5. Статус-код ответа: 400
6. Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-d2fef0d0c91e514994b14fbd9905437e-2ed46914b8469640-00",
  "errors": {
    "id": [
      "The value '090909090909090' is not valid."
    ]
  }
}
```
___

___8. DELETE ​/api​/v1​/Activities​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/32
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа: 
```
access-control-allow-origin: * 
 api-supported-versions: 1.0 
 content-length: 0 
 date: Thu22 Jun 2023 11:28:59 GMT 
 server: Kestrel 
```
___

___9. DELETE ​/api​/v1​/Activities​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/3245686912124
3. Заголовки запроса: https://fakerestapi.azurewebsites.net/api/v1/Activities/3245686912124
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 400
6. Тело ответа: 
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-9d8973a21dc76c4dabf2ec7a5929a5c6-46ba56221fc41e44-00",
  "errors": {
    "id": [
      "The value '3245686912124' is not valid."
    ]
  }
}
```
___

___10. GET ​/api​/v1​/Authors___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа: 
```
  {
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 2,
    "idBook": 1,
    "firstName": "First Name 2",
    "lastName": "Last Name 2"
  },
  {
    "id": 3,
    "idBook": 1,
    "firstName": "First Name 3",
    "lastName": "Last Name 3"
  }.... 
```
___

___11. POST​/api​/v1​/Authors___
1. HTTP-метод: POST
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса: "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" 
4. Тело запроса: 
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
___  

___12. POST​/api​/v1​/Authors___
1. HTTP-метод: POST
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса: "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" 
4. Тело запроса: 
```
{
  "id": 0456,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-2f10223a31140545bbcd4f5c54deaaa4-62cd6dee854f6a40-00",
  "errors": {
    "$.id": [
      "Invalid leading zero before '4'. Path: $.id | LineNumber: 1 | BytePositionInLine: 9."
    ]
  }
}
```
___  

___13. GET ​/api​/v1​/Authors​/authors​/books​/{idBook}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/256
3. Заголовки запроса: "accept: text/plain; v=1.0" 
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
отсутствует
```
___  

___14. GET ​/api​/v1​/Authors​/authors​/books​/{idBook}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/678963509317656
3. Заголовки запроса: "accept: text/plain; v=1.0" 
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c47a73312fd86b4ca157dd11fd108d20-057ced81d7bf4a43-00",
  "errors": {
    "idBook": [
      "The value '678963509317656' is not valid."
    ]
  }
}
```
___ 

___15. GET ​/api​/v1​/Authors​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/25
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 25,
  "idBook": 11,
  "firstName": "First Name 25",
  "lastName": "Last Name 25"
}
```
___ 

___16. GET ​/api​/v1​/Authors​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/-25
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 404
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-c7288f706309234381967d5ea62b64eb-6849d347c5a3c74f-00"
}
```
___ 

___17. GET ​/api​/v1​/Authors​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/38673365645624656
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-f57241230d79bb44ac9ebd387a354f4e-69b919da791fa344-00",
  "errors": {
    "id": [
      "The value '38673365645624656' is not valid."
    ]
  }
}
```
___  

___18. PUT ​/api​/v1​/Authors​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/123
3. Заголовки запроса: -H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
___  

___19. PUT ​/api​/v1​/Authors​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/12345678900987654321
3. Заголовки запроса: "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-8bbf185600cd014dbb6a82ebdd096e25-8bdf555d6f93c14b-00",
  "errors": {
    "id": [
      "The value '12345678900987654321' is not valid."
    ]
  }
}
```
___ 

___20. DELETE ​/api​/v1​/Authors​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/23432
3. Заголовки запроса:  "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
отсутствует
```
___ 

___21. DELETE ​/api​/v1​/Authors​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Authors/0957433241234
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-9d8bd739cd5c1d40af1256014490bf7d-5a03b310400ced4a-00",
  "errors": {
    "id": [
      "The value '0957433241234' is not valid."
    ]
  }
}
```
___ 

___22. GET ​/api​/v1​/Books___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
  {
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-21T12:02:54.7421853+00:00"
  },
  {
    "id": 2,
    "title": "Book 2",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 200,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-20T12:02:54.7421996+00:00"
  },
  {
    "id": 3,
    "title": "Book 3",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 300,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-19T12:02:54.7422103+00:00"
  }...
```
___  

___23. POS  ​/api​/v1​/Books___
1. HTTP-метод: POST
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books
3. Заголовки запроса: "accept: */*" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T12:05:18.519Z"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T12:05:18.519Z"
}
```
___ 

___24. GET ​/api​/v1​/Books​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/25
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 25,
  "title": "Book 25",
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "pageCount": 2500,
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "publishDate": "2023-05-28T12:08:01.1465859+00:00"
}
```
___

___25. GET ​/api​/v1​/Books​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/2534646
3. Заголовки запроса: "accept: text/plain; v=1.0" 
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 404
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-40bbd04132643941bb7048685d376a0f-50608a5302375b4e-00"
}
```
___  

___26. PUT ​/api​/v1​/Books​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/2
3. Заголовки запроса: "accept: */*" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T12:11:35.108Z"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T12:11:35.108Z"
}
```
___ 

___27. PUT ​/api​/v1​/Books​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/8765431234
3. Заголовки запроса: 
4. Тело запроса: 
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-22T12:11:35.108Z"
}
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-893d9c470356af429885101749485f60-07d195bedb1c9143-00",
  "errors": {
    "id": [
      "The value '8765431234' is not valid."
    ]
  }
}
```
___  

___28. DELETE ​/api​/v1​/Books​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Books/765
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
отсутствует
```
___  

___29. GET ​/api​/v1​/CoverPhotos___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  },
  {
    "id": 2,
    "idBook": 2,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"
  },
  {
    "id": 3,
    "idBook": 3,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 3&w=250&h=350"
  }...
```
___ 

___30. POST ​/api​/v1​/CoverPhotos___
1. HTTP-метод: POST
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. Заголовки запроса:  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
___

___31. GET ​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/345
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
отсутствует
```
___ 

___32. GET ​/api​/v1​/CoverPhotos​/books​/covers​/{idBook}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/675758435345
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c2e4d622d4a807409098ed80bd6038e7-c4694ca19036bc45-00",
  "errors": {
    "idBook": [
      "The value '675758435345' is not valid."
    ]
  }
}
```
___ 

___33. GET ​/api​/v1​/CoverPhotos​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/14
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 14,
  "idBook": 14,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 14&w=250&h=350"
}
```
___

___34. GET ​/api​/v1​/CoverPhotos​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/201
3. Заголовки запроса: "accept: text/plain; v=1.0"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 404
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-5a50c45c1483eb4da8ff29172864747b-fd5bf79eb7d33941-00"
}
```
___

___35. PUT ​/api​/v1​/CoverPhotos​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/25
3. Заголовки запроса: "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
___ 

___36. PUT ​/api​/v1​/CoverPhotos​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/8761249856
3. Заголовки запроса:  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" 
4. Тело запроса: 
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-8b9dfb855f34154fa4c7f404810b2ae9-6027a29d620afd4d-00",
  "errors": {
    "id": [
      "The value '8761249856' is not valid."
    ]
  }
}
```
___ 

___37. DELETE ​/api​/v1​/CoverPhotos​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/6
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
отсутствует
```
___ 

___38. DELETE ​/api​/v1​/CoverPhotos​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/1234567890098765432
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-4638b965b4b7524eaf89b32c377af946-fc2d0049549fd740-00",
  "errors": {
    "id": [
      "The value '1234567890098765432' is not valid."
    ]
  }
}
```
___

___39. GET ​/api​/v1​/Users___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
3. Заголовки запроса: "accept: text/plain; v=1.0" 
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
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
  {
    "id": 3,
    "userName": "User 3",
    "password": "Password3"
  }...
```
___ 

___40. POST ​/api​/v1​/Users___
1. HTTP-метод: POST
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users
3. Заголовки запроса: "accept: */*" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
___

___41. GET ​/api​/v1​/Users​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/10
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 10,
  "userName": "User 10",
  "password": "Password10"
}
```
___ 

___42. GET ​/api​/v1​/Users​/{id}___
1. HTTP-метод: GET
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/11
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 404 
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-6e5873813d2e53419efbbb9534329be5-76d80eb03e01344c-00"
}
```
___ 

___43. PUT ​/api​/v1​/Users​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/3
3. Заголовки запроса: "accept: */*" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа: 200
6. Тело ответа:
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
___ 

___44. PUT ​/api​/v1​/Users​/{id}___
1. HTTP-метод: PUT
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/9873465734354
3. Заголовки запроса: "accept: */*" -H  "Content-Type: application/json; v=1.0"
4. Тело запроса: 
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа: 400
6. Тело ответа:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-60d9cc05741cf64bb8d0f5b218e928bb-daac5ba4c1c1c145-00",
  "errors": {
    "id": [
      "The value '9873465734354' is not valid."
    ]
  }
}
```
___  

___45. DELETE ​/api​/v1​/Users​/{id}___
1. HTTP-метод: DELETE
2. Полный URL запроса: https://fakerestapi.azurewebsites.net/api/v1/Users/34
3. Заголовки запроса: "accept: */*"
4. Тело запроса: 
```
отсутствует
```
5. Статус-код ответа: 200
6. Тело ответа:
```
отсутствует
```
___
|Number|DELETE|Полный URL запроса|Заголовки запроса|Тело запроса|Статус-код ответа|Тело ответа|
|-|-|-|-|-|-|-|
|___45. DELETE ​/api​/v1​/Users​/{id}___|DELETE|https://fakerestapi.azurewebsites.net/api/v1/Users/34|"accept: */*"|отсутствуета|200|<li> {<li>"id": 1,<li>"title":"Activity 1",<li> "dueDate": "2023-06-04T16:13:49.273778+00:00",<li>"completed": **false**<li> }|
|___45. DELETE ​/api​/v1​/Users​/{id}___|DELETE|https://fakerestapi.azurewebsites.net/api/v1/Users/34|"accept: */*"|отсутствуета|200|<li> {<li>"id": 1,<li>"title":"Activity 1",<li> "dueDate": "2023-06-04T16:13:49.273778+00:00",<li>"completed": **false**<li> }|