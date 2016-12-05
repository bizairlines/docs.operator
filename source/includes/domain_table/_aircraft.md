## Aircraft

```shell
$ curl '/v1/aircraft' \
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
    }
  ]
}
```
### HTTP REQUEST
`GET /v1/aircraft`

### List/Table
| ID | Name |
|----|------|
| 1 |   Airbus A300 |
| 2 |   Airbus A310 |
| 3 |   AIRBUS A310-300ER |
| 4 |   AIRBUS A310-300ER VIP |
| 5 |   Airbus A318 |
| 6 |   Airbus A318 ELITE |
| 7 |   Airbus A319 |
| 8 |   Airbus A320 |
| 9 |   Airbus A321 |
| 10 |  Airbus A330 |
| 11 |  Airbus A330-200 |
| 12 |  Airbus A340 |
| 13 |  Airbus A350 |
| 14 |  Airbus A380 |
| 15 |  Airbus ACJ 318 |
| 16 |  Airbus ACJ 319 |
| 17 |  Airbus ACJ 320 |
| 18 |  Airbus ACJ 330 |
| 19 |  Airbus ACJ 340 |
| 20 |  Airbus Corportate Jetliner - A319CJ |
| 21 |  Antonov An-140 |
| 22 |  Antonov An-148 |
| 23 |  Antonov An-158 |
| 24 |  Astra SP |
| 25 |  Astra SPX |
| 26 |  ATR 42 |
| 27 |  ATR 72 |
| 28 |  ATR Corporate |
| 29 |  ATR Surveyor |
| 30 |  Beech 1900D |
| 31 |  Beech Baron 58 |
| 32 |  Beechcraft 1900 Airliner |
| 33 |  Beechcraft 1900D VIP |
| 34 |  Beechcraft King Air 100 |
| 35 |  Beechcraft King Air 200 |
| 36 |  Beechcraft King Air 200 Blackhawk |
| 37 |  Beechcraft King Air 250 |
| 38 |  Beechcraft King Air 300 |
| 39 |  Beechcraft King Air 350 |
| 40 |  Beechcraft King Air 350i |
| 41 |  Beechcraft King Air 350iER |
| 42 |  Beechcraft King Air 90 |
| 43 |  Beechcraft King Air C90 |
| 44 |  Beechcraft King Air C90A |
| 45 |  Beechcraft King Air C90B |
| 46 |  Beechcraft King Air C90E |
| 47 |  Beechcraft King Air C90F |
| 48 |  Beechcraft King Air C90GTi |
| 49 |  Beechcraft King Air C90GTX |
| 50 |  Beechcraft Premier I |
| 51 |  Beechcraft Premier IA |
| 52 |  Beechcraft Super King Air 200 |
| 53 |  Beechjet 400 |
| 54 |  Beechjet 400A |
| 55 |  Beriev Be-200 |
| 56 |  Boeing 717 |
| 57 |  Boeing 727 |
| 58 |  Boeing 737 |
| 59 |  Boeing 737 VIP |
| 60 |  Boeing 747 |
| 61 |  Boeing 757 |
| 62 |  Boeing 757 Executive |
| 63 |  Boeing 767 |
| 64 |  Boeing 767-300ER Executive |
| 65 |  Boeing 777 |
| 66 |  Boeing 787 |
| 67 |  Boeing BBJ |
| 68 |  Boeing BBJ 2 |
| 69 |  Boeing BBJ 3 |
| 70 |  Boeing BBJ 747 |
| 71 |  Boeing BBJ 787 |
| 72 |  Boeing BBJ Max 8 |
| 73 |  Boeing BBJ Max 9 |
| 74 |  Boeing Business Jet BBJ |
| 75 |  Boeing MD 83 |
| 76 |  Boeing MD 83 VIP |
| 77 |  Bombardier Challenger 300 |
| 78 |  Bombardier Challenger 350 |
| 79 |  Bombardier Challenger 600 |
| 80 |  Bombardier Challenger 601 |
| 81 |  Bombardier Challenger 601-3A |
| 82 |  Bombardier Challenger 604 |
| 83 |  Bombardier Challenger 605 |
| 84 |  Bombardier Challenger 850 |
| 85 |  Bombardier Challenger SE |
| 86 |  Bombardier CRJ 1000 |
| 87 |  Bombardier CRJ-100 |
| 88 |  Bombardier CRJ-200 |
| 89 |  Bombardier CRJ-700 |
| 90 |  Bombardier CRJ-900 |
| 91 |  Bombardier CS100 |
| 92 |  Bombardier CS300 |
| 93 |  Bombardier Dash 8 |
| 94 |  Bombardier DASH 8-100 |
| 95 |  Bombardier DASH 8-300 |
| 96 |  Bombardier Global 5000 |
| 97 |  Bombardier Global 6000 |
| 98 |  Bombardier Global Express |
| 99 |  Bombardier Global XRS |
| 100 | Bombardier Learjet 31 |
| 101 | Bombardier Learjet 31A |
| 102 | Bombardier Learjet 31ER |
| 103 | Bombardier Learjet 35 |
| 104 | Bombardier Learjet 35A |
| 105 | Bombardier Learjet 40 |
| 106 | Bombardier Learjet 40XR |
| 107 | Bombardier Learjet 45 |
| 108 | Bombardier Learjet 45XR |
| 109 | Bombardier Learjet 55 |
| 110 | Bombardier Learjet 55B |
| 111 | Bombardier Learjet 60 |
| 112 | Bombardier Learjet 60XR |
| 113 | Bombardier Learjet 70 |
| 114 | Bombardier Learjet 75 |
| 115 | Bombardier Regional Jet CRJ |
| 116 | British Aerospace BAe 146 |
| 117 | British Aerospace Jetstream 31 |
| 118 | British Aerospace Jetstream 32 |
| 119 | British Aerospace Jetstream 32EP |
| 120 | British Aerospace Jetstream 41 |
| 121 | Canadair CRJ-100 |
| 122 | Canadair CRJ-200 |
| 123 | CASA C-212 Aviocar |
| 124 | Cessna 182 |
| 125 | Cessna 206 |
| 126 | Cessna 310R |
| 127 | Cessna 340 |
| 128 | Cessna 340A |
| 129 | Cessna 400 |
| 130 | Cessna 402 |
| 131 | Cessna 402B |
| 132 | Cessna 414 |
| 133 | Cessna 414 RAM VI |
| 134 | Cessna 414A |
| 135 | Cessna 421 |
| 136 | Cessna 421A |
| 137 | Cessna 421B |
| 138 | Cessna Caravan 208 Amphibian |
| 139 | Cessna Caravan 208B |
| 140 | Cessna CITATION EXCEL |
| 141 | Cessna CITATION II BRAVO |
| 142 | Cessna CITATION III |
| 143 | Cessna CITATION MUSTANG |
| 144 | Cessna CITATION SOVEREIGN |
| 145 | Cessna CITATION V ULTRA |
| 146 | Cessna CITATION VII |
| 147 | Cessna CITATION X |
| 148 | Cessna CITATIONJET CJ1 |
| 149 | Cessna CITATIONJET CJ2 |
| 150 | Cessna CITATIONJET CJ3 |
| 151 | Cessna CITATIONJET CJ4 |
| 152 | Cessna Conquest I |
| 153 | Cessna Conquest II |
| 154 | Cessna Grand Caravan 208B |
| 155 | Cessna T303 |
| 156 | Cheyenne II |
| 157 | Cheyenne III |
| 158 | Cheyenne IIXL |
| 159 | Chieftan |
| 160 | Cirrus SR 22 |
| 161 | Citation Bravo |
| 162 | Citation CJ |
| 163 | Citation CJ1 |
| 164 | Citation CJ1+ |
| 165 | Citation CJ2 |
| 166 | Citation CJ2+ |
| 167 | Citation CJ3 |
| 168 | Citation CJ3+ |
| 169 | Citation CJ4 |
| 170 | Citation CJ4+ |
| 171 | Citation Encore |
| 172 | Citation Encore+ |
| 173 | Citation Excel |
| 174 | Citation I |
| 175 | Citation I CE-500E |
| 176 | Citation I SP |
| 177 | Citation II |
| 178 | Citation II SP |
| 179 | Citation III |
| 180 | Citation Latitude |
| 181 | Citation M2 |
| 182 | Citation Mustang |
| 183 | Citation SII |
| 184 | Citation Sovereign |
| 185 | Citation Sovereign+ |
| 186 | Citation Ultra |
| 187 | Citation V |
| 188 | Citation VI |
| 189 | Citation VII |
| 190 | Citation X |
| 191 | Citation X+ |
| 192 | Citation XLS |
| 193 | Citation XLS+ |
| 194 | Dash 8-200 |
| 195 | DASSAULT FALCON 10 |
| 196 | DASSAULT FALCON 20 |
| 197 | DASSAULT FALCON 2000 |
| 198 | DASSAULT FALCON 50 |
| 199 | DASSAULT FALCON 7X |
| 200 | DASSAULT FALCON 900 |
| 201 | De Havilland Canada Dash 7 |
| 202 | De Havilland Canada Dash 8 |
| 203 | Diamond DA42 |
| 204 | Diamond EA42 |
| 205 | Dornier 228 Executive |
| 206 | Dornier 328 |
| 207 | Dornier 328 Executive Jet |
| 208 | DORNIER 328 JET |
| 209 | DORNIER 328 JET EXECUTIVE |
| 210 | DORNIER 328 TP |
| 211 | DORNIER 328 TP EXECUTIVE |
| 212 | Eclipse 500 |
| 213 | Eclipse 550 |
| 214 | Embraer 110 Bandeirante |
| 215 | Embraer 120 Brasilia |
| 216 | EMBRAER 170 - E170 |
| 217 | EMBRAER 190 - E190 |
| 218 | Embraer EMB 120 Brasilia  |
| 219 | Embraer EMB 121 Xingu |
| 220 | Embraer ERJ 135 |
| 221 | EMBRAER ERJ 135 JET |
| 222 | Embraer ERJ 140 |
| 223 | Embraer ERJ 145 |
| 224 | EMBRAER ERJ 145 JET |
| 225 | Embraer ERJ 170 |
| 226 | Embraer ERJ 175 |
| 227 | Embraer ERJ 190 |
| 228 | Embraer ERJ 195 |
| 229 | EMBRAER LEGACY |
| 230 | Embraer Legacy 450 |
| 231 | Embraer Legacy 500 |
| 232 | Embraer Legacy 600 |
| 233 | Embraer Legacy 650 |
| 234 | Embraer Lineage 1000 |
| 235 | Embraer Phenom 100 |
| 236 | Embraer Phenom 100E |
| 237 | Embraer Phenom 300 |
| 238 | FAIRCHILD DORNIER METRO 23 |
| 239 | FAIRCHILD MERLIN III |
| 240 | Fairchild Merlin IIIA |
| 241 | Fairchild Merlin IIIC |
| 242 | Fairchild Merlin IV |
| 243 | Fairchild Merlin IVA |
| 244 | Fairchild Metro 23 |
| 245 | Fairchild Metro III Executive |
| 246 | Falcon 10 |
| 247 | Falcon 20 |
| 248 | Falcon 20-C5 |
| 249 | Falcon 200 |
| 250 | Falcon 2000 |
| 251 | Falcon 2000DX |
| 252 | Falcon 2000EX |
| 253 | Falcon 2000EX EASy |
| 254 | Falcon 2000LX |
| 255 | Falcon 2000LXS |
| 256 | Falcon 2000S |
| 257 | Falcon 20F |
| 258 | Falcon 20F-5 |
| 259 | Falcon 50 |
| 260 | Falcon 50B |
| 261 | Falcon 50EX |
| 262 | Falcon 7X |
| 263 | Falcon 900 |
| 264 | Falcon 900B |
| 265 | Falcon 900C |
| 266 | Falcon 900DX |
| 267 | Falcon 900EX |
| 268 | Falcon 900EX EASy |
| 269 | Falcon 900EX-W |
| 270 | Falcon 900LX |
| 271 | Falcon 900LX EASy II |
| 272 | Falcon DA-7X |
| 273 | Fokker 100 |
| 274 | Fokker 50 |
| 275 | Fokker 70 |
| 276 | GULFSTREAM 100 |
| 277 | GULFSTREAM 150 - G150 PRIVATE JET CHARTER |
| 278 | GULFSTREAM 200 |
| 279 | Gulfstream G-100 |
| 280 | Gulfstream G-150 |
| 281 | Gulfstream G-200 |
| 282 | Gulfstream G-280 |
| 283 | Gulfstream G-300 |
| 284 | Gulfstream G-350 |
| 285 | Gulfstream G-400 |
| 286 | Gulfstream G-450 |
| 287 | Gulfstream G-500 |
| 288 | Gulfstream G-550 |
| 289 | Gulfstream G-650 |
| 290 | Gulfstream G-650 ER |
| 291 | Gulfstream IIB |
| 292 | Gulfstream III |
| 293 | Gulfstream IV |
| 294 | GULFSTREAM IV & G450 |
| 295 | Gulfstream IVSP |
| 296 | GULFSTREAM V & G550 |
| 297 | GulfstreamV |
| 298 | Hawker 1000 |
| 299 | Hawker 1000A |
| 300 | HAWKER 400 |
| 301 | Hawker 4000 |
| 302 | Hawker 400A |
| 303 | Hawker 400XP |
| 304 | Hawker 700A |
| 305 | Hawker 700B |
| 306 | Hawker 750 |
| 307 | HAWKER 800 XP |
| 308 | Hawker 800A |
| 309 | Hawker 800B |
| 310 | Hawker 800XP |
| 311 | Hawker 800XPi |
| 312 | Hawker 850XP |
| 313 | Hawker 900XP |
| 314 | Ilyushin Il-114 |
| 315 | Ilyushin Il-96 |
| 316 | McDonnell Douglas MD-80 |
| 317 | McDonnell Douglas MD-90 |
| 318 | Nextant 400XTi |
| 319 | Nextant XT |
| 320 | Piaggio Avanti |
| 321 | Piaggio Avanti II |
| 322 | PIAGGIO P180 AVANTI |
| 323 | Pilatus PC-12 |
| 324 | Pilatus PC-12/45 |
| 325 | Pilatus PC-12/47 |
| 326 | Pilatus PC-12/47E |
| 327 | Pilatus PC-6 |
| 328 | Piper Aerostar 600 |
| 329 | Piper Aztec |
| 330 | Piper Cheyenne |
| 331 | Piper Chieftain |
| 332 | Piper Malibu Mirage |
| 333 | Piper Matrix |
| 334 | Piper Meridian |
| 335 | Piper PA-31 |
| 336 | Piper PA-31 Navajo |
| 337 | Piper PA-31 Seneca |
| 338 | Piper PA-46 |
| 339 | Piper Saratoga |
| 340 | Saab 2000 |
| 341 | Saab 340A |
| 342 | Sabreliner 65 |
| 343 | Sukhoi Superjet 100 |
| 344 | Tupolev Tu-204 |
| 345 | Westwind I |
| 346 | Westwind II |
| 347 | Sikorsky S-76 C+ |
| 348 | Cessna CITATION II |
| 349 | Light Jet |
| 350 | Midsized Jet |
| 351 | Heavy Jet |
| 352 | Mitsubishi MU2B |

### FILTERS
| Parameter | Required | Description                                                                               | Format  |
|-----------|----------|-------------------------------------------------------------------------------------------|---------|
| page      | *no*     | The number of the page.                                                                   | integer |
| sort      | *no*     | The column to sort the information. Default: `id`.                                        | integer |
| order     | *no*     | The direction to do the sorting. Available only `asc` and `desc` options. Default: `asc`. | integer |

### Autocomplete

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

`GET /v1/aircraft/autocomplete`

| Parameter | Required | Description                      | Format |
|-----------|----------|----------------------------------|--------|
| s         | *no*     | The term you want to search for. | string |
