## Airports

```shell
$ curl '/v1/airports' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d sort='iata_code'
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
  "from": 41,
  "to": 60,
  "data": [
    {
      "name": "Adana",
      "country": "Turkey",
      "city": "Adana",
      "iata_code": "ADA",
      "altitude": 65,
      "timezone_offset": 2,
      "timezone": "Europe/Istanbul",
      "icao_code": "LTAF",
      "latitude": 36.982166,
      "created_at": "2016-08-03 21:17:19",
      "updated_at": "2016-08-03 21:17:19",
      "longitude": 35.280388,
      "is_active": true,
      "id": "7fdda9ce-340c-45ec-a0dd-acf34146f186"
    }
  ]
}
```

### HTTP REQUEST
`GET /v1/airports`

### Definition

| Parameter | Required | Description                                                                               | Format  |
|-----------|----------|-------------------------------------------------------------------------------------------|---------|
| page      | *no*     | The number of the page.                                                                   | integer |
| sort      | *no*     | The column to sort the information. Default: `id`.                                        | integer |
| order     | *no*     | The direction to do the sorting. Available only `asc` and `desc` options. Default: `asc`. | integer |

### Autocomplete
`GET /v1/airports/autocomplete`

```shell
$ curl '/v1/airports/autocomplete' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d s='mia'
```

> Example Response

```
{
  "data": [
    {
      "iata_code": "MIA",
      "name": "Miami Intl",
      "latitude": 25.79325,
      "longitude": -80.290556
    },
    {
      "iata_code": "MIG",
      "name": "Mianyang Airport",
      "latitude": 31.4281,
      "longitude": 104.741
    },
    {
      "iata_code": "MPB",
      "name": "Miami Seaplane Base",
      "latitude": 25.7783,
      "longitude": -80.1703
    },
    {
      "iata_code": "OPF",
      "name": "Opa Locka",
      "latitude": 25.907,
      "longitude": -80.278389
    },
    {
      "iata_code": "OXD",
      "name": "Miami University Airport",
      "latitude": 39.5022607,
      "longitude": -84.7843814
    },
    {
      "iata_code": "TNT",
      "name": "Dade Collier Training And Transition",
      "latitude": 25.861806,
      "longitude": -80.897
    },
    {
      "iata_code": "ZVA",
      "name": "Miandrivazo",
      "latitude": -19.562778,
      "longitude": 45.450832
    }
  ]
}
```

| Parameter | Required | Description                      | Format |
|-----------|----------|----------------------------------|--------|
| s         | *no*     | The term you want to search for. | string |
