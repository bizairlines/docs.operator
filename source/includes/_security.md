# Security
## App account
> `POST /v1/security/account`

```shell
$ curl -XPOST '/v1/security/account' \
    -H 'Content-type: application/json' \
    -d email='john@doe.com' \
    -d password='secure password' \
    -d first_name=John \
    -d last_name=Doe \
    -d country_id=100
```

| Parameter     | Required | Description                                               | Format |
|---------------|----------|-----------------------------------------------------------|--------|
| email         | *yes*    | The user’s email address that will also be used as login. | string |
| password      | *yes*    | Secure password.                                          | string |
| first_name    | *yes*    | User's first name.                                        | string |
| last_name     | *yes*    | User's last name.                                         | string |
| country_id    | *yes*    | Country ID based on a [country list](#countries).         | int    |
| phone         | *no*     | User's phone.                                             | string |
| hourly_salary | *no*     | User's hourly salary (USD).                               | float  |

## Operator account
> `POST /v1/security/account/operator`

```shell
$ curl -XPOST '/v1/security/account/operator' \
    -H 'Content-type: application/json' \
    -d email='john@doe.com' \
    -d password='secure password' \
    -d first_name=John \
    -d last_name=Doe
```

> Example Response

```
{
  "data": {
    "email": "john@doe.com",
    "first_name": "John",
    "last_name": "Doe",
    "phone": null,
    "hourly_salary": "0.00",
    "updated_at": "2016-10-27 18:25:14",
    "created_at": "2016-10-27 18:25:14",
    "id": "3d86db25-c2c8-4b27-9040-fa50b41905bb",
    "is_active": false,
    "address": [],
    "company": [
      {
        "id": "a8d944d9-8963-4f58-abeb-17f8651566db",
        "company_name": null,
        "legal_name": null,
        "registration_number": null,
        "site": null,
        "phone": null,
        "address_1": null,
        "address_2": null,
        "city": null,
        "state": null,
        "zipcode": null,
        "bank_info": null,
        "contact_info": null,
        "is_active": false,
        "created_at": "2016-10-27 18:25:14",
        "updated_at": "2016-10-27 18:25:14"
      }
    ],
    "card": [],
    "permission": [],
    "is_complete": false
  }
}
```

Creates an account for operators.

During this moment a fantasy company is created.

| Parameter     | Required | Description                                               | Format |
|---------------|----------|-----------------------------------------------------------|--------|
| email         | *yes*    | The user’s email address that will also be used as login. | string |
| password      | *yes*    | Secure password.                                          | string |
| first_name    | *yes*    | User's first name.                                        | string |
| last_name     | *yes*    | User's last name.                                         | string |
| country_id    | *no*     | Country ID based on a [country list](#countries).         | int    |
| phone         | *no*     | User's phone.                                             | string |
| hourly_salary | *no*     | User's hourly salary (USD).                               | float  |

## Login
> `POST /v1/security/login/app`

```
{
    "email": "name@tld.com",
    "password": "111111"
}
```
```shell
$ curl -XPOST '/v1/security/login/app' \
    -H 'Content-type: application/json' \
    -d email='john@doe.com' \
    -d password='secure password'
```

Check sent credentials, authenticate a user and return a valid token and user object.

| Parameter | Required | Description               | Format |
|-----------|----------|---------------------------|--------|
| email     | *yes*    | The user’s email address. | string |
| password  | *yes*    | Registered password.      | string |

## Reset password
The reset password contains two steps process:

1. Generate and send a 6 digit code;
2. Reset password.

### Generate code
> `POST /v1/security/password/reset`

```shell
$ curl -XPOST '/v1/security/password/reset' \
    -H 'Content-type: application/json' \
    -d email='john@doe.com'
```

Generate a 6 digit code that allows the user to reset the password.

This code is valid for 1 day and will be sent to a registered email.

| Parameter | Required | Description               | Format |
|-----------|----------|---------------------------|--------|
| email     | *yes*    | The user’s email address. | string |

### Reset password
> `PUT /v1/security/password/reset`

```shell
$ curl -XPUT '/v1/security/password/reset' \
    -H 'Content-type: application/json' \
    -d token='123456' \
    -d password='your-password' \
    -d password_confirm='your-password' \
    -d email='john@doe.com'
```

With the 6 digit code sent to the email, the user now is authorized to reset his password.

| Parameter        | Required | Description                        | Format |
|------------------|----------|------------------------------------|--------|
| email            | *yes*    | The user’s email address.          | string |
| token            | *yes*    | 6 digit code sent to user's email. | string |
| password         | *yes*    | Secure password.                   | string |
| password_confirm | *yes*    | Secure password confirmation.      | string |
