# Scope API

Base api url [`kurozeropb.info/scope/api`](https://kurozeropb.info/scope/api) (Will change later)

## Endpoints

### Auth
* [login](auth/login/post.md) : `POST /auth/login`
* [me](auth/me/get.md) : `GET /auth/me`

### Deelnemers
* [activate](deelnemers/activate/post.md) : `POST /deelnemers/activate`
* [all](deelnemers/all/get.md) : `GET /deelnemers/all`
* [create](deelnemers/create/post.md) : `POST /deelnemers/create`
* [id](deelnemers/id/get.md) : `GET /deelnemers/:id`
* [id](deelnemers/id/patch.md) : `PATCH /deelnemers/:id`
* [verify-code](deelnemers/verifycode/post.md) : `POST /deelnemers/verify-code`

### Icons
* [all](icons/all/get.md) : `GET /icons/all`
* [create](icons/create/post.md) : `POST /icons/create`
* [id](icons/id/get.md) : `GET /icons/:id`
* [remove](icons/remove/delete.md) : `DELETE /icons/:id/remove`

### Jobcoaches
* [all](jobcoaches/all/get.md) : `GET /jobcoaches/all`
* [create](jobcoaches/create/post.md) : `POST /jobcoaches/create`
* [id](jobcoaches/id/get.md) : `GET /jobcoaches/:id`
* [id](jobcoaches/id/patch.md) : `PATCH /jobcoaches/:id`

### Miscellaneous
* [ping](ping/get.md) : `GET /ping`
* [index](get.md) : `GET /`