# Auth

**URL** : `/auth/login`

**Method** : `POST`

**Auth required** : NO

**Request body** :
```js
{
    email: String,
    password: String
}
```

## Success Response

**Code** : `200 OK`

**Content return types** :

```js
{
    statusCode: Number,
    statusMessage: String,
    message: String,
    data: {
        token: String,
        user: {
            sid: String,
            firstname: String,
            lastname: String,
            email: String,
            type: String,
            avatar: String,
            createdAt: Date,
            // Client specific properties
            code?: String,
            totalGoals?: Number,
            achievedGoals?: Number,
            finalGoal?: String,
            jobcoach?: String,
            feedbackType?: String,
            goals?: Array<String>,
            active?: Boolean
        }
    }
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

**Condition** : User doesn't exist.

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