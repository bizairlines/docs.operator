# Itineraries
## Search
> `POST /v1/itineraries/search`

```shell
$ curl -XPOST '/v1/itineraries/search' \
    -H 'Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9...' \
    -H 'Content-type: application/json' \
    -d '{"departure_airport":"MCO","arrive_airport":"OPF","departure_at":[{"condition":">=","value":"2016-10-17 00:00:00"},{"condition":"<=","value":"2016-10-17 23:59:59"}],"available_seats":[{"condition":">=","value":1}]}'
```

> Example Response

```
{
  "data": [
    {
      "name": "MCO-OPF",
      "fare": 799,
      "important_notes": "Please pay attention to the departure locations below.\n\nOutbound flight information:\nDeparts from  Atlantic Aviation MCO - 9245 Tradeport Dr, Orlando, FL 32827, United States.\nArrives at 14201 NW 42nd Ave, Opa-locka, FL 33054, United States.\nOperated by: BizConnect Partner\n\nTransportation agreement (if any): http://bizairlines.com/_legal/operators/bizconnect.pdf\n\nExtra information: Check-in 15 minutes prior to the flight.",
      "cancellation_policies": "Fare is Non-refundable. No-show is non-refundable.\n\nItinerary change fees: Changes NOT allowed.\n\nBy purchasing this ticket you agreed to the following cancellation policy: STANDARD JET\n\nPLEASE READ ALL THE CANCELLATION POLICIES BELOW:\n-------------\n50% OF TICKET: Half of the price of the ticket will be refunded for this cancellation policy. Refund may take up to 14 days to appear in your statement. | STANDARD JET POLICY: The greater of $1,000 or full purchase price for cancellations within 24 hours from flight departure; $1,000 for cancellations between 72 and 24 hours from flight departure; $500 for cancellations between 72 hours and 7 days from flight departure. $250 for cancellations made more than 7 days prior to flight departure. | STANDARD AIRLINE POLICY: $250.00 will be charged to any cancellations regardless of ticket cost. The balance will be returned to your Credit Card in up to 10 week days. Cancellations within 24 hours from purchase might be eligible for full refund. | FULLY-REFUNDABLE POLICY. Full cost of ticket will be returned to your Credit Card in up to 10 week days.\n-------------\n\nFor further assistance, please call +1 (877) 331-2412.",
      "luggage_policies": "For this itinerary you are allowed: One standard sized carry-on item of less than 7kg (15lbs) and one personal item (laptop, purse, backpack)., One 23kg (51lbs) allowed per passenger.  Please call +1 (877) 331-2412 if you need extra luggage purchase.",
      "liability_insurance": "$20,000,000.",
      "is_round_trip": 0,
      "is_active": 1,
      "is_sold_out": 0,
      "created_at": "2016-08-04 22:43:51",
      "updated_at": "2016-08-05 13:44:29",
      "id": "dad08178-1d90-4bfa-b253-69ffeaead4ed",
      "flight": [
        {
          "id": "fd7a9a26-3a49-4d3d-a988-d731535470d5",
          "departure_airport": {
            "name": "Orlando Intl",
            "country": "United States",
            "city": "Orlando",
            "iata_code": "MCO",
            "altitude": 96,
            "timezone_offset": -5,
            "timezone": "America/New_York",
            "icao_code": "KMCO",
            "latitude": 28.429394,
            "created_at": "2016-08-03 21:17:20",
            "updated_at": "2016-08-03 21:17:20",
            "longitude": -81.308994,
            "is_active": true,
            "id": "699acd23-c60c-45b2-b22a-c541874ebdee"
          },
          "arrive_airport": {
            "name": "Opa Locka",
            "country": "United States",
            "city": "Miami",
            "iata_code": "OPF",
            "altitude": 8,
            "timezone_offset": -5,
            "timezone": "America/New_York",
            "icao_code": "KOPF",
            "latitude": 25.907,
            "created_at": "2016-08-03 21:17:20",
            "updated_at": "2016-08-03 21:17:20",
            "longitude": -80.278389,
            "is_active": true,
            "id": "c7dc2fc7-8d0e-4693-9386-ee4788f39dc1"
          },
          "flight_type": "shuttle",
          "segment_type": null,
          "fare_type": "non-refundable",
          "flight_number": "BZ0001",
          "minimum_seats": 2,
          "blocked_seats": 1,
          "available_seats": 6,
          "total_seats": 7,
          "insurance_policy": null,
          "recurrence": null,
          "trip_time": 46,
          "is_active": 1,
          "is_quote": 0,
          "is_biz_connect": true,
          "is_sold_out": 0,
          "is_international_flight": false,
          "departure_at": "2016-10-17T07:30:00-04:00",
          "arrive_at": "2016-08-17T08:16:00-04:00",
          "created_at": "2016-08-04 22:43:51",
          "updated_at": "2016-09-20 18:04:58",
          "company": {},
          "fleet": {
            "id": "a37f1798-5b9e-40bd-9081-2e7bd729c2e0",
            "airport": {
              "name": "Orlando Intl",
              "country": "United States",
              "city": "Orlando",
              "iata_code": "MCO",
              "altitude": 96,
              "timezone_offset": -5,
              "timezone": "America/New_York",
              "icao_code": "KMCO",
              "latitude": 28.429394,
              "created_at": "2016-08-03 21:17:20",
              "updated_at": "2016-08-03 21:17:20",
              "longitude": -81.308994,
              "is_active": true,
              "id": "699acd23-c60c-45b2-b22a-c541874ebdee"
            },
            "fabrication_year": null,
            "registration_number": "N01BIZ",
            "crew_capacity": null,
            "passenger_capacity": 7,
            "operation": null,
            "safety_rating": null,
            "insurance_policy": null,
            "cruise_speed": null,
            "auto_empty_leg": 0,
            "is_active": 1,
            "created_at": "-0001-11-30 00:00:00",
            "updated_at": "-0001-11-30 00:00:00",
            "aircraft": {
              "id": 349,
              "name": "Light Jet",
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
                "id": 37,
                "name": "-"
              }
            },
            "company": {},
            "airline": {
              "id": 623,
              "name": "Biz Airlines",
              "category": "charter-operator",
              "created_at": "2016-08-05 10:17:19",
              "updated_at": "2016-08-05 10:17:23"
            },
            "upload": []
          },
          "airline": null
        }
      ]
    }
  ]
}
```

| Parameter               | Required | Description      | Format |
|-------------------------|----------|------------------|--------|
| departure_airport       | *yes*    | IATA Code from the origin airport.          | string         |
| arrive_airport          | *yes*    | IATA Code from the destination airport.     | string         |
| is_active               | *no*     | Return active flights. Default: *true*      | boolean        |
| is_biz_connect          | *no*     | Return only Biz Connect flights.            | boolean        |
| is_international_flight | *no*     | Return only international flights.          | boolean        |
| departure_at            | *no*     | The departure date in *Y-m-d H:i:s* format. | array, string  |
| arrive_at               | *no*     | The arrive date in *Y-m-d H:i:s* format.    | array, string  |
| available_seats         | *no*     | Flights with available seats.               | array, integer |
| minimum_seats           | *no*     | Flights with minimum seats for ticketing.   | array, integer |

<aside class="notice">
Some parameters allow both array and integer/string values. If array is sent, it must have the following structure:
    <code>
    {
        "condition":">=",
        "value":""
    }
    </code>,
where the <code>condition</code> accepts values like <code>>=</code>, <code>></code>, <code>=</code>, <code><</code> and <code><=</code>.
</aside>

