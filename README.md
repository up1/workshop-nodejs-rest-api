# Workshop develop RESTful APIs with NodeJS
* [express](https://github.com/expressjs/express)
* [axios](https://github.com/axios/axios)
* [node postgres](https://node-postgres.com/)
* testing
  * [Postman](https://www.postman.com/)
  * [newman](https://github.com/postmanlabs/newman)
  * [jest](https://jestjs.io/)
  * [supertest](https://github.com/ladjs/supertest)
  * [nock](https://github.com/nock/nock)

## Create project
```
$npm init
$npm i -S express axios pg jest supertest nock
```

## Design RESTful APIs
| Endpoint    | Description | Request body | Response Status Code | Response body |
| ----------- | ----------- | ------------ | -------------------- | ------------- |
| GET /users | Get all users | - | 200 | ```[{"id", 1, "name": "demo", "email": "demo email"}]``` |
| GET /users/:id | Get user by id | - | 200  | ```{"id", 1, "name": "demo", "email": "demo email"}``` |
| POST /users | Create new user | - | 201  | ```{"message": "User created"}``` |
| POST /users | Create new user | - | 409  | ```{"message": "User name duplicated"}``` |

