# Index

List of api routes

**URL** : `/`

**Method** : `GET`

**Auth required** : NO

## Success Response

**Code** : `200 OK`

**Content return types**

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String,
    data: Array<String>
}

```

## Error Response

**Condition** : If something server-side goes wrong.

**Code** : `500 Internal Server Error`

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String,
    error?: String
}
```