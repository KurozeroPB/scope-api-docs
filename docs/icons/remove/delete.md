# Icons

**URL** : `/icons/:id/remove`

**Method** : `DELETE`

**Auth required** : YES
```json
{
    "Authorization": "Bearer <token>"
}
```

## Success Response

**Code** : `200 OK`

**Content return types**

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String
}
```

## Error Response

**Code** : `500 Internal Server Error`

**Condition** : If something server-side goes wrong.

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String,
    error?: String
}
```

**Code** : `404 Not Found`

**Condition** : When the requested icon doesn't exist.

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String
}
```

**Code** : `400 Bad Request`

**Condition** : Bad request.

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String
}
```