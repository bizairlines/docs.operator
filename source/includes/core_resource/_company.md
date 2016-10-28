# Companies
## Update
> `GET /v1/companies/{company_id}`

```shell
$ curl '/v1/companies/{$company_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d name='My Jet Company' \
    -d contact_name='John Doe'
```

> Example Response

```
{
  "data": {
    "id": "a84d8855-da27-4c4a-99fe-fab2f2bccf8b",
    "airline": {
      "id": 628,
      "name": "My Jet Company",
      "category": "charter-operator",
      "iata_code": "APP",
      "icao_code": null,
      "created_at": "2016-10-28 13:43:40",
      "updated_at": "2016-10-28 13:43:40"
    },
    "country": null,
    "name": "My Jet Company",
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
    "contact_name": "John Doe",
    "contact_phone": null,
    "contact_email": null,
    "is_active": true,
    "is_airline": false,
    "is_operator": true,
    "created_at": "2016-10-28 13:04:18",
    "updated_at": "2016-10-28 13:55:39"
  }
}
```

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
