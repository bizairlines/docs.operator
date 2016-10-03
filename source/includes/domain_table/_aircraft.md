## Aircraft
> `GET /v1/aircraft/autocomplete`

```shell
$ curl '/v1/aircraft/autocomplete' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d s="learj"
```
> Example response

```
{
  "data": [
    {
      "id": 1,
      "name": "Airbus A300",
      "crew_capacity": null,
      "passanger_capacity": null,
      "length": null,
      "width": null,
      "height": null,
      "empty_weight": null,
      "max_takeoff_weight": null,
      "wingspan": null,
      "fuselage_width": null,
      "fuselage_height": null,
      "wing_area": null,
      "maximum_fuel_load": null,
      "engine": null,
      "maximum_speed": null,
      "cruise_speed": null,
      "never_exceed_speed": null,
      "manufacturer": {
        "id": 1,
        "name": "Airbus"
      }
    },
    {
      "id": 2,
      "name": "Airbus A310",
      "crew_capacity": null,
      "passanger_capacity": null,
      "length": null,
      "width": null,
      "height": null,
      "empty_weight": null,
      "max_takeoff_weight": null,
      "wingspan": null,
      "fuselage_width": null,
      "fuselage_height": null,
      "wing_area": null,
      "maximum_fuel_load": null,
      "engine": null,
      "maximum_speed": null,
      "cruise_speed": null,
      "never_exceed_speed": null,
      "manufacturer": {
        "id": 1,
        "name": "Airbus"
      }
    }
  ]
}
```

| Parameter | Required | Description                      | Format |
|-----------|----------|----------------------------------|--------|
| s         | *no*     | The term you want to search for. | string |
