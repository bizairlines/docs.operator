## Airports
> `GET /v1/airports/autocomplete`

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
