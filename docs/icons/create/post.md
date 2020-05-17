# Icons

**URL** : `/icons/create`

**Method** : `POST`

**Auth required** : YES
```json
{
    "Authorization": "Bearer <token>"
}
```

**Request body** :
```js
{
    name: String,
    pack: String,
    slug: String,
    colors?: {
        primary: String,
        primaryOpacity: Number,
        secondary: String,
        secondaryOpacity: Number
    }
}
```

## Success Response

**Code** : `200 OK`

**Content return types** :

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

**Code** : `403 Forbidden`

**Condition** : When an unauthorized user tries to create an icon.

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String
}
```

**Code** : `400 Bad Request`

**Condition** : Bad request body.

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String
}
```