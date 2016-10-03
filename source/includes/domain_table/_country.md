## Countries
> `GET /v1/countries`

```shell
$ curl '/v1/countries' \
    -H 'Content-type: application/json'
```

> Example response

```
{
  "data": [
    {
      "id": 234,
      "name": "United States",
      "iso_code_2": "US",
      "iso_code_3": "USA",
      "area_code": "1",
      "order": 3,
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 233,
      "name": "United Kingdom",
      "iso_code_2": "GB",
      "iso_code_3": "GBR",
      "area_code": "44",
      "order": 2,
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 39,
      "name": "Canada",
      "iso_code_2": "CA",
      "iso_code_3": "CAN",
      "area_code": "1",
      "order": 1,
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    },
    {
      "id": 1,
      "name": "Afghanistan",
      "iso_code_2": "AF",
      "iso_code_3": "AFG",
      "area_code": "93",
      "order": null,
      "created_at": "2016-08-03 21:17:21",
      "updated_at": "2016-08-03 21:17:21"
    }
  ]
}
```

Return the list of countries ordered by the attribute `order` where the countries with `null` value are the lasts.

| ID | Name | ISO Code 2 | ISO Code 3 |
|----|------|------------|------------|
| 1 |   Afghanistan  | AF  | AFG |
| 2 |   Albania  | AL  | ALB |
| 3 |   Algeria  | DZ  | DZA |
| 4 |   American Samoa   | AS  | ASM |
| 5 |   Andorra  | AD  | AND |
| 6 |   Angola   | AO  | AGO |
| 7 |   Anguilla     | AI  | AIA |
| 8 |   Antarctica   | AQ  | ATA |
| 9 |   Antigua & Barbuda    | AG  | ATG |
| 10 |  Argentina    | AR  | ARG |
| 11 |  Armenia  | AM  | ARM |
| 12 |  Aruba    | AW  | ABW |
| 13 |  Australia    | AU  | AUS |
| 14 |  Austria  | AT  | AUT |
| 15 |  Azerbaijan   | AZ  | AZE |
| 16 |  Bahamas  | BS  | BHS |
| 17 |  Bahrain  | BH  | BHR |
| 18 |  Bangladesh   | BD  | BGD |
| 19 |  Barbados     | BB  | BRB |
| 20 |  Belarus  | BY  | BLR |
| 21 |  Belgium  | BE  | BEL |
| 22 |  Belize   | BZ  | BLZ |
| 23 |  Benin    | BJ  | BEN |
| 24 |  Bermuda  | BM  | BMU |
| 25 |  Bhutan   | BT  | BTN |
| 26 |  Bolivia  | BO  | BOL |
| 27 |  Bosnia   | BA  | BIH |
| 28 |  Botswana     | BW  | BWA |
| 29 |  Bouvet Island    | BV  | BVT |
| 30 |  Brazil   | BR  | BRA |
| 31 |  British Indian Ocean Territory   | IO  | IOT |
| 32 |  British Virgin Islands   | VG  | VGB |
| 33 |  Brunei   | BN  | BRN |
| 34 |  Bulgaria     | BG  | BGR |
| 35 |  Burkina Faso     | BF  | BFA |
| 36 |  Burundi  | BI  | BDI |
| 37 |  Cambodia     | KH  | KHM |
| 38 |  Cameroon     | CM  | CMR |
| 39 |  Canada   | CA  | CAN |
| 40 |  Cape Verde   | CV  | CPV |
| 41 |  Caribbean Netherlands    | BQ  | BES |
| 42 |  Cayman Islands   | KY  | CYM |
| 43 |  Central African Republic     | CF  | CAF |
| 44 |  Chad     | TD  | TCD |
| 45 |  Chile    | CL  | CHL |
| 46 |  China    | CN  | CHN |
| 47 |  Christmas Island     | CX  | CXR |
| 48 |  Cocos (Keeling) Islands  | CC  | CCK |
| 49 |  Colombia     | CO  | COL |
| 50 |  Comoros  | KM  | COM |
| 51 |  Congo - Brazzaville  | CG  | COG |
| 52 |  Congo - Kinshasa     | CD  | COD |
| 53 |  Cook Islands     | CK  | COK |
| 54 |  Costa Rica   | CR  | CRI |
| 55 |  Croatia  | HR  | HRV |
| 56 |  Cuba     | CU  | CUB |
| 57 |  Curaçao  | CW  | CUW |
| 58 |  Cyprus   | CY  | CYP |
| 59 |  Czech Republic   | CZ  | CZE |
| 60 |  Côte d’Ivoire    | CI  | CIV |
| 61 |  Denmark  | DK  | DNK |
| 62 |  Djibouti     | DJ  | DJI |
| 63 |  Dominica     | DM  | DMA |
| 64 |  Dominican Republic   | DO  | DOM |
| 65 |  Ecuador  | EC  | ECU |
| 66 |  Egypt    | EG  | EGY |
| 67 |  El Salvador  | SV  | SLV |
| 68 |  Equatorial Guinea    | GQ  | GNQ |
| 69 |  Eritrea  | ER  | ERI |
| 70 |  Estonia  | EE  | EST |
| 71 |  Ethiopia     | ET  | ETH |
| 72 |  Falkland Islands     | FK  | FLK |
| 73 |  Faroe Islands    | FO  | FRO |
| 74 |  Fiji     | FJ  | FJI |
| 75 |  Finland  | FI  | FIN |
| 76 |  France   | FR  | FRA |
| 77 |  French Guiana    | GF  | GUF |
| 78 |  French Polynesia     | PF  | PYF |
| 79 |  French Southern Territories  | TF  | ATF |
| 80 |  Gabon    | GA  | GAB |
| 81 |  Gambia   | GM  | GMB |
| 82 |  Georgia  | GE  | GEO |
| 83 |  Germany  | DE  | DEU |
| 84 |  Ghana    | GH  | GHA |
| 85 |  Gibraltar    | GI  | GIB |
| 86 |  Greece   | GR  | GRC |
| 87 |  Greenland    | GL  | GRL |
| 88 |  Grenada  | GD  | GRD |
| 89 |  Guadeloupe   | GP  | GLP |
| 90 |  Guam     | GU  | GUM |
| 91 |  Guatemala    | GT  | GTM |
| 92 |  Guernsey     | GG  | GGY |
| 93 |  Guinea   | GN  | GIN |
| 94 |  Guinea-Bissau    | GW  | GNB |
| 95 |  Guyana   | GY  | GUY |
| 96 |  Haiti    | HT  | HTI |
| 97 |  Heard & McDonald Islands     | HM  | HMD |
| 98 |  Honduras     | HN  | HND |
| 99 |  Hong Kong    | HK  | HKG |
| 100 | Hungary  | HU  | HUN |
| 101 | Iceland  | IS  | ISL |
| 102 | India    | IN  | IND |
| 103 | Indonesia    | ID  | IDN |
| 104 | Iran     | IR  | IRN |
| 105 | Iraq     | IQ  | IRQ |
| 106 | Ireland  | IE  | IRL |
| 107 | Isle of Man  | IM  | IMN |
| 108 | Israel   | IL  | ISR |
| 109 | Italy    | IT  | ITA |
| 110 | Jamaica  | JM  | JAM |
| 111 | Japan    | JP  | JPN |
| 112 | Jersey   | JE  | JEY |
| 113 | Jordan   | JO  | JOR |
| 114 | Kazakhstan   | KZ  | KAZ |
| 115 | Kenya    | KE  | KEN |
| 116 | Kiribati     | KI  | KIR |
| 117 | Kuwait   | KW  | KWT |
| 118 | Kyrgyzstan   | KG  | KGZ |
| 119 | Laos     | LA  | LAO |
| 120 | Latvia   | LV  | LVA |
| 121 | Lebanon  | LB  | LBN |
| 122 | Lesotho  | LS  | LSO |
| 123 | Liberia  | LR  | LBR |
| 124 | Libya    | LY  | LBY |
| 125 | Liechtenstein    | LI  | LIE |
| 126 | Lithuania    | LT  | LTU |
| 127 | Luxembourg   | LU  | LUX |
| 128 | Macau    | MO  | MAC |
| 129 | Macedonia    | MK  | MKD |
| 130 | Madagascar   | MG  | MDG |
| 131 | Malawi   | MW  | MWI |
| 132 | Malaysia     | MY  | MYS |
| 133 | Maldives     | MV  | MDV |
| 134 | Mali     | ML  | MLI |
| 135 | Malta    | MT  | MLT |
| 136 | Marshall Islands     | MH  | MHL |
| 137 | Martinique   | MQ  | MTQ |
| 138 | Mauritania   | MR  | MRT |
| 139 | Mauritius    | MU  | MUS |
| 140 | Mayotte  | YT  | MYT |
| 141 | Mexico   | MX  | MEX |
| 142 | Micronesia   | FM  | FSM |
| 143 | Moldova  | MD  | MDA |
| 144 | Monaco   | MC  | MCO |
| 145 | Mongolia     | MN  | MNG |
| 146 | Montenegro   | ME  | MNE |
| 147 | Montserrat   | MS  | MSR |
| 148 | Morocco  | MA  | MAR |
| 149 | Mozambique   | MZ  | MOZ |
| 150 | Myanmar  | MM  | MMR |
| 151 | Namibia  | NA  | NAM |
| 152 | Nauru    | NR  | NRU |
| 153 | Nepal    | NP  | NPL |
| 154 | Netherlands  | NL  | NLD |
| 155 | New Caledonia    | NC  | NCL |
| 156 | New Zealand  | NZ  | NZL |
| 157 | Nicaragua    | NI  | NIC |
| 158 | Niger    | NE  | NER |
| 159 | Nigeria  | NG  | NGA |
| 160 | Niue     | NU  | NIU |
| 161 | Norfolk Island   | NF  | NFK |
| 162 | North Korea  | KP  | PRK |
| 163 | Northern Mariana Islands     | MP  | MNP |
| 164 | Norway   | NO  | NOR |
| 165 | Oman     | OM  | OMN |
| 166 | Pakistan     | PK  | PAK |
| 167 | Palau    | PW  | PLW |
| 168 | Palestine    | PS  | PSE |
| 169 | Panama   | PA  | PAN |
| 170 | Papua New Guinea     | PG  | PNG |
| 171 | Paraguay     | PY  | PRY |
| 172 | Peru     | PE  | PER |
| 173 | Philippines  | PH  | PHL |
| 174 | Pitcairn Islands     | PN  | PCN |
| 175 | Poland   | PL  | POL |
| 176 | Portugal     | PT  | PRT |
| 177 | Puerto Rico  | PR  | PRI |
| 178 | Qatar    | QA  | QAT |
| 179 | Romania  | RO  | ROU |
| 180 | Russia   | RU  | RUS |
| 181 | Rwanda   | RW  | RWA |
| 182 | Réunion  | RE  | REU |
| 183 | Samoa    | WS  | WSM |
| 184 | San Marino   | SM  | SMR |
| 185 | Saudi Arabia     | SA  | SAU |
| 186 | Senegal  | SN  | SEN |
| 187 | Serbia   | RS  | SRB |
| 188 | Seychelles   | SC  | SYC |
| 189 | Sierra Leone     | SL  | SLE |
| 190 | Singapore    | SG  | SGP |
| 191 | Sint Maarten     | SX  | SXM |
| 192 | Slovakia     | SK  | SVK |
| 193 | Slovenia     | SI  | SVN |
| 194 | Solomon Islands  | SB  | SLB |
| 195 | Somalia  | SO  | SOM |
| 196 | South Africa     | ZA  | ZAF |
| 197 | South Georgia & South Sandwich Islands   | GS  | SGS |
| 198 | South Korea  | KR  | KOR |
| 199 | South Sudan  | SS  | SSD |
| 200 | Spain    | ES  | ESP |
| 201 | Sri Lanka    | LK  | LKA |
| 202 | St. Barthélemy   | BL  | BLM |
| 203 | St. Helena   | SH  | SHN |
| 204 | St. Kitts & Nevis    | KN  | KNA |
| 205 | St. Lucia    | LC  | LCA |
| 206 | St. Martin   | MF  | MAF |
| 207 | St. Pierre & Miquelon    | PM  | SPM |
| 208 | St. Vincent & Grenadines     | VC  | VCT |
| 209 | Sudan    | SD  | SDN |
| 210 | Suriname     | SR  | SUR |
| 211 | Svalbard & Jan Mayen     | SJ  | SJM |
| 212 | Swaziland    | SZ  | SWZ |
| 213 | Sweden   | SE  | SWE |
| 214 | Switzerland  | CH  | CHE |
| 215 | Syria    | SY  | SYR |
| 216 | São Tomé & Príncipe  | ST  | STP |
| 217 | Taiwan   | TW  | TWN |
| 218 | Tajikistan   | TJ  | TJK |
| 219 | Tanzania     | TZ  | TZA |
| 220 | Thailand     | TH  | THA |
| 221 | Timor-Leste  | TL  | TLS |
| 222 | Togo     | TG  | TGO |
| 223 | Tokelau  | TK  | TKL |
| 224 | Tonga    | TO  | TON |
| 225 | Trinidad & Tobago    | TT  | TTO |
| 226 | Tunisia  | TN  | TUN |
| 227 | Turkey   | TR  | TUR |
| 228 | Turkmenistan     | TM  | TKM |
| 229 | Turks & Caicos Islands   | TC  | TCA |
| 230 | Tuvalu   | TV  | TUV |
| 231 | U.S. Outlying Islands    | UM  | UMI |
| 232 | U.S. Virgin Islands  | VI  | VIR |
| 233 | United Kingdom   | GB  | GBR |
| 234 | United States    | US  | USA |
| 235 | Uganda   | UG  | UGA |
| 236 | Ukraine  | UA  | UKR |
| 237 | United Arab Emirates     | AE  | ARE |
| 238 | Uruguay  | UY  | URY |
| 239 | Uzbekistan   | UZ  | UZB |
| 240 | Vanuatu  | VU  | VUT |
| 241 | Vatican City     | VA  | VAT |
| 242 | Venezuela    | VE  | VEN |
| 243 | Vietnam  | VN  | VNM |
| 244 | Wallis & Futuna  | WF  | WLF |
| 245 | Western Sahara   | EH  | ESH |
| 246 | Yemen    | YE  | YEM |
| 247 | Zambia   | ZM  | ZMB |
| 248 | Zimbabwe     | ZW  | ZWE |
| 249 | Åland Islands    | AX  | ALA |
