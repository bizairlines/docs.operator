# Users
## Get
```
GET /v1/users/{id}
```
```shell
$ curl '/v1/users/{$id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

Retrieve an user information, such as company, country and address.

## Update
```
PUT /v1/users/{$id}
```
```shell
$ curl -XPUT '/v1/users/{$id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d first_name=John \
    -d last_name=Doe \
    -d country_id=100 \
    -d phone='+55 61 991560000' \
    -d hourly_salary=2000
```

<aside class="notice">
It's not necessary to send all the parameters in the same request.
</aside>

| Parameter        | Description                                               | Format |
|------------------|-----------------------------------------------------------|--------|
| first_name       | User's first name.                                        | string |
| last_name        | User's last name.                                         | string |
| country_id       | Country ID based on a [country list](#countries).         | int    |
| phone            | User's phone.                                             | string |
| hourly_salary    | User's hourly salary (USD).                               | float  |

## Delete
```
DELETE /v1/users/{$id}
```
```shell
$ curl -XDELETE '/v1/users/{$id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

Delete user's account.

## Avatar
```
POST /v1/users/{$id}/avatar
```
```shell
$ curl -XPOST '/v1/users/{$id}/avatar' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -F 'image=@/path/to/pictures/picture.jpg'
```

| Parameter | Required | Description                      | Format |
|-----------|----------|----------------------------------|--------|
| image     | *yes*    | A valid **PNG** or **JPG** file. | binary |

## Change password
```
PUT /v1/users/{$id}/password
```
```shell
$ curl -XPUT '/v1/users/{$id}/password' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d password='secure password'
```

| Parameter | Required | Description      | Format |
|-----------|----------|------------------|--------|
| password  | *yes*    | Secure password. | string |
