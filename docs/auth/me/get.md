# Auth

**URL** : `/auth/me`

**Method** : `GET`

**Auth required** : YES
```json
{
    "Authorization": "Bearer <token>"
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