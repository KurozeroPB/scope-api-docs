# Jobcoaches

**URL** : `/jobcoaches/:id`

**Method** : `PATCH`

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

**Condition** : When the requested user doesn't exist.

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String
}
```

**Code** : `401 Unauthorized`

**Condition** : When a user tries to edit someone else.

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