## Airlines
### List/Table
> `GET /v1/airlines`

```shell
$ curl '/v1/airlines' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d sort='name'
    -d order='desc'
    -d page=2
```

> Example Response

```
{
  "total": 8108,
  "per_page": 20,
  "current_page": 3,
  "last_page": 406,
  "next_page_url": "[::protocol]://[::domain]:[::port]/v1/airports?page=4",
  "prev_page_url": "[::protocol]://[::domain]:[::port]/v1/airports?page=2",
  "prev_page_url": null,
  "from": 1,
  "to": 20,
  "data": [
    {
      "id": 1,
      "name": "Aer Lingus",
      "category": "airline",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    }
  ]
}
```

| Parameter | Required | Description                                                                               | Format  |
|-----------|----------|-------------------------------------------------------------------------------------------|---------|
| page      | *no*     | The number of the page.                                                                   | integer |
| sort      | *no*     | The column to sort the information. Default: `id`.                                        | integer |
| order     | *no*     | The direction to do the sorting. Available only `asc` and `desc` options. Default: `asc`. | integer |

### Autocomplete
> `GET /v1/airlines/autocomplete`

```shell
$ curl '/v1/airlines/autocomplete' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d s='aero' \
    -d category[]='jet-shuttle' \
    -d category[]='charter-operator'
```

> Example response

```
{
  "data": [
    {
      "id": 143,
      "name": "Aero Charter",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 144,
      "name": "Aero Jet Services",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 145,
      "name": "Aerodynamics Malaga",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 146,
      "name": "Aerolineas Ejecutivas",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 147,
      "name": "Aeronautical Charters",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 148,
      "name": "Aerotours",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 172,
      "name": "Albinati Aeronautics",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 228,
      "name": "Catalina Aerospace",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 277,
      "name": "DuPage Aerospace",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 314,
      "name": "ExxAero",
      "category": "charter-operator",
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    }
  ]
}
```

Search for registered airlines. The airlines are available in 3 categories:

* `airline`
* `jet-shuttle`
* `charter-operator`

<aside class="notice">
In order to get the proper result you must sent the attribute "category", the default category is "airline" but you can search for multiple categories.
</aside>

| Parameter | Required | Description                      | Format |
|-----------|----------|----------------------------------|--------|
| s         | *no*     | The term you want to search for. | string |
| category  | *no*     | The desired airline category.    | string |
