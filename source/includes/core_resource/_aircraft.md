# Aircraft
## List available aircraft

```shell
$ curl '/v1/companies/{$company_id}/aircraft' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example Response

```
{
  "data": [
    {
      "id": "cc84ca08-4742-499e-9129-64a3864274d5",
      "aircraft": {
        "id": 66,
        "manufacturer": {
          "id": 5,
          "name": "Boeing"
        },
        "category": null,
        "type": null,
        "name": "Boeing 787",
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
        "name": "My Jet Company",
        "category": "charter-operator",
        "iata_code": "XP",
        "icao_code": "XPT",
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
      "fabrication_year": 2015,
      "refurbished_interior_year": 2016,
      "registration_number": "N131AD",
      "crew_capacity": null,
      "passenger_capacity": null,
      "insurance_policy_value": null,
      "insurance_policy_link": "www.my-jet-company.com",
      "insurance_policy_description": null,
      "cruise_speed": null,
      "passenger_hourly_cost": 0,
      "repositioning_hourly_cost": 0,
      "empty_leg_hourly_cost": 0,
      "overnight_fee": 0,
      "landing_fee": 0,
      "min_operation_cost": null,
      "max_repositioning_distance": null,
      "max_overnight_day": 0,
      "has_entertainment": true,
      "has_wifi": false,
      "has_power_outlet": true,
      "has_laptop_seat": false,
      "is_auto_empty_leg": true,
      "is_full_charter": false,
      "is_empty_leg": true,
      "is_shuttle": true,
      "is_part_91": false,
      "is_part_121": true,
      "is_part_135": false,
      "is_argus": false,
      "is_wyvern": true,
      "is_isbao": true,
      "is_ascf": true,
      "is_instant_booking": true,
      "is_active": true,
      "created_at": "2016-11-08 08:45:30",
      "updated_at": "2016-11-29 13:09:32",
      "company": {
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
          "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-/hqhrsfjsu4q7vew1dpi1.png",
          "name": "company/51-/hqhrsfjsu4q7vew1dpi1",
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
        "site": "www.kyle.com",
        "phone": "12121212",
        "address_1": "Miami International Airport, Northwest 25th Street, Miami, FL, United States",
        "address_2": "",
        "city": "Miami",
        "state": "Florida",
        "zipcode": "33142",
        "bank_info": null,
        "contact_info": null,
        "contact_name": "Kyle House",
        "contact_phone": "12121212",
        "contact_email": "kyle@gmail.com",
        "is_active": true,
        "is_airline": false,
        "is_operator": true,
        "has_entered_iata": true,
        "created_at": "2016-11-08 08:41:35",
        "updated_at": "2016-11-25 00:26:00"
      },
      "upload": [
        {
          "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
          "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
          "name": "company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0",
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
          "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf.jpeg",
          "name": "company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf",
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
          "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak.png",
          "name": "company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak",
          "mimetype": "image/png",
          "size": 5012,
          "extension": "png",
          "is_active": true,
          "created_at": "2016-11-28 22:23:28",
          "updated_at": "2016-11-28 22:23:28",
          "position": "seats"
        }
      ]
    }
  ]
}
```

### HTTP Request
`GET /v1/companies/{company_id}/aircraft`

### Definition
List the available aircraft from the company.

## Show aircraft

```shell
$ curl '/v1/companies/{$company_id}/aircraft/{$aircraft_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example Response

```
{
  "data": {
    "id": "cc84ca08-4742-499e-9129-64a3864274d5",
    "aircraft": {
      "id": 66,
      "manufacturer": {
        "id": 5,
        "name": "Boeing"
      },
      "category": null,
      "type": null,
      "name": "Boeing 787",
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
      "name": "My Jet Company",
      "category": "charter-operator",
      "iata_code": "XP",
      "icao_code": "XPT",
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
    "fabrication_year": 2015,
    "refurbished_interior_year": 2016,
    "registration_number": "N131AD",
    "crew_capacity": null,
    "passenger_capacity": null,
    "insurance_policy_value": null,
    "insurance_policy_link": "www.my-jet-company.com",
    "insurance_policy_description": null,
    "cruise_speed": null,
    "passenger_hourly_cost": 0,
    "repositioning_hourly_cost": 0,
    "empty_leg_hourly_cost": 0,
    "overnight_fee": 0,
    "landing_fee": 0,
    "min_operation_cost": null,
    "max_repositioning_distance": null,
    "max_overnight_day": 0,
    "has_entertainment": true,
    "has_wifi": false,
    "has_power_outlet": true,
    "has_laptop_seat": false,
    "is_auto_empty_leg": true,
    "is_full_charter": false,
    "is_empty_leg": true,
    "is_shuttle": true,
    "is_part_91": false,
    "is_part_121": true,
    "is_part_135": false,
    "is_argus": false,
    "is_wyvern": true,
    "is_isbao": true,
    "is_ascf": true,
    "is_instant_booking": true,
    "is_active": true,
    "created_at": "2016-11-08 08:45:30",
    "updated_at": "2016-11-29 13:09:32",
    "company": {
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-/hqhrsfjsu4q7vew1dpi1.png",
        "name": "company/51-/hqhrsfjsu4q7vew1dpi1",
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
      "site": "www.kyle.com",
      "phone": "12121212",
      "address_1": "Miami International Airport, Northwest 25th Street, Miami, FL, United States",
      "address_2": "",
      "city": "Miami",
      "state": "Florida",
      "zipcode": "33142",
      "bank_info": null,
      "contact_info": null,
      "contact_name": "Kyle House",
      "contact_phone": "12121212",
      "contact_email": "kyle@gmail.com",
      "is_active": true,
      "is_airline": false,
      "is_operator": true,
      "has_entered_iata": true,
      "created_at": "2016-11-08 08:41:35",
      "updated_at": "2016-11-25 00:26:00"
    },
    "upload": [
      {
        "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
        "name": "company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0",
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf.jpeg",
        "name": "company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf",
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak.png",
        "name": "company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak",
        "mimetype": "image/png",
        "size": 5012,
        "extension": "png",
        "is_active": true,
        "created_at": "2016-11-28 22:23:28",
        "updated_at": "2016-11-28 22:23:28",
        "position": "seats"
      }
    ]
  }
}
```

### HTTP REQUEST
`GET /v1/companies/{company_id}/aircraft/{aircraft_id}`

### DEFINITION
Get the aircraft's public information.

## Create aircraft

```shell
$ curl -XPOST'/v1/companies/{$company_id}/aircraft' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"aircraft": 66, "airport": "JFK", "registration_number": N131AD}'
```

> Example Response

```
{
  "data": {
    "id": "cc84ca08-4742-499e-9129-64a3864274d5",
    "aircraft": {
      "id": 66,
      "manufacturer": {
        "id": 5,
        "name": "Boeing"
      },
      "category": null,
      "type": null,
      "name": "Boeing 787",
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
      "name": "My Jet Company",
      "category": "charter-operator",
      "iata_code": "XP",
      "icao_code": "XPT",
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
    "passenger_capacity": null,
    "insurance_policy_value": null,
    "insurance_policy_link": "www.my-jet-company.com",
    "insurance_policy_description": null,
    "cruise_speed": null,
    "passenger_hourly_cost": 0,
    "repositioning_hourly_cost": 0,
    "empty_leg_hourly_cost": 0,
    "overnight_fee": 0,
    "landing_fee": 0,
    "min_operation_cost": null,
    "max_repositioning_distance": null,
    "max_overnight_day": 0,
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
    "updated_at": "2016-11-29 13:09:32",
    "company": {
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-/hqhrsfjsu4q7vew1dpi1.png",
        "name": "company/51-/hqhrsfjsu4q7vew1dpi1",
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
      "site": "www.kyle.com",
      "phone": "12121212",
      "address_1": "Miami International Airport, Northwest 25th Street, Miami, FL, United States",
      "address_2": "",
      "city": "Miami",
      "state": "Florida",
      "zipcode": "33142",
      "bank_info": null,
      "contact_info": null,
      "contact_name": "Kyle House",
      "contact_phone": "12121212",
      "contact_email": "kyle@gmail.com",
      "is_active": true,
      "is_airline": false,
      "is_operator": true,
      "has_entered_iata": true,
      "created_at": "2016-11-08 08:41:35",
      "updated_at": "2016-11-25 00:26:00"
    },
    "upload": [
      {
        "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
        "name": "company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0",
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf.jpeg",
        "name": "company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf",
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak.png",
        "name": "company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak",
        "mimetype": "image/png",
        "size": 5012,
        "extension": "png",
        "is_active": true,
        "created_at": "2016-11-28 22:23:28",
        "updated_at": "2016-11-28 22:23:28",
        "position": "seats"
      }
    ]
  }
}
```

### HTTP REQUEST
`POST /v1/companies/{company_id}/aircraft`

### DEFINITION
Update the aircraft's public information.

| Parameter                    | Required | Description                                                       | Format  |
|------------------------------|----------|-------------------------------------------------------------------|---------|
| aircraft                     | *yes*    | ID for the aircraft available in the [domain table](#aircraft23). | int     |
| airport                      | *yes*    | IATA Code for the aircraft base. See [airport list](#airports).   | string  |
| fabrication_year             | *yes*    | | int     |
| refurbished_interior_year    | *no*     | | int     |
| registration_number          | *no*     | | string  |
| crew_capacity                | *no*     | | int     |
| passenger_capacity           | *no*     | | int     |
| insurance_policy_description | *no*     | | string  |
| insurance_policy_value       | *no*     | | float   |
| insurance_policy_link        | *no*     | | string  |
| cruise_speed                 | *no*     | | float   |
| passenger_hourly_cost        | *no*     | | float   |
| repositioning_hourly_cost    | *no*     | | float   |
| empty_leg_hourly_cost        | *no*     | | float   |
| overnight_fee                | *no*     | | float   |
| landing_fee                  | *no*     | | float   |
| min_operation_cost           | *no*     | Minimum operation cost. Used to overwrite full charter or empty-leg costs if it's value are less than `min_operation_cost`.     | float   |
| max_repositioning_distance   | *no*     | Maximum repositioning distance in Kilometers from aircraft's base.                                                              | float   |
| max_overnight_day            | *no*     | Maximum overnight days the aircraft is allowed.                                                                                 | int     |
| has_entertainment            | *no*     | If the aircraft has entertaiment options.                                                                                       | boolean |
| has_wifi                     | *no*     | If the aircraft has wifi connections.                                                                                           | boolean |
| has_power_outlet             | *no*     | If the aircraft has power outlet.                                                                                               | boolean |
| has_laptop_seat              | *no*     | If the aircraft has space enough to open a laptop with confort.                                                                 | boolean |
| is_auto_empty_leg            | *no*     | If the API can create an empty-leg flight after a full charter payment confirmation.                                            | boolean |
| is_full_charter              | *no*     | If the aircraft is available for full charter flights. If the value is `false` the aircraft will not be available for searches. | boolean |
| is_empty_leg                 | *no*     | If the aircraft is available for empty-leg flights.                                                                             | boolean |
| is_shuttle                   | *no*     | If the aircraft is available for shuttle flights.                                                                               | boolean |
| is_part_91                   | *no*     | | boolean |
| is_part_121                  | *no*     | | boolean |
| is_part_135                  | *no*     | | boolean |
| is_argus                     | *no*     | | boolean |
| is_wyvern                    | *no*     | | boolean |
| is_isbao                     | *no*     | | boolean |
| is_ascf                      | *no*     | | boolean |
| is_instant_booking           | *no*     | If the aircraft requires owner authorization for empty-legs and full charter bookings.                                          | boolean |

## Update aircraft

```shell
$ curl -XPUT '/v1/companies/{$company_id}/aircraft/{$aircraft_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"is_part_91": true, "fabrication_year": 2014}'
```

> Example Response

```
{
  "data": {
    "id": "cc84ca08-4742-499e-9129-64a3864274d5",
    "aircraft": {
      "id": 66,
      "manufacturer": {
        "id": 5,
        "name": "Boeing"
      },
      "category": null,
      "type": null,
      "name": "Boeing 787",
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
      "name": "My Jet Company",
      "category": "charter-operator",
      "iata_code": "XP",
      "icao_code": "XPT",
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
    "passenger_capacity": null,
    "insurance_policy_value": null,
    "insurance_policy_link": "www.my-jet-company.com",
    "insurance_policy_description": null,
    "cruise_speed": null,
    "passenger_hourly_cost": 0,
    "repositioning_hourly_cost": 0,
    "empty_leg_hourly_cost": 0,
    "overnight_fee": 0,
    "landing_fee": 0,
    "min_operation_cost": null,
    "max_repositioning_distance": null,
    "max_overnight_day": 0,
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
    "updated_at": "2016-11-29 13:09:32",
    "company": {
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-/hqhrsfjsu4q7vew1dpi1.png",
        "name": "company/51-/hqhrsfjsu4q7vew1dpi1",
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
      "site": "www.kyle.com",
      "phone": "12121212",
      "address_1": "Miami International Airport, Northwest 25th Street, Miami, FL, United States",
      "address_2": "",
      "city": "Miami",
      "state": "Florida",
      "zipcode": "33142",
      "bank_info": null,
      "contact_info": null,
      "contact_name": "Kyle House",
      "contact_phone": "12121212",
      "contact_email": "kyle@gmail.com",
      "is_active": true,
      "is_airline": false,
      "is_operator": true,
      "has_entered_iata": true,
      "created_at": "2016-11-08 08:41:35",
      "updated_at": "2016-11-25 00:26:00"
    },
    "upload": [
      {
        "id": "b59b61fb-d947-46a3-a1df-5eb629ebd2f6",
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0.png",
        "name": "company/51-my-jet-company/aircraft/hwkwyy9i66o5bbhrvyy0",
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf.jpeg",
        "name": "company/51-my-jet-company/aircraft/ajofyznofsytaqstmftf",
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
        "url": "https://res.cloudinary.com/bizairlines/image/upload/v1/company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak.png",
        "name": "company/51-my-jet-company/aircraft/ybyolsryocs3wh0cstak",
        "mimetype": "image/png",
        "size": 5012,
        "extension": "png",
        "is_active": true,
        "created_at": "2016-11-28 22:23:28",
        "updated_at": "2016-11-28 22:23:28",
        "position": "seats"
      }
    ]
  }
}
```

### HTTP REQUEST
`PUT /v1/companies/{company_id}/aircraft/{aircraft_id}`

### DEFINITION
Update the aircraft's public information.

| Parameter                    | Description                                                       | Format  |
|------------------------------|-------------------------------------------------------------------|---------|
| aircraft                     | ID for the aircraft available in the [domain table](#aircraft23). | int     |
| airport                      | IATA Code for the aircraft base. See [airport list](#airports).   | string  |
| fabrication_year             | | int     |
| refurbished_interior_year    | | int     |
| registration_number          | | string  |
| crew_capacity                | | int     |
| passenger_capacity           | | int     |
| insurance_policy_description | | string  |
| insurance_policy_value       | | float   |
| insurance_policy_link        | | string  |
| cruise_speed                 | | float   |
| passenger_hourly_cost        | | float   |
| repositioning_hourly_cost    | | float   |
| empty_leg_hourly_cost        | | float   |
| overnight_fee                | | float   |
| landing_fee                  | | float   |
| min_operation_cost           | Minimum operation cost. Used to overwrite full charter or empty-leg costs if it's value are less than `min_operation_cost`.     | float   |
| max_repositioning_distance   | Maximum repositioning distance in Kilometers from aircraft's base.                                                              | float   |
| max_overnight_day            | Maximum overnight days the aircraft is allowed.                                                                                 | int     |
| has_entertainment            | If the aircraft has entertaiment options.                                                                                       | boolean |
| has_wifi                     | If the aircraft has wifi connections.                                                                                           | boolean |
| has_power_outlet             | If the aircraft has power outlet.                                                                                               | boolean |
| has_laptop_seat              | If the aircraft has space enough to open a laptop with confort.                                                                 | boolean |
| is_auto_empty_leg            | If the API can create an empty-leg flight after a full charter payment confirmation.                                            | boolean |
| is_full_charter              | If the aircraft is available for full charter flights. If the value is `false` the aircraft will not be available for searches. | boolean |
| is_empty_leg                 | If the aircraft is available for empty-leg flights.                                                                             | boolean |
| is_shuttle                   | If the aircraft is available for shuttle flights.                                                                               | boolean |
| is_part_91                   | | boolean |
| is_part_121                  | | boolean |
| is_part_135                  | | boolean |
| is_argus                     | | boolean |
| is_wyvern                    | | boolean |
| is_isbao                     | | boolean |
| is_ascf                      | | boolean |
| is_instant_booking           | If the aircraft requires owner authorization for empty-legs and full charter bookings.                                          | boolean |

## Upload image

```shell
$ curl -XPOST '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/uploads' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"image":"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABG4AAAS4CAYAAABGqo...}'
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
`POST /v1/companies/{company_id}/aircraft/{aircraft_id}/uploads`

### DEFINITION
Uploads images for the aircraft.

Requirements:

* Min width: 100px;
* Min height: 100px;
* Max image size: 2.5Mb;
* Allowed extensions: `jpeg`, `jpg`, `gif` and `png`;

## Delete image

```shell
$ curl -XDELETE '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/uploads/{$file_id}' \
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
`DELETE /v1/companies/{company_id}/{aircraft_id}/uploads/{file_id}`

### DEFINITION
Removes aircraft's image.

## List temporary base

```shell
$ curl '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/temporary-bases' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": "e831d803-feef-4bd1-b219-f0a0acefb4dd",
      "airport": {
        "name": "Miami Intl",
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
        "city": "Miami",
        "region": null,
        "iata_code": "MIA",
        "icao_code": "KMIA",
        "timezone": {
          "timezone": "America/New_York",
          "offset": "-05:00"
        },
        "altitude": 8,
        "latitude": 25.79325,
        "longitude": -80.290556,
        "taxi_time": null,
        "is_active": true,
        "created_at": "2016-08-03 21:17:20",
        "updated_at": "2016-10-19 11:33:26",
        "id": "074d49ea-89dc-4c39-b5e5-abbe1c94dc88"
      },
      "starts_at": "2016-12-24",
      "ends_at": "2017-01-02",
      "created_at": "2016-12-05 13:26:04",
      "updated_at": "2016-12-05 13:26:04"
    }
  ]
}
```

### HTTP REQUEST
`GET /v1/companies/{company_id}/aircraft/{aircraft_id}/temporary-bases`

### DEFINITION
Lists the aircraft's temporary bases.

<aside class="notice">
This endpoint will not return past temporary bases.
</aside>

## Create temporary base

```shell
$ curl -XPOST '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/temporary-bases' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": {
    "airport": {
      "name": "Miami Intl",
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
      "city": "Miami",
      "region": null,
      "iata_code": "MIA",
      "icao_code": "KMIA",
      "timezone": {
        "timezone": "America/New_York",
        "offset": "-05:00"
      },
      "altitude": 8,
      "latitude": 25.79325,
      "longitude": -80.290556,
      "taxi_time": null,
      "is_active": true,
      "created_at": "2016-08-03 21:17:20",
      "updated_at": "2016-10-19 11:33:26",
      "id": "074d49ea-89dc-4c39-b5e5-abbe1c94dc88"
    },
    "starts_at": "2016-12-24",
    "ends_at": "2017-01-02",
    "updated_at": "2016-12-05 13:26:04",
    "created_at": "2016-12-05 13:26:04",
    "id": "e831d803-feef-4bd1-b219-f0a0acefb4dd"
  }
}
```

### HTTP REQUEST
`POST /v1/companies/{company_id}/aircraft/{aircraft_id}/temporary-bases`

### DEFINITION
Creates aircraft's temporary bases.

| Parameter | Required | Description                                                       | Format  |
|-----------|----------|-------------------------------------------------------------------|---------|
| airport   | *yes*    | IATA Code for the aircraft base. See [airport list](#airports).   | string  |
| starts_at | *yes*    | Start date. Format: `YYYY-MM-DD`                                  | date    |
| ends_at   | *yes*    | End date. Format: `YYYY-MM-DD`                                    | date    |

## Delete temporary base

```shell
$ curl -XDELETE '/v1/companies/{$company_id}/aircraft/{$aircraft_id}/temporary-bases/{$temporary_base_id}' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": {
    "airport": {
      "name": "Miami Intl",
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
      "city": "Miami",
      "region": null,
      "iata_code": "MIA",
      "icao_code": "KMIA",
      "timezone": {
        "timezone": "America/New_York",
        "offset": "-05:00"
      },
      "altitude": 8,
      "latitude": 25.79325,
      "longitude": -80.290556,
      "taxi_time": null,
      "is_active": true,
      "created_at": "2016-08-03 21:17:20",
      "updated_at": "2016-10-19 11:33:26",
      "id": "074d49ea-89dc-4c39-b5e5-abbe1c94dc88"
    },
    "starts_at": "2016-12-24",
    "ends_at": "2017-01-02",
    "updated_at": "2016-12-05 13:26:04",
    "created_at": "2016-12-05 13:26:04",
    "id": "e831d803-feef-4bd1-b219-f0a0acefb4dd"
  }
}
```

### HTTP REQUEST
`DELETE /v1/companies/{company_id}/aircraft/{aircraft_id}/temporary-bases/{temporary_base_id}`

### DEFINITION
Deletes aircraft's temporary bases.
