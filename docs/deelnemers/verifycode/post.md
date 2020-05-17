# Verify Code

**URL** : `/deelnemers/verify-code`

**Method** : `POST`

**Auth required** : NO

**Request body** :
```js
{
    email: String;
    code: String;
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