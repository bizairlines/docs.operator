# Flights
## List flights

```shell
$ curl '/v1/companies/{$company_id}/flights' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`GET /v1/companies/{company_id}/flights`

### DEFINITION
Returns the available flights based on a desired date regardless the aircraft.

| Parameter | Required | Description                      | Format |
|-----------|----------|----------------------------------|--------|
| date      | *no*     | Format: `YYYY-MM-DD`             | string |

## List aircraft flights

```shell
$ curl '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/flights' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`GET /v1/companies/{company_id}/aircraft/{aircraft_id}/flights`

### DEFINITION
Returns the available flights based on a desired date and aircraft.

| Parameter | Required | Description                      | Format |
|-----------|----------|----------------------------------|--------|
| date      | *no*     | Format: `YYYY-MM-DD`             | string |

## Show flight

```shell
$ curl '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/flights/{$flight_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`GET /v1/companies/{company_id}/aircraft/{aircraft_id}/flights/{flight_id}`

### DEFINITION
Get a flight.

## Create flight

```shell
$ curl -XPOST '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/flights' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"departure_airport":"3G4","arrive_airport":"7A4","flight_type":"empty-leg","segment_type":"jet","fare_type":"non-refundable"...}'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`POST /v1/companies/{company_id}/aircraft/{aircraft_id}/flights`

### DEFINITION
Create a flight.

| Parameter                             | Required | Description                                                                          | Format |
|---------------------------------------|----------|--------------------------------------------------------------------------------------|--------|
| departure_airport                     | *yes*    | Airport IATA Code. See [airport list](#airports).                                    | string |
| arrive_airport                        | *yes*    | Airport IATA Code. See [airport list](#airports).                                    | string |
| aircraft                              | *yes*    | Registered aircraft on company's fleet.                                              | string |
| flight_type                           | *no*     | Available options: `shuttle`, `empty-legt` and `full-charter`.                       | string |
| insurance_policy                      | *no*     | Insurance policy for that flight. If no policy is set it will get from the aircraft. | string |
| fare_type                             | *no*     | Available options: `refundable` and `non-refundable`.                                | string |
| departure_at                          | *no*     | Date time. Format: `YYYY-MM-DD hh:mm:ss`.                                            | string |
| arrive_at                             | *no*     | Date time. Format: `YYYY-MM-DD hh:mm:ss`.                                            | string |
| minimum_seats                         | *no*     | If `shuttle` flight, the minimum seats for the first checkout.                       | int    |
| blocked_seats                         | *no*     | | int |
| fare                                  | *no*     | If `shuttle` flight, the fare for each seat. For `empty-leg` and `full-charter` it will be auto calculated. | float |
| cancellation_policy[]                 | *no*     | | array |
| cancellation_policy[penalty_24h]      | *no*     | Penalty for cancelation less than 24h before flight.                                  | float   |
| cancellation_policy[penalty_72h]      | *no*     | Penalty for cancellation less than 72h before flight.                                 | float   |
| cancellation_policy[penalty_over_72h] | *no*     | Penalty for cancellation greater than 72h before flight.                              | float   |
| cancellation_policy[is_relative]      | *no*     | Wether is percentage or fixed value.                                                  | boolean |
| luggage_policy[]                      | *no*     | | array |
| luggage_policy[hand_quantity]         | *no*     | Maximum luggage in hands.                                                             | int     |
| luggage_policy[hand_weight]           | *no*     | Maximum weight for luggage in hands (Kilo).                                           | float   |
| luggage_policy[checkin_quantity]      | *no*     | Maximum luggage for checkin.                                                          | int     |
| luggage_policy[checkin_weight]        | *no*     | Maximum weight for luggage for checkin (Kilo).                                        | float   |

## Update flight

```shell
$ curl -XPUT '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/flights/{$flight_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"departure_airport":"3G4","arrive_airport":"7A4","flight_type":"empty-leg","segment_type":"jet","fare_type":"non-refundable"...}'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`PUT /v1/companies/{company_id}/aircraft/{aircraft_id}/flights/{flight_id}`

### DEFINITION
Update a flight.

| Parameter                             | Required | Description                                                                          | Format |
|---------------------------------------|----------|--------------------------------------------------------------------------------------|--------|
| departure_airport                     | *no*     | Airport IATA Code. See [airport list](#airports).                                    | string |
| arrive_airport                        | *no*     | Airport IATA Code. See [airport list](#airports).                                    | string |
| aircraft                              | *no*     | Registered aircraft on company's fleet.                                              | string |
| flight_type                           | *no*     | Available options: `shuttle`, `empty-legt` and `full-charter`.                       | string |
| insurance_policy                      | *no*     | Insurance policy for that flight. If no policy is set it will get from the aircraft. | string |
| fare_type                             | *no*     | Available options: `refundable` and `non-refundable`.                                | string |
| departure_at                          | *no*     | Date time. Format: `YYYY-MM-DD hh:mm:ss`.                                            | string |
| arrive_at                             | *no*     | Date time. Format: `YYYY-MM-DD hh:mm:ss`.                                            | string |
| minimum_seats                         | *no*     | If `shuttle` flight, the minimum seats for the first checkout.                       | int    |
| blocked_seats                         | *no*     | | int |
| fare                                  | *no*     | If `shuttle` flight, the fare for each seat. For `empty-leg` and `full-charter` it will be auto calculated. | float |
| cancellation_policy[]                 | *no*     | | array |
| cancellation_policy[penalty_24h]      | *no*     | Penalty for cancelation less than 24h before flight.                                  | float   |
| cancellation_policy[penalty_72h]      | *no*     | Penalty for cancellation less than 72h before flight.                                 | float   |
| cancellation_policy[penalty_over_72h] | *no*     | Penalty for cancellation greater than 72h before flight.                              | float   |
| cancellation_policy[is_relative]      | *no*     | Wether is percentage or fixed value.                                                  | boolean |
| luggage_policy[]                      | *no*     | | array |
| luggage_policy[hand_quantity]         | *no*     | Maximum luggage in hands.                                                             | int     |
| luggage_policy[hand_weight]           | *no*     | Maximum weight for luggage in hands (Kilo).                                           | float   |
| luggage_policy[checkin_quantity]      | *no*     | Maximum luggage for checkin.                                                          | int     |
| luggage_policy[checkin_weight]        | *no*     | Maximum weight for luggage for checkin (Kilo).                                        | float   |

## Delete flight

```shell
$ curl -XDELETE '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/flights/{$flight_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`DELETE /v1/companies/{company_id}/aircraft/{aircraft_id}/flights/{flight_id}`

### DEFINITION
Deletes a flight.

## Activate flight

```shell
$ curl -XPOST '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/flights/{$flight_id}/activate' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`POST /v1/companies/{company_id}/aircraft/{aircraft_id}/flights/{flight_id}/activate`

### DEFINITION
Activates a flight.

## Deactivate flight

```shell
$ curl -XPOST '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/flights/{$flight_id}/deactivate' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": "8fd7c746-ac1d-4937-b480-1772ec08dd31",
      "aircraft_id": null,
      "departure_airport": {
        "name": "Ashland County Airport",
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
        "state": null,
        "city": "Ashland",
        "region": null,
        "iata_code": "3G4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 1206,
        "latitude": 40.9029722,
        "longitude": -82.2556389,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "c49f2a78-8c9a-45f2-aa16-d54f7f8c24ef"
      },
      "arrive_airport": {
        "name": "Foster Field",
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
        "state": null,
        "city": "Apple River",
        "region": null,
        "iata_code": "7A4",
        "icao_code": "\\N",
        "timezone": {
          "timezone": "America/Chicago",
          "offset": "-06:00"
        },
        "altitude": 990,
        "latitude": 42.4664444,
        "longitude": -90.1693889,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:21",
        "updated_at": "2016-10-19 11:33:37",
        "id": "716f6b04-6928-4653-a50a-fa6d66bd9d12"
      },
      "flight_type": "empty-leg",
      "segment_type": "jet",
      "fare_type": "non-refundable",
      "insurance_policy": "test",
      "flight_number": "1322",
      "minimum_seats": 1,
      "blocked_seats": 1,
      "available_seats": 500,
      "total_seats": 501,
      "trip_time": 120,
      "checkin_time": null,
      "security_time": null,
      "boarding_time": null,
      "has_internet": null,
      "has_power_outlet": null,
      "has_friendly_seat": null,
      "is_active": true,
      "is_quote": 0,
      "is_biz_connect": false,
      "is_sold_out": false,
      "is_international_flight": false,
      "is_recurrence": true,
      "fare": null,
      "recurrence": "{\"type\":\"daily\",\"interval\":1,\"ends_at\":\"2016-12-21\"}",
      "departure_at": "2016-12-05T17:02:00-05:00",
      "arrive_at": "2016-12-05T18:02:00-06:00",
      "created_at": "2016-11-21 15:01:08",
      "updated_at": "2016-11-21 15:01:08",
      "aircraft": {
        "id": "cc84ca08-4742-499e-9129-64a3864274d5",
        "aircraft": {
          "id": 47,
          "manufacturer": {
            "id": 4,
            "name": "Beechcraft"
          },
          "category": null,
          "type": null,
          "name": "Beechcraft King Air C90F",
          "engine": null,
          "crew_capacity": null,
          "passanger_capacity": null,
          "length": null,
          "width": null,
          "height": null,
          "empty_weight": null,
          "wingspan": null,
          "fuselage_width": null,
          "fuselage_height": null,
          "wing_area": null,
          "max_fuel_load": null,
          "max_speed": null,
          "cruise_speed": null,
          "max_takeoff_distance": null,
          "max_takeoff_weight": null,
          "max_landing_distance": null,
          "max_landing_weight": null,
          "max_range_distance": null,
          "created_at": null,
          "updated_at": null
        },
        "airline": {
          "id": 631,
          "name": "Kyle House Company",
          "category": "charter-operator",
          "iata_code": "KYL",
          "icao_code": "KYle",
          "created_at": "2016-11-08 08:43:06",
          "updated_at": "2016-11-08 08:43:06"
        },
        "airport": {
          "name": "John F Kennedy Intl",
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
          "state": null,
          "city": "New York",
          "region": null,
          "iata_code": "JFK",
          "icao_code": "KJFK",
          "timezone": {
            "timezone": "America/New_York",
            "offset": "-05:00"
          },
          "altitude": 13,
          "latitude": 40.639751,
          "longitude": -73.778925,
          "taxi_time": null,
          "is_active": true,
          "created_at": "2016-08-03 21:17:20",
          "updated_at": "2016-10-19 11:33:27",
          "id": "bf7ead59-3fed-4f32-8358-942f6c00b145"
        },
        "fabrication_year": 2014,
        "refurbished_interior_year": 2016,
        "registration_number": "N131AD",
        "crew_capacity": null,
        "passenger_capacity": 500,
        "insurance_policy_value": 1000,
        "insurance_policy_link": "www.kyle.com",
        "insurance_policy_description": "qweqweqwe",
        "cruise_speed": null,
        "passenger_hourly_cost": 13,
        "repositioning_hourly_cost": 13,
        "empty_leg_hourly_cost": 13,
        "overnight_fee": 13,
        "landing_fee": 13,
        "min_operation_cost": null,
        "max_repositioning_distance": null,
        "max_overnight_day": 1,
        "has_entertainment": true,
        "has_wifi": false,
        "has_power_outlet": true,
        "has_laptop_seat": false,
        "is_auto_empty_leg": true,
        "is_full_charter": false,
        "is_empty_leg": true,
        "is_shuttle": true,
        "is_part_91": true,
        "is_part_121": true,
        "is_part_135": false,
        "is_argus": false,
        "is_wyvern": true,
        "is_isbao": true,
        "is_ascf": true,
        "is_instant_booking": true,
        "is_active": true,
        "created_at": "2016-11-08 08:45:30",
        "updated_at": "2016-12-05 11:40:28",
        "upload": [
          {
            "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
            "name": "company/51-kyle-house-company/aircraft/hwkwyy9i66o5bbhrvyy0",
            "mimetype": "image/png",
            "size": 312110,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-08 08:46:01",
            "updated_at": "2016-11-08 08:46:01",
            "position": "other-3"
          },
          {
            "id": "c0b0718e-a87a-4a99-a190-6080e6363520",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf.jpeg",
            "name": "company/51-kyle-house-company/aircraft/ajofyznofsytaqstmftf",
            "mimetype": "image/jpeg",
            "size": 909224,
            "extension": "jpeg",
            "is_active": true,
            "created_at": "2016-11-08 15:45:33",
            "updated_at": "2016-11-08 15:45:33",
            "position": "other-2"
          },
          {
            "id": "e85521b2-90b1-4813-b776-768a9d059d7c",
            "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak.png",
            "name": "company/51-kyle-house-company/aircraft/ybyolsryocs3wh0cstak",
            "mimetype": "image/png",
            "size": 5012,
            "extension": "png",
            "is_active": true,
            "created_at": "2016-11-28 22:23:28",
            "updated_at": "2016-11-28 22:23:28",
            "position": "seats"
          }
        ]
      },
      "airline": {
        "id": 631,
        "name": "Kyle House Company",
        "category": "charter-operator",
        "iata_code": "KYL",
        "icao_code": "KYle",
        "created_at": "2016-11-08 08:43:06",
        "updated_at": "2016-11-08 08:43:06"
      },
      "cancellation_policy": {
        "id": "d17955a3-bf7d-44b9-9516-dea1744492ba",
        "cancellation_policy": "test",
        "penalty_24h": 1.23,
        "penalty_72h": 1.23,
        "penalty_over_72h": 1.23,
        "is_relative": true,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      },
      "luggage_policy": {
        "id": "a47dfb53-0b09-4cde-ae24-009344f16105",
        "hand_quantity": 1,
        "hand_weight": 1.23,
        "checkin_quantity": 1,
        "checkin_weight": 1.23,
        "created_at": "2016-11-21 15:01:09",
        "updated_at": "2016-11-21 15:01:09"
      }
    }
  ]
}
```

### HTTP REQUEST
`POST /v1/companies/{company_id}/aircraft/{aircraft_id}/flights/{flight_id}/deactivate`

### DEFINITION
Deactivates a flight.
