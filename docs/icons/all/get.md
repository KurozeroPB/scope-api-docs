# Icons

**URL** : `/icons/all`

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
            name: String,
            pack: String,
            slug: String,
            // if pack = fad :
            colors?: {
                primary: String,
                primaryOpacity: Number,
                secondary: String,
                secondaryOpacity: Number
            }
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