## Airlines
```
GET /v1/airlines/autocomplete
```
```shell
$ curl '/v1/airlines/autocomplete' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d s='aero' \
    -d category[]='jet-shuttle' \
    -d category[]='charter-operator'
```
```
Example response
```
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

Return the list of registered airlines. The airlines are available in 3 categories:

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
