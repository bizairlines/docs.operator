# Security
## Create account
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
