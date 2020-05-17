# Jobcoaches

**URL** : `/jobcoaches/all`

**Method** : `GET`

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
    message: String,
    data: [
        {
            sid: String,
            firstname: String,
            lastname: String,
            email: String,
            type: String,
            avatar: String,
            createdAt: Date
        },
        ...
    ]
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