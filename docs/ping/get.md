# Ping

Check the api status

**URL** : `/ping`

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
    data: {
        timestamp: Number,
        uptime: Number,
        application: {
            name: String,
            version: String,
            env: String,
            pid: Number,
            versions: {
                http_parser: String,
                node: String,
                v8: String,
                ares: String,
                uv: String,
                zlib: String,
                modules: String,
                openssl: String
            }
            dependencies: Record<string, string>
        },
        memory: {
            rss: Number,
            heapTotal: Number,
            heapUsed: Number,
            external: Number,
            arrayBuffers: Number
        },
        system: {
            arch: String,
            platform: String,
            type: String,
            release: String,
            hostname: String,
            uptime: Number,
            cores: Number,
            memory: Number
        }
    }
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