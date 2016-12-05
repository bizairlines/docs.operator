# Companies
## Show company

```shell
$ curl '/v1/companies/{$company_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example Response

```
{
  "data": {
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
}
```

### HTTP REQUEST
`GET /v1/companies/{company_id}`

### DEFINITION
Get the company's public information.

## Update company

```shell
$ curl -XPUT '/v1/companies/{$company_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d name='My Jet Company' \
    -d contact_name='John Doe'
```

> Example Response

```
{
  "data": {
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
}
```

### HTTP REQUEST
`PUT /v1/companies/{company_id}`

### DEFINITION
Update the company's public information.

| Parameter           | Required | Description                                               | Format |
|---------------------|----------|-----------------------------------------------------------|--------|
| name                | *yes*    | Company name.                                             | string |
| country             | *no*     | Country ISO CODE 2 based on a [country list](#countries). | string |
| legal_name          | *no*     |                                                           | string |
| registration_number | *no*     |                                                           | string |
| site                | *no*     |                                                           | string |
| phone               | *no*     |                                                           | string |
| address_1           | *no*     |                                                           | string |
| address_2           | *no*     |                                                           | string |
| city                | *no*     |                                                           | string |
| state               | *no*     |                                                           | string |
| zipcode             | *no*     |                                                           | string |
| bank_info           | *no*     |                                                           | string |
| contact_info        | *no*     |                                                           | string |
| contact_name        | *no*     |                                                           | string |
| contact_phone       | *no*     |                                                           | string |
| contact_email       | *no*     |                                                           | string |

## Upload standard image

```shell
$ curl -XPOST '/v1/companies/{$company_id}/uploads/standard' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"image":"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABG4AAAS4CAYAAABGqo...}"'
```

> Example response

```
{
  "data" : {
    "id": "c8fdb2c6-6637-47eb-a0ce-664a22f13f02",
    "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1.png",
    "name": "company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1",
    "mimetype": "image/png",
    "size": 5012,
    "extension": "png",
    "is_active": true,
    "created_at": "2016-11-08 08:42:47",
    "updated_at": "2016-11-08 08:42:47"
  }
}
```

### HTTP REQUEST
`POST /v1/companies/{company_id}/uploads/standard`

### DEFINITION
Uploads the primary image for the company.

Requirements:

* Min width: 100px;
* Min height: 100px;
* Max image size: 1Mb;
* Allowed extensions: `jpeg`, `jpg`, `gif` and `png`;

## Upload small image

```shell
$ curl -XPOST '/v1/companies/{$company_id}/uploads/small' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"image":"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABG4AAAS4CAYAAABGqo...}"'
```

> Example response

```
{
  "data" : {
    "id": "c8fdb2c6-6637-47eb-a0ce-664a22f13f02",
    "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1.png",
    "name": "company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1",
    "mimetype": "image/png",
    "size": 5012,
    "extension": "png",
    "is_active": true,
    "created_at": "2016-11-08 08:42:47",
    "updated_at": "2016-11-08 08:42:47"
  }
}
```

### HTTP REQUEST
`POST /v1/companies/{company_id}/uploads/small`

### DEFINITION
Uploads the secondary image for the company.

Requirements:

* Ratio 1:1 (square);
* Min width: 100px;
* Min height: 100px;
* Max image size: 500Kb;
* Allowed extensions: `jpeg`, `jpg`, `gif` and `png`;

## Delete standard image

```shell
$ curl -XDELETE '/v1/companies/{$company_id}/uploads/standard' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data" : {
    "id": "c8fdb2c6-6637-47eb-a0ce-664a22f13f02",
    "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1.png",
    "name": "company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1",
    "mimetype": "image/png",
    "size": 5012,
    "extension": "png",
    "is_active": true,
    "created_at": "2016-11-08 08:42:47",
    "updated_at": "2016-11-08 08:42:47"
  }
}
```

### HTTP REQUEST
`DELETE /v1/companies/{company_id}/uploads/standard`

### DEFINITION
Removes company's standard image.

## Delete small image

```shell
$ curl -XDELETE '/v1/companies/{$company_id}/uploads/small' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data" : {
    "id": "c8fdb2c6-6637-47eb-a0ce-664a22f13f02",
    "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1.png",
    "name": "company/51-my-jet-company/hqhrsfjsu4q7vew1dpi1",
    "mimetype": "image/png",
    "size": 5012,
    "extension": "png",
    "is_active": true,
    "created_at": "2016-11-08 08:42:47",
    "updated_at": "2016-11-08 08:42:47"
  }
}
```

### HTTP REQUEST
`DELETE /v1/companies/{company_id}/uploads/small`

### DEFINITION
Removes company's small image.
