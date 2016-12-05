# Security
## Create account

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

### HTTP REQUEST
`POST /v1/security/account/operator`

### DEFINITION
Creates an account for operators.

During this moment a fantasy company is created.

| Parameter     | Required | Description                                               | Format |
|---------------|----------|-----------------------------------------------------------|--------|
| email         | *yes*    | The user’s email address that will also be used as login. | string |
| password      | *yes*    | Secure password.                                          | string |
| first_name    | *yes*    | User's first name.                                        | string |
| last_name     | *yes*    | User's last name.                                         | string |
| country       | *no*     | Country ISO CODE 2 based on a [country list](#countries). | string |
| phone         | *no*     | User's phone.                                             | string |

## Login

```shell
$ curl -XPOST '/v1/security/login/app' \
    -H 'Content-type: application/json' \
    -d email='john@doe.com' \
    -d password='secure password'
```

> Example Response

```
{
  "data": {
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...",
    "user": {
      "id": "3f084a13-c0f4-428e-a80e-04647674ced4",
      "country": null,
      "avatar": {
        "id": "3cb8249c-2fba-4a24-b09c-d6ac6ca84a3d",
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1.png",
        "name": "company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1",
        "mimetype": "image/jpeg",
        "size": 328043,
        "extension": "jpeg",
        "is_active": true,
        "created_at": "2016-12-04 23:32:04",
        "updated_at": "2016-12-04 23:32:04"
      },
      "email": "kyle@gmail.com",
      "first_name": "Kyle",
      "last_name": "House",
      "phone": null,
      "company_position": null,
      "is_active": true,
      "created_at": "2016-11-08 08:41:35",
      "updated_at": "2016-12-04 23:32:04",
      "address": [],
      "company": [
        {
          "id": "3fa978cf-efb9-4072-8251-6d36f05a92ad",
          "airline": {
            "id": 631,
            "name": "My Jet Company",
            "category": "charter-operator",
            "iata_code": "XP",
            "icao_code": "XPT",
            "created_at": "2016-11-08 08:43:06",
            "updated_at": "2016-11-08 08:43:06"
          },
          "country": {
            "id": 234,
            "name": "United States",
            "iso_code_2": "US",
            "iso_code_3": "USA",
            "area_code": "1",
            "order": 3,
            "created_at": "2016-08-03 21:17:21",
            "updated_at": "2016-08-03 21:17:21"
          },
          "logo": {
            "id": "169e9890-10af-41c1-b511-0b2a5a20428d",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/gmykmx08z6fui4pnhe7u.png",
            "name": "company/51-my-jet-company/gmykmx08z6fui4pnhe7u",
            "mimetype": "image/png",
            "size": 195234,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-25 00:26:00",
            "updated_at": "2016-11-25 00:26:00"
          },
          "thumbnail": {
            "id": "c8fdb2c6-6637-47eb-a0ce-664a22f13f02",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1.png",
            "name": "company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:42:47",
            "updated_at": "2016-11-08 08:42:47"
          },
          "name": "My Jet Company",
          "legal_name": null,
          "registration_number": null,
          "site": "www.my-jet-company.com",
          "phone": "12121212",
          "address_1": "Miami International Airport, Northwest 25th Street, Miami, FL, United States",
          "address_2": "",
          "city": "Miami",
          "state": "Florida",
          "zipcode": "33142",
          "bank_info": null,
          "contact_info": null,
          "contact_name": "My Jet Company",
          "contact_phone": "",
          "contact_email": "",
          "is_active": true,
          "is_airline": false,
          "is_operator": true,
          "has_entered_iata": true,
          "created_at": "2016-11-08 08:41:35",
          "updated_at": "2016-11-25 00:26:00"
        }
      ],
      "card": [],
      "permission": [
        {
          "permission": "admin",
          "system": {
            "name": "Charter Operator Tool",
            "slug": "charter-operator-tool",
            "description": null
          }
        }
      ],
      "is_complete": false
    }
  }
}
```

### HTTP REQUEST
`POST /v1/security/login/operator`

### DEFINITION
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
`POST /v1/security/password/reset`

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
`PUT /v1/security/password/reset`

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
