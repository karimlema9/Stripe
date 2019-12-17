# Stripe

## CRUD

1. [List Cards](https://github.com/karimlema9/Stripe/blob/master/Stripe/Cards/Cards.md#list) </br>
1.1 [Ceate Card](https://github.com/karimlema9/Stripe/blob/master/Stripe/Cards/Cards.md#create) </br>
1.2 [Update Card](https://github.com/karimlema9/Stripe/blob/master/Stripe/Cards/Cards.md#update) </br>
1.3 [Delete Card](https://github.com/karimlema9/Stripe/blob/master/Stripe/Cards/Cards.md#delete) </br>
2. [List Subscriptions](https://github.com/karimlema9/Stripe/blob/master/Stripe/Suscriptions/Suscriptions.md#list) </br>
2.1 [Ceate Subscriptions](https://github.com/karimlema9/Stripe/blob/master/Stripe/Suscriptions/Suscriptions.md#create) </br>
2.2 [Update Subscriptions](https://github.com/karimlema9/Stripe/blob/master/Stripe/Suscriptions/Suscriptions.md#update) </br>
2.3 [Cancel Subscriptions](https://github.com/karimlema9/Stripe/blob/master/Stripe/Suscriptions/Suscriptions.md#cancel) 

# Index

1. [Travels](#Travels) </br>
1.1 [List](#List) </br>
1.2 [List Day](#ListDay) </br>
1.3 [List Week](#ListDay) </br>
1.4 [List Month](#ListDay) </br>
1.5 [Show](#Show) </br>
1.6 [Create](#Create) </br>
1.7 [Update](#Update) </br>
1.8 [Delete](#Delete) </br>
1.9 [Status](#Status) </br>

2. [Addresses](#Addresses) </br>
2.1 [List](#addresses-List) </br>
2.2 [Show](#Show) </br>
2.3 [Create](#Create) </br>
2.4 [Update](#Update) </br>
2.5 [Delete](#Delete) </br>
2.6 [Countries](#upCountriesdate) </br>

1. [Client](#Client) </br>
3.1 [List](#List) </br>
3.2 [Show](#Show) </br>
3.3 [Create](#Create) </br>
3.4 [Update](#Update) </br>
3.5 [Delete](#Delete) </br>

# Travels
## List
> **GET** https://api.hardman.app/api/v2/travels

List all travels

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |

### Response
~~~json
{
            "id": 21,
            "hardman_identifier": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
            "date_start": "2019-12-02",
            "date_end": "2019-12-24",
            "driver_id": null,
            "driver": null,
            "customer_id": 6,
            "customer": {
                "id": 6,
                "name": "Tralavel Oslo SL",
                "vat_number": "65985645",
                "email": "modegaard@tralaveloslo.com",
                "phone": "+47625348579",
                "contact_name": "Martin Odegaard",
                "address1": "Stenersgata 1, 0050 Oslo, Noruega",
                "address2": null,
                "city": "Barcelona",
                "state": "Oslo kommune",
                "postal_code": "0050",
                "shipping_address1": null,
                "shipping_address2": null,
                "shipping_city": null,
                "shipping_state": null,
                "shipping_postal_code": null,
                "tenant_id": null,
                "country": {
                    "id": 578,
                    "iso_3166_2": "NO",
                    "iso_3166_3": "NOR",
                    "name": "Norway",
                    "swap_postal_code": false,
                    "swap_currency_symbol": false,
                    "thousand_separator": null,
                    "decimal_separator": null
                }
            },
            "primary_regno_id": null,
            "primary_regno": null,
            "secondary_regno_id": null,
            "secondary_regno": null,
            "price_client": 0,
            "price_driver": 0,
            "routeA": {
                "id": 31,
                "travel": {
                    "id": 21,
                    "customer_id": 6,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-02 00:00:00",
                    "date_end": "2019-12-24 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-02 14:40:35",
                    "updated_at": "2019-12-02 14:40:35",
                    "deleted_at": null
                },
                "travel_id": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
                "order": 0,
                "load": 1,
                "address": {
                    "id": 1,
                    "name": "Catedral de Barcelona",
                    "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                    "city": "Barcelona",
                    "country_id": 724,
                    "country": {
                        "id": 724,
                        "iso_3166_2": "ES",
                        "iso_3166_3": "ESP",
                        "name": "Spain",
                        "swap_postal_code": true,
                        "swap_currency_symbol": true,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "08002",
                    "phone": "+34 632548759",
                    "email": "sfernandez@tralavelbarcelona.com",
                    "contact_name": "Sergio Fernandez",
                    "latitude": 41.383962,
                    "longitude": 2.1761990999999625
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "routeB": {
                "id": 31,
                "travel": {
                    "id": 21,
                    "customer_id": 6,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-02 00:00:00",
                    "date_end": "2019-12-24 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-02 14:40:35",
                    "updated_at": "2019-12-02 14:40:35",
                    "deleted_at": null
                },
                "travel_id": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
                "order": 0,
                "load": 1,
                "address": {
                    "id": 1,
                    "name": "Catedral de Barcelona",
                    "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                    "city": "Barcelona",
                    "country_id": 724,
                    "country": {
                        "id": 724,
                        "iso_3166_2": "ES",
                        "iso_3166_3": "ESP",
                        "name": "Spain",
                        "swap_postal_code": true,
                        "swap_currency_symbol": true,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "08002",
                    "phone": "+34 632548759",
                    "email": "sfernandez@tralavelbarcelona.com",
                    "contact_name": "Sergio Fernandez",
                    "latitude": 41.383962,
                    "longitude": 2.1761990999999625
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "offered": false,
            "accepted": false,
            "status_id": 1,
            "status": {
                "id": 1,
                "name": "Draft",
                "color": "#a9aaba",
                "description": null,
                "deleted_at": null,
                "created_at": "2019-11-19 10:52:44",
                "updated_at": "2019-12-09 12:27:42",
                "priority": 2
            },
            "priority": 2,
            "phases": [
                {
                    "id": 31,
                    "travel": {
                        "id": 21,
                        "customer_id": 6,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-02 00:00:00",
                        "date_end": "2019-12-24 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-02 14:40:35",
                        "updated_at": "2019-12-02 14:40:35",
                        "deleted_at": null
                    },
                    "travel_id": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
                    "order": 0,
                    "load": 1,
                    "address": {
                        "id": 1,
                        "name": "Catedral de Barcelona",
                        "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                        "city": "Barcelona",
                        "country_id": 724,
                        "country": {
                            "id": 724,
                            "iso_3166_2": "ES",
                            "iso_3166_3": "ESP",
                            "name": "Spain",
                            "swap_postal_code": true,
                            "swap_currency_symbol": true,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "08002",
                        "phone": "+34 632548759",
                        "email": "sfernandez@tralavelbarcelona.com",
                        "contact_name": "Sergio Fernandez",
                        "latitude": 41.383962,
                        "longitude": 2.1761990999999625
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                }
            ],
            "incidences": [],
            "created_at": "2019-12-02T13:40:35.000000Z",
            "updated_at": "2019-12-02T13:40:35.000000Z",
            "modifiable": true,
            "custom_inputs": [],
            "owner": "3",
            "transferred": true,
            "contract_to": {
                "id": 201,
                "to": {
                    "id": 4,
                    "name": "Ikazia Hospital Rotterdam",
                    "address1": "Montessoriweg 1, 3083 AN Rotterdam, Países Bajos",
                    "address2": null,
                    "city": "Rotterdam",
                    "state": "Rotterdam",
                    "postal_code": "3083 AN",
                    "vat_number": "PB-475858585"
                },
                "status": true,
                "created_at": "2019-12-09T07:49:32.000000Z"
            }
        },
        ...
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 0101 | Travel not found |

## List Day
> **POST** https://api.hardman.app/api/v2/travels/day

List one-day travels

### Parameters
| Key  | Description   | Validation |
| ---- | ------------- | ---------- |
| date | Data of a day | Required   |


### Response
~~~json
        {
            "id": 28,
            "hardman_identifier": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
            "date_start": "2019-12-12",
            "date_end": "2019-12-28",
            "driver_id": null,
            "driver": null,
            "customer_id": 5,
            "customer": {
                "id": 5,
                "name": "Tralavel Barcelona SL",
                "vat_number": "15689574",
                "email": null,
                "phone": null,
                "contact_name": null,
                "address1": "Pla de la Seu, s/n, 08002 Barcelona, España",
                "address2": null,
                "city": "Barcelona",
                "state": "Barcelona",
                "postal_code": "08002",
                "shipping_address1": null,
                "shipping_address2": null,
                "shipping_city": null,
                "shipping_state": null,
                "shipping_postal_code": null,
                "tenant_id": null,
                "country": {
                    "id": 724,
                    "iso_3166_2": "ES",
                    "iso_3166_3": "ESP",
                    "name": "Spain",
                    "swap_postal_code": true,
                    "swap_currency_symbol": true,
                    "thousand_separator": null,
                    "decimal_separator": null
                }
            },
            "primary_regno_id": null,
            "primary_regno": null,
            "secondary_regno_id": null,
            "secondary_regno": null,
            "price_client": 0,
            "price_driver": 0,
            "routeA": {
                "id": 42,
                "travel": {
                    "id": 28,
                    "customer_id": 5,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-12 00:00:00",
                    "date_end": "2019-12-28 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-12 11:29:08",
                    "updated_at": "2019-12-12 12:02:49",
                    "deleted_at": null
                },
                "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                "order": 0,
                "load": 1,
                "address": {
                    "id": 1,
                    "name": "Catedral de Barcelona",
                    "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                    "city": "Barcelona",
                    "country_id": 724,
                    "country": {
                        "id": 724,
                        "iso_3166_2": "ES",
                        "iso_3166_3": "ESP",
                        "name": "Spain",
                        "swap_postal_code": true,
                        "swap_currency_symbol": true,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "08002",
                    "phone": "+34 632548759",
                    "email": "sfernandez@tralavelbarcelona.com",
                    "contact_name": "Sergio Fernandez",
                    "latitude": 41.383962,
                    "longitude": 2.1761990999999625
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "routeB": {
                "id": 43,
                "travel": {
                    "id": 28,
                    "customer_id": 5,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-12 00:00:00",
                    "date_end": "2019-12-28 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-12 11:29:08",
                    "updated_at": "2019-12-12 12:02:49",
                    "deleted_at": null
                },
                "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                "order": 1,
                "load": 0,
                "address": {
                    "id": 2,
                    "name": "Oslo City",
                    "address": "Stenersgata 1, 0050 Oslo, Noruega",
                    "city": "Oslo",
                    "country_id": 578,
                    "country": {
                        "id": 578,
                        "iso_3166_2": "NO",
                        "iso_3166_3": "NOR",
                        "name": "Norway",
                        "swap_postal_code": false,
                        "swap_currency_symbol": false,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "0050",
                    "phone": "+4 7625348579",
                    "email": "modegaard@tralaveloslo.com",
                    "contact_name": "Martin Odegaard",
                    "latitude": 59.9126918,
                    "longitude": 10.752917000000025
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "offered": false,
            "accepted": false,
            "status_id": 1,
            "status": {
                "id": 1,
                "name": "Draft",
                "color": "#a9aaba",
                "description": null,
                "deleted_at": null,
                "created_at": "2019-11-19 10:52:44",
                "updated_at": "2019-12-09 12:27:42",
                "priority": 2
            },
            "priority": 2,
            "phases": [
                {
                    "id": 42,
                    "travel": {
                        "id": 28,
                        "customer_id": 5,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-12 00:00:00",
                        "date_end": "2019-12-28 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-12 11:29:08",
                        "updated_at": "2019-12-12 12:02:49",
                        "deleted_at": null
                    },
                    "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                    "order": 0,
                    "load": 1,
                    "address": {
                        "id": 1,
                        "name": "Catedral de Barcelona",
                        "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                        "city": "Barcelona",
                        "country_id": 724,
                        "country": {
                            "id": 724,
                            "iso_3166_2": "ES",
                            "iso_3166_3": "ESP",
                            "name": "Spain",
                            "swap_postal_code": true,
                            "swap_currency_symbol": true,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "08002",
                        "phone": "+34 632548759",
                        "email": "sfernandez@tralavelbarcelona.com",
                        "contact_name": "Sergio Fernandez",
                        "latitude": 41.383962,
                        "longitude": 2.1761990999999625
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                },
                {
                    "id": 43,
                    "travel": {
                        "id": 28,
                        "customer_id": 5,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-12 00:00:00",
                        "date_end": "2019-12-28 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-12 11:29:08",
                        "updated_at": "2019-12-12 12:02:49",
                        "deleted_at": null
                    },
                    "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                    "order": 1,
                    "load": 0,
                    "address": {
                        "id": 2,
                        "name": "Oslo City",
                        "address": "Stenersgata 1, 0050 Oslo, Noruega",
                        "city": "Oslo",
                        "country_id": 578,
                        "country": {
                            "id": 578,
                            "iso_3166_2": "NO",
                            "iso_3166_3": "NOR",
                            "name": "Norway",
                            "swap_postal_code": false,
                            "swap_currency_symbol": false,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "0050",
                        "phone": "+4 7625348579",
                        "email": "modegaard@tralaveloslo.com",
                        "contact_name": "Martin Odegaard",
                        "latitude": 59.9126918,
                        "longitude": 10.752917000000025
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                }
            ],
            "incidences": [],
            "created_at": "2019-12-12T10:29:08.000000Z",
            "updated_at": "2019-12-12T11:02:49.000000Z",
            "modifiable": true,
            "custom_inputs": [],
            "owner": "3",
            "transferred": false,
            "contract_to": null
        },
        ...
~~~

### Errors
| Code | Message |
| ---- | ------- |
| 0201 | Travel not found |

## List Week
> **POST** https://api.hardman.app/api/v2/travels/week

List one-week travels

### Parameters
| Key  | Description   | Validation |
| ---- | ------------- | ---------- |
| date | Data of a day | Required   |

### Response
~~~json
        {
            "id": 28,
            "hardman_identifier": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
            "date_start": "2019-12-12",
            "date_end": "2019-12-28",
            "driver_id": null,
            "driver": null,
            "customer_id": 5,
            "customer": {
                "id": 5,
                "name": "Tralavel Barcelona SL",
                "vat_number": "15689574",
                "email": null,
                "phone": null,
                "contact_name": null,
                "address1": "Pla de la Seu, s/n, 08002 Barcelona, España",
                "address2": null,
                "city": "Barcelona",
                "state": "Barcelona",
                "postal_code": "08002",
                "shipping_address1": null,
                "shipping_address2": null,
                "shipping_city": null,
                "shipping_state": null,
                "shipping_postal_code": null,
                "tenant_id": null,
                "country": {
                    "id": 724,
                    "iso_3166_2": "ES",
                    "iso_3166_3": "ESP",
                    "name": "Spain",
                    "swap_postal_code": true,
                    "swap_currency_symbol": true,
                    "thousand_separator": null,
                    "decimal_separator": null
                }
            },
            "primary_regno_id": null,
            "primary_regno": null,
            "secondary_regno_id": null,
            "secondary_regno": null,
            "price_client": 0,
            "price_driver": 0,
            "routeA": {
                "id": 42,
                "travel": {
                    "id": 28,
                    "customer_id": 5,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-12 00:00:00",
                    "date_end": "2019-12-28 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-12 11:29:08",
                    "updated_at": "2019-12-12 12:02:49",
                    "deleted_at": null
                },
                "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                "order": 0,
                "load": 1,
                "address": {
                    "id": 1,
                    "name": "Catedral de Barcelona",
                    "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                    "city": "Barcelona",
                    "country_id": 724,
                    "country": {
                        "id": 724,
                        "iso_3166_2": "ES",
                        "iso_3166_3": "ESP",
                        "name": "Spain",
                        "swap_postal_code": true,
                        "swap_currency_symbol": true,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "08002",
                    "phone": "+34 632548759",
                    "email": "sfernandez@tralavelbarcelona.com",
                    "contact_name": "Sergio Fernandez",
                    "latitude": 41.383962,
                    "longitude": 2.1761990999999625
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "routeB": {
                "id": 43,
                "travel": {
                    "id": 28,
                    "customer_id": 5,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-12 00:00:00",
                    "date_end": "2019-12-28 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-12 11:29:08",
                    "updated_at": "2019-12-12 12:02:49",
                    "deleted_at": null
                },
                "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                "order": 1,
                "load": 0,
                "address": {
                    "id": 2,
                    "name": "Oslo City",
                    "address": "Stenersgata 1, 0050 Oslo, Noruega",
                    "city": "Oslo",
                    "country_id": 578,
                    "country": {
                        "id": 578,
                        "iso_3166_2": "NO",
                        "iso_3166_3": "NOR",
                        "name": "Norway",
                        "swap_postal_code": false,
                        "swap_currency_symbol": false,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "0050",
                    "phone": "+4 7625348579",
                    "email": "modegaard@tralaveloslo.com",
                    "contact_name": "Martin Odegaard",
                    "latitude": 59.9126918,
                    "longitude": 10.752917000000025
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "offered": false,
            "accepted": false,
            "status_id": 1,
            "status": {
                "id": 1,
                "name": "Draft",
                "color": "#a9aaba",
                "description": null,
                "deleted_at": null,
                "created_at": "2019-11-19 10:52:44",
                "updated_at": "2019-12-09 12:27:42",
                "priority": 2
            },
            "priority": 2,
            "phases": [
                {
                    "id": 42,
                    "travel": {
                        "id": 28,
                        "customer_id": 5,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-12 00:00:00",
                        "date_end": "2019-12-28 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-12 11:29:08",
                        "updated_at": "2019-12-12 12:02:49",
                        "deleted_at": null
                    },
                    "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                    "order": 0,
                    "load": 1,
                    "address": {
                        "id": 1,
                        "name": "Catedral de Barcelona",
                        "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                        "city": "Barcelona",
                        "country_id": 724,
                        "country": {
                            "id": 724,
                            "iso_3166_2": "ES",
                            "iso_3166_3": "ESP",
                            "name": "Spain",
                            "swap_postal_code": true,
                            "swap_currency_symbol": true,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "08002",
                        "phone": "+34 632548759",
                        "email": "sfernandez@tralavelbarcelona.com",
                        "contact_name": "Sergio Fernandez",
                        "latitude": 41.383962,
                        "longitude": 2.1761990999999625
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                },
                {
                    "id": 43,
                    "travel": {
                        "id": 28,
                        "customer_id": 5,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-12 00:00:00",
                        "date_end": "2019-12-28 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-12 11:29:08",
                        "updated_at": "2019-12-12 12:02:49",
                        "deleted_at": null
                    },
                    "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                    "order": 1,
                    "load": 0,
                    "address": {
                        "id": 2,
                        "name": "Oslo City",
                        "address": "Stenersgata 1, 0050 Oslo, Noruega",
                        "city": "Oslo",
                        "country_id": 578,
                        "country": {
                            "id": 578,
                            "iso_3166_2": "NO",
                            "iso_3166_3": "NOR",
                            "name": "Norway",
                            "swap_postal_code": false,
                            "swap_currency_symbol": false,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "0050",
                        "phone": "+4 7625348579",
                        "email": "modegaard@tralaveloslo.com",
                        "contact_name": "Martin Odegaard",
                        "latitude": 59.9126918,
                        "longitude": 10.752917000000025
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                }
            ],
            "incidences": [],
            "created_at": "2019-12-12T10:29:08.000000Z",
            "updated_at": "2019-12-12T11:02:49.000000Z",
            "modifiable": true,
            "custom_inputs": [],
            "owner": "3",
            "transferred": false,
            "contract_to": null
        },
        ...
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 0301 | Travel not found |

## List Month
> **POST** https://api.hardman.app/api/v2/travels/month

List one-month travels

### Parameters
| Key  | Description   | Validation |
| ---- | ------------- | ---------- |
| date | Data of a day | Required   |

### Response
~~~json
        {
            "id": 28,
            "hardman_identifier": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
            "date_start": "2019-12-12",
            "date_end": "2019-12-28",
            "driver_id": null,
            "driver": null,
            "customer_id": 5,
            "customer": {
                "id": 5,
                "name": "Tralavel Barcelona SL",
                "vat_number": "15689574",
                "email": null,
                "phone": null,
                "contact_name": null,
                "address1": "Pla de la Seu, s/n, 08002 Barcelona, España",
                "address2": null,
                "city": "Barcelona",
                "state": "Barcelona",
                "postal_code": "08002",
                "shipping_address1": null,
                "shipping_address2": null,
                "shipping_city": null,
                "shipping_state": null,
                "shipping_postal_code": null,
                "tenant_id": null,
                "country": {
                    "id": 724,
                    "iso_3166_2": "ES",
                    "iso_3166_3": "ESP",
                    "name": "Spain",
                    "swap_postal_code": true,
                    "swap_currency_symbol": true,
                    "thousand_separator": null,
                    "decimal_separator": null
                }
            },
            "primary_regno_id": null,
            "primary_regno": null,
            "secondary_regno_id": null,
            "secondary_regno": null,
            "price_client": 0,
            "price_driver": 0,
            "routeA": {
                "id": 42,
                "travel": {
                    "id": 28,
                    "customer_id": 5,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-12 00:00:00",
                    "date_end": "2019-12-28 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-12 11:29:08",
                    "updated_at": "2019-12-12 12:02:49",
                    "deleted_at": null
                },
                "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                "order": 0,
                "load": 1,
                "address": {
                    "id": 1,
                    "name": "Catedral de Barcelona",
                    "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                    "city": "Barcelona",
                    "country_id": 724,
                    "country": {
                        "id": 724,
                        "iso_3166_2": "ES",
                        "iso_3166_3": "ESP",
                        "name": "Spain",
                        "swap_postal_code": true,
                        "swap_currency_symbol": true,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "08002",
                    "phone": "+34 632548759",
                    "email": "sfernandez@tralavelbarcelona.com",
                    "contact_name": "Sergio Fernandez",
                    "latitude": 41.383962,
                    "longitude": 2.1761990999999625
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "routeB": {
                "id": 43,
                "travel": {
                    "id": 28,
                    "customer_id": 5,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-12 00:00:00",
                    "date_end": "2019-12-28 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-12 11:29:08",
                    "updated_at": "2019-12-12 12:02:49",
                    "deleted_at": null
                },
                "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                "order": 1,
                "load": 0,
                "address": {
                    "id": 2,
                    "name": "Oslo City",
                    "address": "Stenersgata 1, 0050 Oslo, Noruega",
                    "city": "Oslo",
                    "country_id": 578,
                    "country": {
                        "id": 578,
                        "iso_3166_2": "NO",
                        "iso_3166_3": "NOR",
                        "name": "Norway",
                        "swap_postal_code": false,
                        "swap_currency_symbol": false,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "0050",
                    "phone": "+4 7625348579",
                    "email": "modegaard@tralaveloslo.com",
                    "contact_name": "Martin Odegaard",
                    "latitude": 59.9126918,
                    "longitude": 10.752917000000025
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "offered": false,
            "accepted": false,
            "status_id": 1,
            "status": {
                "id": 1,
                "name": "Draft",
                "color": "#a9aaba",
                "description": null,
                "deleted_at": null,
                "created_at": "2019-11-19 10:52:44",
                "updated_at": "2019-12-09 12:27:42",
                "priority": 2
            },
            "priority": 2,
            "phases": [
                {
                    "id": 42,
                    "travel": {
                        "id": 28,
                        "customer_id": 5,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-12 00:00:00",
                        "date_end": "2019-12-28 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-12 11:29:08",
                        "updated_at": "2019-12-12 12:02:49",
                        "deleted_at": null
                    },
                    "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                    "order": 0,
                    "load": 1,
                    "address": {
                        "id": 1,
                        "name": "Catedral de Barcelona",
                        "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                        "city": "Barcelona",
                        "country_id": 724,
                        "country": {
                            "id": 724,
                            "iso_3166_2": "ES",
                            "iso_3166_3": "ESP",
                            "name": "Spain",
                            "swap_postal_code": true,
                            "swap_currency_symbol": true,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "08002",
                        "phone": "+34 632548759",
                        "email": "sfernandez@tralavelbarcelona.com",
                        "contact_name": "Sergio Fernandez",
                        "latitude": 41.383962,
                        "longitude": 2.1761990999999625
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                },
                {
                    "id": 43,
                    "travel": {
                        "id": 28,
                        "customer_id": 5,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-12 00:00:00",
                        "date_end": "2019-12-28 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-12 11:29:08",
                        "updated_at": "2019-12-12 12:02:49",
                        "deleted_at": null
                    },
                    "travel_id": "72d2c650-cd6a-4787-a182-fa7d75f1feab",
                    "order": 1,
                    "load": 0,
                    "address": {
                        "id": 2,
                        "name": "Oslo City",
                        "address": "Stenersgata 1, 0050 Oslo, Noruega",
                        "city": "Oslo",
                        "country_id": 578,
                        "country": {
                            "id": 578,
                            "iso_3166_2": "NO",
                            "iso_3166_3": "NOR",
                            "name": "Norway",
                            "swap_postal_code": false,
                            "swap_currency_symbol": false,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "0050",
                        "phone": "+4 7625348579",
                        "email": "modegaard@tralaveloslo.com",
                        "contact_name": "Martin Odegaard",
                        "latitude": 59.9126918,
                        "longitude": 10.752917000000025
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                }
            ],
            "incidences": [],
            "created_at": "2019-12-12T10:29:08.000000Z",
            "updated_at": "2019-12-12T11:02:49.000000Z",
            "modifiable": true,
            "custom_inputs": [],
            "owner": "3",
            "transferred": false,
            "contract_to": null
        },
        ...
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 0401 | Travel not found |

## Show
> **GET** https://api.hardman.app/api/v2/travels/{id}

List one travel

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |

### Response
~~~json
{
            "id": 21,
            "hardman_identifier": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
            "date_start": "2019-12-02",
            "date_end": "2019-12-24",
            "driver_id": null,
            "driver": null,
            "customer_id": 6,
            "customer": {
                "id": 6,
                "name": "Tralavel Oslo SL",
                "vat_number": "65985645",
                "email": "modegaard@tralaveloslo.com",
                "phone": "+47625348579",
                "contact_name": "Martin Odegaard",
                "address1": "Stenersgata 1, 0050 Oslo, Noruega",
                "address2": null,
                "city": "Barcelona",
                "state": "Oslo kommune",
                "postal_code": "0050",
                "shipping_address1": null,
                "shipping_address2": null,
                "shipping_city": null,
                "shipping_state": null,
                "shipping_postal_code": null,
                "tenant_id": null,
                "country": {
                    "id": 578,
                    "iso_3166_2": "NO",
                    "iso_3166_3": "NOR",
                    "name": "Norway",
                    "swap_postal_code": false,
                    "swap_currency_symbol": false,
                    "thousand_separator": null,
                    "decimal_separator": null
                }
            },
            "primary_regno_id": null,
            "primary_regno": null,
            "secondary_regno_id": null,
            "secondary_regno": null,
            "price_client": 0,
            "price_driver": 0,
            "routeA": {
                "id": 31,
                "travel": {
                    "id": 21,
                    "customer_id": 6,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-02 00:00:00",
                    "date_end": "2019-12-24 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-02 14:40:35",
                    "updated_at": "2019-12-02 14:40:35",
                    "deleted_at": null
                },
                "travel_id": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
                "order": 0,
                "load": 1,
                "address": {
                    "id": 1,
                    "name": "Catedral de Barcelona",
                    "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                    "city": "Barcelona",
                    "country_id": 724,
                    "country": {
                        "id": 724,
                        "iso_3166_2": "ES",
                        "iso_3166_3": "ESP",
                        "name": "Spain",
                        "swap_postal_code": true,
                        "swap_currency_symbol": true,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "08002",
                    "phone": "+34 632548759",
                    "email": "sfernandez@tralavelbarcelona.com",
                    "contact_name": "Sergio Fernandez",
                    "latitude": 41.383962,
                    "longitude": 2.1761990999999625
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "routeB": {
                "id": 31,
                "travel": {
                    "id": 21,
                    "customer_id": 6,
                    "driver_id": null,
                    "primary_regno_id": null,
                    "secondary_regno_id": null,
                    "price_client": 0,
                    "price_driver": 0,
                    "offered": 0,
                    "accepted": 0,
                    "date_start": "2019-12-02 00:00:00",
                    "date_end": "2019-12-24 00:00:00",
                    "status_id": 1,
                    "created_at": "2019-12-02 14:40:35",
                    "updated_at": "2019-12-02 14:40:35",
                    "deleted_at": null
                },
                "travel_id": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
                "order": 0,
                "load": 1,
                "address": {
                    "id": 1,
                    "name": "Catedral de Barcelona",
                    "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                    "city": "Barcelona",
                    "country_id": 724,
                    "country": {
                        "id": 724,
                        "iso_3166_2": "ES",
                        "iso_3166_3": "ESP",
                        "name": "Spain",
                        "swap_postal_code": true,
                        "swap_currency_symbol": true,
                        "thousand_separator": null,
                        "decimal_separator": null
                    },
                    "postal_code": "08002",
                    "phone": "+34 632548759",
                    "email": "sfernandez@tralavelbarcelona.com",
                    "contact_name": "Sergio Fernandez",
                    "latitude": 41.383962,
                    "longitude": 2.1761990999999625
                },
                "intermodal": null,
                "arrived": null,
                "comments": null,
                "goods": null,
                "done": null,
                "custom_inputs": []
            },
            "offered": false,
            "accepted": false,
            "status_id": 1,
            "status": {
                "id": 1,
                "name": "Draft",
                "color": "#a9aaba",
                "description": null,
                "deleted_at": null,
                "created_at": "2019-11-19 10:52:44",
                "updated_at": "2019-12-09 12:27:42",
                "priority": 2
            },
            "priority": 2,
            "phases": [
                {
                    "id": 31,
                    "travel": {
                        "id": 21,
                        "customer_id": 6,
                        "driver_id": null,
                        "primary_regno_id": null,
                        "secondary_regno_id": null,
                        "price_client": 0,
                        "price_driver": 0,
                        "offered": 0,
                        "accepted": 0,
                        "date_start": "2019-12-02 00:00:00",
                        "date_end": "2019-12-24 00:00:00",
                        "status_id": 1,
                        "created_at": "2019-12-02 14:40:35",
                        "updated_at": "2019-12-02 14:40:35",
                        "deleted_at": null
                    },
                    "travel_id": "5fbab8c8-fefd-4bbe-bad0-90a5d0b160e8",
                    "order": 0,
                    "load": 1,
                    "address": {
                        "id": 1,
                        "name": "Catedral de Barcelona",
                        "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                        "city": "Barcelona",
                        "country_id": 724,
                        "country": {
                            "id": 724,
                            "iso_3166_2": "ES",
                            "iso_3166_3": "ESP",
                            "name": "Spain",
                            "swap_postal_code": true,
                            "swap_currency_symbol": true,
                            "thousand_separator": null,
                            "decimal_separator": null
                        },
                        "postal_code": "08002",
                        "phone": "+34 632548759",
                        "email": "sfernandez@tralavelbarcelona.com",
                        "contact_name": "Sergio Fernandez",
                        "latitude": 41.383962,
                        "longitude": 2.1761990999999625
                    },
                    "intermodal": null,
                    "arrived": null,
                    "comments": null,
                    "goods": null,
                    "done": null,
                    "custom_inputs": []
                }
            ],
            "incidences": [],
            "created_at": "2019-12-02T13:40:35.000000Z",
            "updated_at": "2019-12-02T13:40:35.000000Z",
            "modifiable": true,
            "custom_inputs": [],
            "owner": "3",
            "transferred": true,
            "contract_to": {
                "id": 201,
                "to": {
                    "id": 4,
                    "name": "Ikazia Hospital Rotterdam",
                    "address1": "Montessoriweg 1, 3083 AN Rotterdam, Países Bajos",
                    "address2": null,
                    "city": "Rotterdam",
                    "state": "Rotterdam",
                    "postal_code": "3083 AN",
                    "vat_number": "PB-475858585"
                },
                "status": true,
                "created_at": "2019-12-09T07:49:32.000000Z"
            }
        }
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 0501 | Travel not found |

## Create
> **POST** https://api.hardman.app/api/v2/travels

Create travel

### Parameters
| Key                | Description                 | Validation               |
| ------------------ | --------------------------- | ------------------------ |
| customer_id        | Identifier's customer       | Optional, Number         |
| date_start         | Travel end start            | Required, Date           |
| date_end           | Travel end date             | Optional, Date           |
| driver_id          | Identifier's driver         | Optional, Number         |
| price_client       | Travel price client         | Optional, Decimal Number |
| price_driver       | Travel price driver         | Optional, Decimal Number |
| primary_regno_id   | Travel truck registration   | Optional                 |
| secondary_regno_id | Travel trailer registration | Optional                 |
| status_id          | Identifier's status         | Optional, Number         |
| phases             | Travel phases               | Optional, Array          |
| custom_inputs      | Travel custom input         | Optional, Array          |

### Response
~~~json
{
        "id": 29,
        "hardman_identifier": "333c19b9-b48b-40fa-9c2c-3705caaf3019",
        "date_start": "2019-12-13",
        "date_end": "1970-01-01",
        "driver_id": null,
        "driver": null,
        "customer_id": 3,
        "customer": {
            "id": 3,
            "name": "Tralavel SL",
            "vat_number": "12345678",
            "email": "user@company.com",
            "phone": "+34631507852",
            "contact_name": "Contact name",
            "address1": "Carrer major, 0, 43515 La Galera, Tarragona, España",
            "address2": null,
            "city": "La Galera",
            "state": "Tarragona",
            "postal_code": "43515",
            "shipping_address1": null,
            "shipping_address2": null,
            "shipping_city": null,
            "shipping_state": null,
            "shipping_postal_code": null,
            "tenant_id": 3,
            "country": {
                "id": 724,
                "iso_3166_2": "ES",
                "iso_3166_3": "ESP",
                "name": "Spain",
                "swap_postal_code": true,
                "swap_currency_symbol": true,
                "thousand_separator": null,
                "decimal_separator": null
            }
        },
        "primary_regno_id": null,
        "primary_regno": null,
        "secondary_regno_id": null,
        "secondary_regno": null,
        "price_client": null,
        "price_driver": null,
        "routeA": null,
        "routeB": null,
        "offered": false,
        "accepted": false,
        "status_id": 1,
        "status": {
            "id": 1,
            "name": "Draft",
            "color": "#a9aaba",
            "description": "",
            "deleted_at": null,
            "created_at": "2019-11-19 10:52:44",
            "updated_at": "2019-12-09 12:27:42",
            "priority": 2
        },
        "priority": 2,
        "phases": [],
        "incidences": [],
        "created_at": "2019-12-13T10:54:00.000000Z",
        "updated_at": "2019-12-13T10:54:00.000000Z",
        "modifiable": true,
        "custom_inputs": [],
        "owner": "3",
        "transferred": false,
        "contract_to": null
    }
~~~

### Errors
| Code | Message                 |
| ---- | ----------------------- |
| 0601 | Tenant client not found |
| 0602 | Address not found       |
| 0603 | Driver not available    |

## Update
> **POST** https://api.hardman.app/api/v2/travels/{id}

Update travel

### Parameters
| Key                | Description                 | Validation               |
| ------------------ | --------------------------- | ------------------------ |
| customer_id        | Identifier's customer       | Optional, Number         |
| date_start         | Travel end start            | Required, Date           |
| date_end           | Travel end date             | Optional, Date           |
| driver_id          | Identifier's driver         | Optional, Number         |
| price_client       | Travel price client         | Optional, Decimal Number |
| price_driver       | Travel price driver         | Optional, Decimal Number |
| primary_regno_id   | Travel truck registration   | Optional                 |
| secondary_regno_id | Travel trailer registration | Optional                 |
| custom_inputs      | Travel custom input         | Optional, Array          |

### Response
~~~json
{
        "id": 29,
        "hardman_identifier": "333c19b9-b48b-40fa-9c2c-3705caaf3019",
        "date_start": "2019-12-14",
        "date_end": "1970-01-01",
        "driver_id": null,
        "driver": null,
        "customer_id": 3,
        "customer": {
            "id": 3,
            "name": "Tralavel SL",
            "vat_number": "12345678",
            "email": "user@company.com",
            "phone": "+34631507852",
            "contact_name": "Contact name",
            "address1": "Carrer major, 0, 43515 La Galera, Tarragona, España",
            "address2": null,
            "city": "La Galera",
            "state": "Tarragona",
            "postal_code": "43515",
            "shipping_address1": null,
            "shipping_address2": null,
            "shipping_city": null,
            "shipping_state": null,
            "shipping_postal_code": null,
            "tenant_id": 3,
            "country": {
                "id": 724,
                "iso_3166_2": "ES",
                "iso_3166_3": "ESP",
                "name": "Spain",
                "swap_postal_code": true,
                "swap_currency_symbol": true,
                "thousand_separator": null,
                "decimal_separator": null
            }
        },
        "primary_regno_id": null,
        "primary_regno": null,
        "secondary_regno_id": null,
        "secondary_regno": null,
        "price_client": null,
        "price_driver": null,
        "routeA": null,
        "routeB": null,
        "offered": false,
        "accepted": false,
        "status_id": 1,
        "status": {
            "id": 1,
            "name": "Draft",
            "color": "#a9aaba",
            "description": "",
            "deleted_at": null,
            "created_at": "2019-11-19 10:52:44",
            "updated_at": "2019-12-09 12:27:42",
            "priority": 2
        },
        "priority": 2,
        "phases": [],
        "incidences": [],
        "created_at": "2019-12-13T10:54:00.000000Z",
        "updated_at": "2019-12-13T10:54:00.000000Z",
        "modifiable": true,
        "custom_inputs": [],
        "owner": "3",
        "transferred": false,
        "contract_to": null
    }
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 0701 | Travel not found |
| 0702 | Invalid input id |

## Delete
> **POST** https://api.hardman.app/api/v2/travels/{id}

Delete travel

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
    "data": true
}
~~~

### Errors
| Code | Message                          |
| ---- | -------------------------------- |
| 0801 | Travel not found                 |
| 0802 | Cannot delete transferred travel |

## Status
> **PUT** https://api.hardman.app/api/v2/travels/status/{id}/{status}

Update travel status

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
    "data": true
}
~~~

### Errors
| Code | Message                                                |
| ---- | ------------------------------------------------------ |
| 0901 | Travel not found                                       |
| 0902 | You cannot modify the status travel                    |
| 0903 | Travel cannot be sent due to no driver assigned        |
| 0904 | Travel cannot be sent because driver is not available  |
| 0905 | Travel cannot be sent due to no truck assigned         |
| 0906 | Travel cannot be sent because truck is not available   |
| 0907 | Travel cannot be sent due to no trailer assigned       |
| 0908 | Travel cannot be sent because trailer is not available |

# Addresses
## List
> **GET** https://api.hardman.app/api/v2/addresses

List all addresses

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 1,
            "name": "Catedral de Barcelona",
            "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
            "city": "Barcelona",
            "country_id": 724,
            "country": {
                "id": 724,
                "iso_3166_2": "ES",
                "iso_3166_3": "ESP",
                "name": "Spain",
                "swap_postal_code": true,
                "swap_currency_symbol": true,
                "thousand_separator": null,
                "decimal_separator": null
            },
            "postal_code": "08002",
            "phone": "+34 632548759",
            "email": "sfernandez@tralavelbarcelona.com",
            "contact_name": "Sergio Fernandez",
            "latitude": 41.383962,
            "longitude": 2.1761990999999625
},
...
~~~

### Errors
| Code | Message |
| ---- | ------- |


## Show
> **GET** https://api.hardman.app/api/v2/addresses/{id}

List one address

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 1,
            "name": "Catedral de Barcelona",
            "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
            "city": "Barcelona",
            "country_id": 724,
            "country": {
                "id": 724,
                "iso_3166_2": "ES",
                "iso_3166_3": "ESP",
                "name": "Spain",
                "swap_postal_code": true,
                "swap_currency_symbol": true,
                "thousand_separator": null,
                "decimal_separator": null
            },
            "postal_code": "08002",
            "phone": "+34 632548759",
            "email": "sfernandez@tralavelbarcelona.com",
            "contact_name": "Sergio Fernandez",
            "latitude": 41.383962,
            "longitude": 2.1761990999999625
}
~~~

### Errors
| Code | Message |
| ---- | ------- |
| 1401 | Address not found |

## Create
> **POST** https://api.hardman.app/api/v2/addresses

Create address

### Parameters
| Key          | Description          | Validation |
| ------------ | -------------------- | ---------- |
| name         | Company name         | Required   |
| city         | City name            | Required   |
| address      | Company address      | Required   |
| postal_code  | Postal code          | Required   |
| country_id   | Identifier's country | Required   |
| coordinates  | Address cordinates   | Optional   |
| email        | Contact email        | Optional   |
| phone        | Phone number         | Optional   |
| contact_name | Contact name         | Optional   |

### Response
~~~json
{
        "id": 34,
        "name": "Tralavel SL",
        "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
        "city": "Barcelona",
        "country_id": "724",
        "country": {
            "id": 724,
            "iso_3166_2": "ES",
            "iso_3166_3": "ESP",
            "name": "Spain",
            "swap_postal_code": true,
            "swap_currency_symbol": true,
            "thousand_separator": null,
            "decimal_separator": null
        },
        "postal_code": "08002",
        "phone": null,
        "email": null,
        "contact_name": null,
        "latitude": null,
        "longitude": null
}
~~~

### Errors
| Code | Message |
| ---- | ------- |

## Update
> **PUT** https://api.hardman.app/api/v2/addresses/{id} 
 
Update address
 
### Parameters 
| Key          | Description          | Validation |
| ------------ | -------------------- | ---------- |
| name         | Company name         | Required   |
| city         | City name            | Required   |
| address      | Company address      | Required   |
| postal_code  | Postal code          | Required   |
| country_id   | Identifier's country | Required   |
| coordinates  | Address cordinates   | Optional   |
| email        | Contact email        | Optional   |
| phone        | Phone number         | Optional   |
| contact_name | Contact name         | Optional   |
 
### Response 
~~~json 
{ 
        "id": 34,
        "name": "Tralavel SA",
        "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
        "city": "Barcelona",
        "country_id": "724",
        "country": {
            "id": 724,
            "iso_3166_2": "ES",
            "iso_3166_3": "ESP",
            "name": "Spain",
            "swap_postal_code": true,
            "swap_currency_symbol": true,
            "thousand_separator": null,
            "decimal_separator": null
        },
        "postal_code": "08002",
        "phone": null,
        "email": null,
        "contact_name": null,
        "latitude": null,
        "longitude": null
}
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |
| 1601 | Address not found |

## Delete
> **GET** https://api.hardman.app/api/v2/addresses

Delete address

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
    "data": true
}
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |
| 1701 | Address not found |

## Countries
> **GET** https://api.hardman.app/api/v2/countries

List all countries

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 4,
            "iso_3166_2": "AF",
            "iso_3166_3": "AFG",
            "name": "Afghanistan",
            "swap_postal_code": false,
            "swap_currency_symbol": false,
            "thousand_separator": null,
            "decimal_separator": null
},
...
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |
| 1701 | Address not found |

# Client
## List
> **GET** https://api.hardman.app/api/v2/clients

List all clients

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 5,
            "name": "Tralavel Barcelona SL",
            "vat_number": "15689574",
            "email": null,
            "phone": null,
            "contact_name": null,
            "address1": "Pla de la Seu, s/n, 08002 Barcelona, España",
            "address2": null,
            "city": "Barcelona",
            "state": "Barcelona",
            "postal_code": "08002",
            "shipping_address1": null,
            "shipping_address2": null,
            "shipping_city": null,
            "shipping_state": null,
            "shipping_postal_code": null,
            "tenant_id": null,
            "country": {
                "id": 724,
                "iso_3166_2": "ES",
                "iso_3166_3": "ESP",
                "name": "Spain",
                "swap_postal_code": true,
                "swap_currency_symbol": true,
                "thousand_separator": null,
                "decimal_separator": null
            }
},
...
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |

## Show
> **GET** https://api.hardman.app/api/v2/clients/{id}

List one client

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 5,
            "name": "Tralavel Barcelona SL",
            "vat_number": "15689574",
            "email": null,
            "phone": null,
            "contact_name": null,
            "address1": "Pla de la Seu, s/n, 08002 Barcelona, España",
            "address2": null,
            "city": "Barcelona",
            "state": "Barcelona",
            "postal_code": "08002",
            "shipping_address1": null,
            "shipping_address2": null,
            "shipping_city": null,
            "shipping_state": null,
            "shipping_postal_code": null,
            "tenant_id": null,
            "country": {
                "id": 724,
                "iso_3166_2": "ES",
                "iso_3166_3": "ESP",
                "name": "Spain",
                "swap_postal_code": true,
                "swap_currency_symbol": true,
                "thousand_separator": null,
                "decimal_separator": null
            }
}
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 2001 | Client not found |

## Create
> **POST** https://api.hardman.app/api/v2/countries

Create client

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |
| name                   | Company name           | Required, Text   |
| vat_number             | Vat number             | Required         |
| contact_name           | Contact name           | Required, Text   |
| email                  | Contact email          | Required         |
| phone                  | Contact phone          | Required, Text   |
| work_phone             | Contact work phone     | Optional, Text   |
| address1               | City name              | Optional         |
| address2               | Company address        | Optional         |
| city                   | City name              | Optional         |
| state                  | Client state           | Optional         |
| country_id             | Identifiers's country  | Optional         |
| postal_code            | Postal code            | Optional         |
| payment_terms          | Payment terms          | Optional         |
| invoice_number_counter | Invoice number counter | Optional, Number |
| quote_number_counter   | Quote number counter   | Optional, Number |
| shipping_address1      | Shipping address       | Optional         |
| shipping_address2      | Shipping address       | Optional         |
| shipping_city          | Shipping city          | Optional         |
| shipping_state         | Shipping state         | Optional         |
| shipping_postal_code   | Shipping postal code   | Optional         |

### Response
~~~json
{
        "id": 22,
        "name": "Tralavel SL",
        "vat_number": "12345679",
        "email": "jbrossa@tralavel.com",
        "phone": "698578547",
        "contact_name": "Jordi Brossa",
        "address1": null,
        "address2": null,
        "city": null,
        "state": null,
        "postal_code": null,
        "shipping_address1": null,
        "shipping_address2": null,
        "shipping_city": null,
        "shipping_state": null,
        "shipping_postal_code": null,
        "tenant_id": null,
        "country": null
}
~~~

### Errors
| Code | Message |
| ---- | ------- |

## Update
> **PUT** https://api.hardman.app/api/v2/countries/{id}

Update client

### Parameters
| Key                    | Description            | Validation       |
| ---------------------- | ---------------------- | ---------------- |
| name                   | Company name           | Required, Text   |
| vat_number             | Vat number             | Required         |
| contact_name           | Contact name           | Required, Text   |
| email                  | Contact email          | Required         |
| phone                  | Contact phone          | Required, Text   |
| work_phone             | Contact work phone     | Optional, Text   |
| address1               | City name              | Optional         |
| address2               | Company address        | Optional         |
| city                   | City name              | Optional         |
| state                  | Client state           | Optional         |
| country_id             | Identifiers's country  | Optional         |
| postal_code            | Postal code            | Optional         |
| payment_terms          | Payment terms          | Optional         |
| invoice_number_counter | Invoice number counter | Optional, Number |
| quote_number_counter   | Quote number counter   | Optional, Number |
| shipping_address1      | Shipping address       | Optional         |
| shipping_address2      | Shipping address       | Optional         |
| shipping_city          | Shipping city          | Optional         |
| shipping_state         | Shipping state         | Optional         |
| shipping_postal_code   | Shipping postal code   | Optional         |

### Response
~~~json
{
        "id": 22,
        "name": "Tralavel SL",
        "vat_number": "12345679",
        "email": "cgomez@tralavel.com",
        "phone": "698578547",
        "contact_name": "Carlos Gómez",
        "address1": null,
        "address2": null,
        "city": null,
        "state": null,
        "postal_code": null,
        "shipping_address1": null,
        "shipping_address2": null,
        "shipping_city": null,
        "shipping_state": null,
        "shipping_postal_code": null,
        "tenant_id": null,
        "country": null
}
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 2201 | Client not found |

## Delete
> **DELETE** https://api.hardman.app/api/v2/countries/{id}

Delete client

### Parameters
| Key                    | Description            | Validation       |
| ---------------------- | ---------------------- | ---------------- |


### Response
~~~json
{
    "data": 1
}
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 2301 | Client not found |

# PrimaryRegno
## ListTravel
> **DELETE** https://api.hardman.app/api/v2/primaryregnos

List Travel

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
    "data": 1
}
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 2301 | Client not found |

## List
> **GET** https://api.hardman.app/api/v2/primaryregnos

List primary regnos

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 9,
            "regno": "6589 KLH",
            "user": null,
            "tenant": {
                "id": 3,
                "name": "Tralavel SL",
                "token_intermodal": null,
                "timezone_id": null,
                "date_format_id": null,
                "datetime_format_id": null,
                "currency_id": 3,
                "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
                "last_login": null,
                "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
                "address2": null,
                "city": "La Galera",
                "state": "Tarragona",
                "postal_code": "43515",
                "country_id": 724,
                "invoice_terms": null,
                "email_footer": null,
                "industry_id": null,
                "size_id": null,
                "invoice_taxes": 1,
                "invoice_item_taxes": 0,
                "invoice_design_id": 11,
                "work_phone": null,
                "work_email": null,
                "language_id": 12,
                "custom_value1": null,
                "custom_value2": null,
                "fill_products": 1,
                "update_products": 1,
                "primary_color": null,
                "secondary_color": null,
                "hide_quantity": 0,
                "hide_paid_to_date": 0,
                "custom_invoice_taxes1": null,
                "custom_invoice_taxes2": null,
                "vat_number": "12345678",
                "invoice_number_prefix": null,
                "invoice_number_counter": 1,
                "quote_number_prefix": null,
                "quote_number_counter": 1,
                "share_counter": 1,
                "id_number": null,
                "token_billing_type_id": 4,
                "invoice_footer": null,
                "pdf_email_attachment": 0,
                "subdomain": null,
                "font_size": 9,
                "invoice_labels": null,
                "custom_design1": null,
                "show_item_taxes": 0,
                "iframe_url": null,
                "military_time": 0,
                "enable_reminder1": 0,
                "enable_reminder2": 0,
                "enable_reminder3": 0,
                "num_days_reminder1": 7,
                "num_days_reminder2": 14,
                "num_days_reminder3": 30,
                "recurring_hour": 8,
                "invoice_number_pattern": null,
                "quote_number_pattern": null,
                "quote_terms": null,
                "email_design_id": 1,
                "enable_email_markup": 0,
                "website": null,
                "direction_reminder1": 1,
                "direction_reminder2": 1,
                "direction_reminder3": 1,
                "field_reminder1": 1,
                "field_reminder2": 1,
                "field_reminder3": 1,
                "client_view_css": null,
                "header_font_id": 1,
                "body_font_id": 1,
                "auto_convert_quote": 1,
                "all_pages_footer": 1,
                "all_pages_header": 1,
                "show_currency_code": 1,
                "enable_portal_password": 0,
                "send_portal_password": 0,
                "recurring_invoice_number_prefix": "R",
                "enable_client_portal": 1,
                "invoice_fields": null,
                "devices": null,
                "logo": null,
                "logo_width": 1062,
                "logo_height": 263,
                "logo_size": 15153,
                "invoice_embed_documents": 0,
                "document_email_attachment": 0,
                "enable_client_portal_dashboard": 1,
                "company_id": 3,
                "page_size": "A4",
                "live_preview": 1,
                "invoice_number_padding": 4,
                "enable_second_tax_rate": 0,
                "auto_bill_on_due_date": 0,
                "start_of_week": 1,
                "enable_buy_now_buttons": 0,
                "include_item_taxes_inline": 0,
                "financial_year_start": null,
                "enabled_modules": 63,
                "enabled_dashboard_sections": 7,
                "show_accept_invoice_terms": 0,
                "show_accept_quote_terms": 0,
                "require_invoice_signature": 0,
                "require_quote_signature": 0,
                "client_number_prefix": null,
                "client_number_counter": 0,
                "client_number_pattern": null,
                "domain_id": 1,
                "payment_terms": null,
                "reset_counter_frequency_id": null,
                "payment_type_id": null,
                "gateway_fee_enabled": 0,
                "reset_counter_date": null,
                "tax_name1": null,
                "tax_rate1": "0.000",
                "tax_name2": null,
                "tax_rate2": "0.000",
                "quote_design_id": 1,
                "custom_design2": null,
                "custom_design3": null,
                "analytics_key": null,
                "credit_number_counter": 0,
                "credit_number_prefix": null,
                "credit_number_pattern": null,
                "task_rate": "0.0000",
                "inclusive_taxes": 0,
                "convert_products": 0,
                "enable_reminder4": 0,
                "signature_on_pdf": 0,
                "ubl_email_attachment": 0,
                "auto_archive_invoice": 0,
                "auto_archive_quote": 0,
                "auto_email_invoice": 1,
                "send_item_details": 0,
                "custom_fields": [],
                "background_image_id": null,
                "custom_messages": [],
                "is_custom_domain": 0,
                "show_product_notes": 0,
                "created_at": "2019-11-19 11:29:52",
                "updated_at": "2019-11-19 11:29:52",
                "deleted_at": null,
                "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
                "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
            },
            "current_user": null,
            "created_at": "2019-11-25T07:32:17.000000Z",
            "updated_at": "2019-12-09T08:35:35.000000Z"
},
...
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |

## ListTravel
> **GET** https://api.hardman.app/api/v2/primaryregnos/{id}

List one primary regno

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 9,
            "regno": "6589 KLH",
            "user": null,
            "tenant": {
                "id": 3,
                "name": "Tralavel SL",
                "token_intermodal": null,
                "timezone_id": null,
                "date_format_id": null,
                "datetime_format_id": null,
                "currency_id": 3,
                "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
                "last_login": null,
                "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
                "address2": null,
                "city": "La Galera",
                "state": "Tarragona",
                "postal_code": "43515",
                "country_id": 724,
                "invoice_terms": null,
                "email_footer": null,
                "industry_id": null,
                "size_id": null,
                "invoice_taxes": 1,
                "invoice_item_taxes": 0,
                "invoice_design_id": 11,
                "work_phone": null,
                "work_email": null,
                "language_id": 12,
                "custom_value1": null,
                "custom_value2": null,
                "fill_products": 1,
                "update_products": 1,
                "primary_color": null,
                "secondary_color": null,
                "hide_quantity": 0,
                "hide_paid_to_date": 0,
                "custom_invoice_taxes1": null,
                "custom_invoice_taxes2": null,
                "vat_number": "12345678",
                "invoice_number_prefix": null,
                "invoice_number_counter": 1,
                "quote_number_prefix": null,
                "quote_number_counter": 1,
                "share_counter": 1,
                "id_number": null,
                "token_billing_type_id": 4,
                "invoice_footer": null,
                "pdf_email_attachment": 0,
                "subdomain": null,
                "font_size": 9,
                "invoice_labels": null,
                "custom_design1": null,
                "show_item_taxes": 0,
                "iframe_url": null,
                "military_time": 0,
                "enable_reminder1": 0,
                "enable_reminder2": 0,
                "enable_reminder3": 0,
                "num_days_reminder1": 7,
                "num_days_reminder2": 14,
                "num_days_reminder3": 30,
                "recurring_hour": 8,
                "invoice_number_pattern": null,
                "quote_number_pattern": null,
                "quote_terms": null,
                "email_design_id": 1,
                "enable_email_markup": 0,
                "website": null,
                "direction_reminder1": 1,
                "direction_reminder2": 1,
                "direction_reminder3": 1,
                "field_reminder1": 1,
                "field_reminder2": 1,
                "field_reminder3": 1,
                "client_view_css": null,
                "header_font_id": 1,
                "body_font_id": 1,
                "auto_convert_quote": 1,
                "all_pages_footer": 1,
                "all_pages_header": 1,
                "show_currency_code": 1,
                "enable_portal_password": 0,
                "send_portal_password": 0,
                "recurring_invoice_number_prefix": "R",
                "enable_client_portal": 1,
                "invoice_fields": null,
                "devices": null,
                "logo": null,
                "logo_width": 1062,
                "logo_height": 263,
                "logo_size": 15153,
                "invoice_embed_documents": 0,
                "document_email_attachment": 0,
                "enable_client_portal_dashboard": 1,
                "company_id": 3,
                "page_size": "A4",
                "live_preview": 1,
                "invoice_number_padding": 4,
                "enable_second_tax_rate": 0,
                "auto_bill_on_due_date": 0,
                "start_of_week": 1,
                "enable_buy_now_buttons": 0,
                "include_item_taxes_inline": 0,
                "financial_year_start": null,
                "enabled_modules": 63,
                "enabled_dashboard_sections": 7,
                "show_accept_invoice_terms": 0,
                "show_accept_quote_terms": 0,
                "require_invoice_signature": 0,
                "require_quote_signature": 0,
                "client_number_prefix": null,
                "client_number_counter": 0,
                "client_number_pattern": null,
                "domain_id": 1,
                "payment_terms": null,
                "reset_counter_frequency_id": null,
                "payment_type_id": null,
                "gateway_fee_enabled": 0,
                "reset_counter_date": null,
                "tax_name1": null,
                "tax_rate1": "0.000",
                "tax_name2": null,
                "tax_rate2": "0.000",
                "quote_design_id": 1,
                "custom_design2": null,
                "custom_design3": null,
                "analytics_key": null,
                "credit_number_counter": 0,
                "credit_number_prefix": null,
                "credit_number_pattern": null,
                "task_rate": "0.0000",
                "inclusive_taxes": 0,
                "convert_products": 0,
                "enable_reminder4": 0,
                "signature_on_pdf": 0,
                "ubl_email_attachment": 0,
                "auto_archive_invoice": 0,
                "auto_archive_quote": 0,
                "auto_email_invoice": 1,
                "send_item_details": 0,
                "custom_fields": [],
                "background_image_id": null,
                "custom_messages": [],
                "is_custom_domain": 0,
                "show_product_notes": 0,
                "created_at": "2019-11-19 11:29:52",
                "updated_at": "2019-11-19 11:29:52",
                "deleted_at": null,
                "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
                "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
            },
            "current_user": null,
            "created_at": "2019-11-25T07:32:17.000000Z",
            "updated_at": "2019-12-09T08:35:35.000000Z"
}
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 2301 | Client not found |

## Create
> **POST** https://api.hardman.app/api/v2/primaryregnos

Create primary regno

### Parameters
| Key     | Description        | Validation       |
| ------- | ------------------ | ---------------- |
| regno   | Truck registration | Required, Text   |
| user_id | Identifier's user  | Optional, Number |


### Response
~~~json
{
        "id": 15,
        "regno": "1234HHH",
        "user": null,
        "tenant": {
            "id": 3,
            "name": "Tralavel SL",
            "token_intermodal": null,
            "timezone_id": null,
            "date_format_id": null,
            "datetime_format_id": null,
            "currency_id": 3,
            "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
            "last_login": null,
            "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
            "address2": null,
            "city": "La Galera",
            "state": "Tarragona",
            "postal_code": "43515",
            "country_id": 724,
            "invoice_terms": null,
            "email_footer": null,
            "industry_id": null,
            "size_id": null,
            "invoice_taxes": 1,
            "invoice_item_taxes": 0,
            "invoice_design_id": 11,
            "work_phone": null,
            "work_email": null,
            "language_id": 12,
            "custom_value1": null,
            "custom_value2": null,
            "fill_products": 1,
            "update_products": 1,
            "primary_color": null,
            "secondary_color": null,
            "hide_quantity": 0,
            "hide_paid_to_date": 0,
            "custom_invoice_taxes1": null,
            "custom_invoice_taxes2": null,
            "vat_number": "12345678",
            "invoice_number_prefix": null,
            "invoice_number_counter": 1,
            "quote_number_prefix": null,
            "quote_number_counter": 1,
            "share_counter": 1,
            "id_number": null,
            "token_billing_type_id": 4,
            "invoice_footer": null,
            "pdf_email_attachment": 0,
            "subdomain": null,
            "font_size": 9,
            "invoice_labels": null,
            "custom_design1": null,
            "show_item_taxes": 0,
            "iframe_url": null,
            "military_time": 0,
            "enable_reminder1": 0,
            "enable_reminder2": 0,
            "enable_reminder3": 0,
            "num_days_reminder1": 7,
            "num_days_reminder2": 14,
            "num_days_reminder3": 30,
            "recurring_hour": 8,
            "invoice_number_pattern": null,
            "quote_number_pattern": null,
            "quote_terms": null,
            "email_design_id": 1,
            "enable_email_markup": 0,
            "website": null,
            "direction_reminder1": 1,
            "direction_reminder2": 1,
            "direction_reminder3": 1,
            "field_reminder1": 1,
            "field_reminder2": 1,
            "field_reminder3": 1,
            "client_view_css": null,
            "header_font_id": 1,
            "body_font_id": 1,
            "auto_convert_quote": 1,
            "all_pages_footer": 1,
            "all_pages_header": 1,
            "show_currency_code": 1,
            "enable_portal_password": 0,
            "send_portal_password": 0,
            "recurring_invoice_number_prefix": "R",
            "enable_client_portal": 1,
            "invoice_fields": null,
            "devices": null,
            "logo": null,
            "logo_width": 1062,
            "logo_height": 263,
            "logo_size": 15153,
            "invoice_embed_documents": 0,
            "document_email_attachment": 0,
            "enable_client_portal_dashboard": 1,
            "company_id": 3,
            "page_size": "A4",
            "live_preview": 1,
            "invoice_number_padding": 4,
            "enable_second_tax_rate": 0,
            "auto_bill_on_due_date": 0,
            "start_of_week": 1,
            "enable_buy_now_buttons": 0,
            "include_item_taxes_inline": 0,
            "financial_year_start": null,
            "enabled_modules": 63,
            "enabled_dashboard_sections": 7,
            "show_accept_invoice_terms": 0,
            "show_accept_quote_terms": 0,
            "require_invoice_signature": 0,
            "require_quote_signature": 0,
            "client_number_prefix": null,
            "client_number_counter": 0,
            "client_number_pattern": null,
            "domain_id": 1,
            "payment_terms": null,
            "reset_counter_frequency_id": null,
            "payment_type_id": null,
            "gateway_fee_enabled": 0,
            "reset_counter_date": null,
            "tax_name1": null,
            "tax_rate1": "0.000",
            "tax_name2": null,
            "tax_rate2": "0.000",
            "quote_design_id": 1,
            "custom_design2": null,
            "custom_design3": null,
            "analytics_key": null,
            "credit_number_counter": 0,
            "credit_number_prefix": null,
            "credit_number_pattern": null,
            "task_rate": "0.0000",
            "inclusive_taxes": 0,
            "convert_products": 0,
            "enable_reminder4": 0,
            "signature_on_pdf": 0,
            "ubl_email_attachment": 0,
            "auto_archive_invoice": 0,
            "auto_archive_quote": 0,
            "auto_email_invoice": 1,
            "send_item_details": 0,
            "custom_fields": {},
            "background_image_id": null,
            "custom_messages": {},
            "is_custom_domain": 0,
            "show_product_notes": 0,
            "created_at": "2019-11-19 11:29:52",
            "updated_at": "2019-11-19 11:29:52",
            "deleted_at": null,
            "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
            "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
        },
        "current_user": null,
        "created_at": "2019-12-16T10:01:13.000000Z",
        "updated_at": "2019-12-16T10:01:13.000000Z"
}
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 2301 | Client not found |


## Update
> **PUT** https://api.hardman.app/api/v2/primaryregnos/{id}

Update primary regno

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
        "id": 15,
        "regno": "1234HHH",
        "user": null,
        "tenant": {
            "id": 3,
            "name": "Tralavel SL",
            "token_intermodal": null,
            "timezone_id": null,
            "date_format_id": null,
            "datetime_format_id": null,
            "currency_id": 3,
            "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
            "last_login": null,
            "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
            "address2": null,
            "city": "La Galera",
            "state": "Tarragona",
            "postal_code": "43515",
            "country_id": 724,
            "invoice_terms": null,
            "email_footer": null,
            "industry_id": null,
            "size_id": null,
            "invoice_taxes": 1,
            "invoice_item_taxes": 0,
            "invoice_design_id": 11,
            "work_phone": null,
            "work_email": null,
            "language_id": 12,
            "custom_value1": null,
            "custom_value2": null,
            "fill_products": 1,
            "update_products": 1,
            "primary_color": null,
            "secondary_color": null,
            "hide_quantity": 0,
            "hide_paid_to_date": 0,
            "custom_invoice_taxes1": null,
            "custom_invoice_taxes2": null,
            "vat_number": "12345678",
            "invoice_number_prefix": null,
            "invoice_number_counter": 1,
            "quote_number_prefix": null,
            "quote_number_counter": 1,
            "share_counter": 1,
            "id_number": null,
            "token_billing_type_id": 4,
            "invoice_footer": null,
            "pdf_email_attachment": 0,
            "subdomain": null,
            "font_size": 9,
            "invoice_labels": null,
            "custom_design1": null,
            "show_item_taxes": 0,
            "iframe_url": null,
            "military_time": 0,
            "enable_reminder1": 0,
            "enable_reminder2": 0,
            "enable_reminder3": 0,
            "num_days_reminder1": 7,
            "num_days_reminder2": 14,
            "num_days_reminder3": 30,
            "recurring_hour": 8,
            "invoice_number_pattern": null,
            "quote_number_pattern": null,
            "quote_terms": null,
            "email_design_id": 1,
            "enable_email_markup": 0,
            "website": null,
            "direction_reminder1": 1,
            "direction_reminder2": 1,
            "direction_reminder3": 1,
            "field_reminder1": 1,
            "field_reminder2": 1,
            "field_reminder3": 1,
            "client_view_css": null,
            "header_font_id": 1,
            "body_font_id": 1,
            "auto_convert_quote": 1,
            "all_pages_footer": 1,
            "all_pages_header": 1,
            "show_currency_code": 1,
            "enable_portal_password": 0,
            "send_portal_password": 0,
            "recurring_invoice_number_prefix": "R",
            "enable_client_portal": 1,
            "invoice_fields": null,
            "devices": null,
            "logo": null,
            "logo_width": 1062,
            "logo_height": 263,
            "logo_size": 15153,
            "invoice_embed_documents": 0,
            "document_email_attachment": 0,
            "enable_client_portal_dashboard": 1,
            "company_id": 3,
            "page_size": "A4",
            "live_preview": 1,
            "invoice_number_padding": 4,
            "enable_second_tax_rate": 0,
            "auto_bill_on_due_date": 0,
            "start_of_week": 1,
            "enable_buy_now_buttons": 0,
            "include_item_taxes_inline": 0,
            "financial_year_start": null,
            "enabled_modules": 63,
            "enabled_dashboard_sections": 7,
            "show_accept_invoice_terms": 0,
            "show_accept_quote_terms": 0,
            "require_invoice_signature": 0,
            "require_quote_signature": 0,
            "client_number_prefix": null,
            "client_number_counter": 0,
            "client_number_pattern": null,
            "domain_id": 1,
            "payment_terms": null,
            "reset_counter_frequency_id": null,
            "payment_type_id": null,
            "gateway_fee_enabled": 0,
            "reset_counter_date": null,
            "tax_name1": null,
            "tax_rate1": "0.000",
            "tax_name2": null,
            "tax_rate2": "0.000",
            "quote_design_id": 1,
            "custom_design2": null,
            "custom_design3": null,
            "analytics_key": null,
            "credit_number_counter": 0,
            "credit_number_prefix": null,
            "credit_number_pattern": null,
            "task_rate": "0.0000",
            "inclusive_taxes": 0,
            "convert_products": 0,
            "enable_reminder4": 0,
            "signature_on_pdf": 0,
            "ubl_email_attachment": 0,
            "auto_archive_invoice": 0,
            "auto_archive_quote": 0,
            "auto_email_invoice": 1,
            "send_item_details": 0,
            "custom_fields": {},
            "background_image_id": null,
            "custom_messages": {},
            "is_custom_domain": 0,
            "show_product_notes": 0,
            "created_at": "2019-11-19 11:29:52",
            "updated_at": "2019-11-19 11:29:52",
            "deleted_at": null,
            "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
            "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
        },
        "current_user": null,
        "created_at": "2019-12-16T10:01:13.000000Z",
        "updated_at": "2019-12-16T10:01:13.000000Z"
}
~~~

### Errors
| Code | Message         |
| ---- | --------------- |
| 3101 | Truck not found |


## Delete
> **DELETE** https://api.hardman.app/api/v2/primaryregnos/{id}

Delete primary regno

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
        "success": true
}
~~~

### Errors
| Code | Message         |
| ---- | --------------- |
| 3001 | Truck not found |

# SecondaryRegno
## ListTravels
> **DELETE** https://api.hardman.app/api/v2/primaryregnos/{id}

Delete primary regno

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
        "success": true
}
~~~

### Errors
| Code | Message         |
| ---- | --------------- |
| 3001 | Truck not found |

## List
> **GET** https://api.hardman.app/api/v2/secondaryregnos

List all secondary regnos

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 3,
            "regno": "R 1654 HCH",
            "user": null,
            "tenant": {
                "id": 3,
                "name": "Tralavel SL",
                "token_intermodal": null,
                "timezone_id": null,
                "date_format_id": null,
                "datetime_format_id": null,
                "currency_id": 3,
                "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
                "last_login": null,
                "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
                "address2": null,
                "city": "La Galera",
                "state": "Tarragona",
                "postal_code": "43515",
                "country_id": 724,
                "invoice_terms": null,
                "email_footer": null,
                "industry_id": null,
                "size_id": null,
                "invoice_taxes": 1,
                "invoice_item_taxes": 0,
                "invoice_design_id": 11,
                "work_phone": null,
                "work_email": null,
                "language_id": 12,
                "custom_value1": null,
                "custom_value2": null,
                "fill_products": 1,
                "update_products": 1,
                "primary_color": null,
                "secondary_color": null,
                "hide_quantity": 0,
                "hide_paid_to_date": 0,
                "custom_invoice_taxes1": null,
                "custom_invoice_taxes2": null,
                "vat_number": "12345678",
                "invoice_number_prefix": null,
                "invoice_number_counter": 1,
                "quote_number_prefix": null,
                "quote_number_counter": 1,
                "share_counter": 1,
                "id_number": null,
                "token_billing_type_id": 4,
                "invoice_footer": null,
                "pdf_email_attachment": 0,
                "subdomain": null,
                "font_size": 9,
                "invoice_labels": null,
                "custom_design1": null,
                "show_item_taxes": 0,
                "iframe_url": null,
                "military_time": 0,
                "enable_reminder1": 0,
                "enable_reminder2": 0,
                "enable_reminder3": 0,
                "num_days_reminder1": 7,
                "num_days_reminder2": 14,
                "num_days_reminder3": 30,
                "recurring_hour": 8,
                "invoice_number_pattern": null,
                "quote_number_pattern": null,
                "quote_terms": null,
                "email_design_id": 1,
                "enable_email_markup": 0,
                "website": null,
                "direction_reminder1": 1,
                "direction_reminder2": 1,
                "direction_reminder3": 1,
                "field_reminder1": 1,
                "field_reminder2": 1,
                "field_reminder3": 1,
                "client_view_css": null,
                "header_font_id": 1,
                "body_font_id": 1,
                "auto_convert_quote": 1,
                "all_pages_footer": 1,
                "all_pages_header": 1,
                "show_currency_code": 1,
                "enable_portal_password": 0,
                "send_portal_password": 0,
                "recurring_invoice_number_prefix": "R",
                "enable_client_portal": 1,
                "invoice_fields": null,
                "devices": null,
                "logo": null,
                "logo_width": 1062,
                "logo_height": 263,
                "logo_size": 15153,
                "invoice_embed_documents": 0,
                "document_email_attachment": 0,
                "enable_client_portal_dashboard": 1,
                "company_id": 3,
                "page_size": "A4",
                "live_preview": 1,
                "invoice_number_padding": 4,
                "enable_second_tax_rate": 0,
                "auto_bill_on_due_date": 0,
                "start_of_week": 1,
                "enable_buy_now_buttons": 0,
                "include_item_taxes_inline": 0,
                "financial_year_start": null,
                "enabled_modules": 63,
                "enabled_dashboard_sections": 7,
                "show_accept_invoice_terms": 0,
                "show_accept_quote_terms": 0,
                "require_invoice_signature": 0,
                "require_quote_signature": 0,
                "client_number_prefix": null,
                "client_number_counter": 0,
                "client_number_pattern": null,
                "domain_id": 1,
                "payment_terms": null,
                "reset_counter_frequency_id": null,
                "payment_type_id": null,
                "gateway_fee_enabled": 0,
                "reset_counter_date": null,
                "tax_name1": null,
                "tax_rate1": "0.000",
                "tax_name2": null,
                "tax_rate2": "0.000",
                "quote_design_id": 1,
                "custom_design2": null,
                "custom_design3": null,
                "analytics_key": null,
                "credit_number_counter": 0,
                "credit_number_prefix": null,
                "credit_number_pattern": null,
                "task_rate": "0.0000",
                "inclusive_taxes": 0,
                "convert_products": 0,
                "enable_reminder4": 0,
                "signature_on_pdf": 0,
                "ubl_email_attachment": 0,
                "auto_archive_invoice": 0,
                "auto_archive_quote": 0,
                "auto_email_invoice": 1,
                "send_item_details": 0,
                "custom_fields": [],
                "background_image_id": null,
                "custom_messages": [],
                "is_custom_domain": 0,
                "show_product_notes": 0,
                "created_at": "2019-11-19 11:29:52",
                "updated_at": "2019-11-19 11:29:52",
                "deleted_at": null,
                "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
                "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
            },
            "current_user": null,
            "created_at": "2019-11-19T11:03:58.000000Z",
            "updated_at": "2019-12-09T08:35:35.000000Z"
},
...
~~~

### Errors
| Code | Message         |
| ---- | --------------- |
| 3001 | Truck not found |

## Show
> **GET** https://api.hardman.app/api/v2/secondaryregnos/{id}

List one secondary regno

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 3,
            "regno": "R 1654 HCH",
            "user": null,
            "tenant": {
                "id": 3,
                "name": "Tralavel SL",
                "token_intermodal": null,
                "timezone_id": null,
                "date_format_id": null,
                "datetime_format_id": null,
                "currency_id": 3,
                "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
                "last_login": null,
                "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
                "address2": null,
                "city": "La Galera",
                "state": "Tarragona",
                "postal_code": "43515",
                "country_id": 724,
                "invoice_terms": null,
                "email_footer": null,
                "industry_id": null,
                "size_id": null,
                "invoice_taxes": 1,
                "invoice_item_taxes": 0,
                "invoice_design_id": 11,
                "work_phone": null,
                "work_email": null,
                "language_id": 12,
                "custom_value1": null,
                "custom_value2": null,
                "fill_products": 1,
                "update_products": 1,
                "primary_color": null,
                "secondary_color": null,
                "hide_quantity": 0,
                "hide_paid_to_date": 0,
                "custom_invoice_taxes1": null,
                "custom_invoice_taxes2": null,
                "vat_number": "12345678",
                "invoice_number_prefix": null,
                "invoice_number_counter": 1,
                "quote_number_prefix": null,
                "quote_number_counter": 1,
                "share_counter": 1,
                "id_number": null,
                "token_billing_type_id": 4,
                "invoice_footer": null,
                "pdf_email_attachment": 0,
                "subdomain": null,
                "font_size": 9,
                "invoice_labels": null,
                "custom_design1": null,
                "show_item_taxes": 0,
                "iframe_url": null,
                "military_time": 0,
                "enable_reminder1": 0,
                "enable_reminder2": 0,
                "enable_reminder3": 0,
                "num_days_reminder1": 7,
                "num_days_reminder2": 14,
                "num_days_reminder3": 30,
                "recurring_hour": 8,
                "invoice_number_pattern": null,
                "quote_number_pattern": null,
                "quote_terms": null,
                "email_design_id": 1,
                "enable_email_markup": 0,
                "website": null,
                "direction_reminder1": 1,
                "direction_reminder2": 1,
                "direction_reminder3": 1,
                "field_reminder1": 1,
                "field_reminder2": 1,
                "field_reminder3": 1,
                "client_view_css": null,
                "header_font_id": 1,
                "body_font_id": 1,
                "auto_convert_quote": 1,
                "all_pages_footer": 1,
                "all_pages_header": 1,
                "show_currency_code": 1,
                "enable_portal_password": 0,
                "send_portal_password": 0,
                "recurring_invoice_number_prefix": "R",
                "enable_client_portal": 1,
                "invoice_fields": null,
                "devices": null,
                "logo": null,
                "logo_width": 1062,
                "logo_height": 263,
                "logo_size": 15153,
                "invoice_embed_documents": 0,
                "document_email_attachment": 0,
                "enable_client_portal_dashboard": 1,
                "company_id": 3,
                "page_size": "A4",
                "live_preview": 1,
                "invoice_number_padding": 4,
                "enable_second_tax_rate": 0,
                "auto_bill_on_due_date": 0,
                "start_of_week": 1,
                "enable_buy_now_buttons": 0,
                "include_item_taxes_inline": 0,
                "financial_year_start": null,
                "enabled_modules": 63,
                "enabled_dashboard_sections": 7,
                "show_accept_invoice_terms": 0,
                "show_accept_quote_terms": 0,
                "require_invoice_signature": 0,
                "require_quote_signature": 0,
                "client_number_prefix": null,
                "client_number_counter": 0,
                "client_number_pattern": null,
                "domain_id": 1,
                "payment_terms": null,
                "reset_counter_frequency_id": null,
                "payment_type_id": null,
                "gateway_fee_enabled": 0,
                "reset_counter_date": null,
                "tax_name1": null,
                "tax_rate1": "0.000",
                "tax_name2": null,
                "tax_rate2": "0.000",
                "quote_design_id": 1,
                "custom_design2": null,
                "custom_design3": null,
                "analytics_key": null,
                "credit_number_counter": 0,
                "credit_number_prefix": null,
                "credit_number_pattern": null,
                "task_rate": "0.0000",
                "inclusive_taxes": 0,
                "convert_products": 0,
                "enable_reminder4": 0,
                "signature_on_pdf": 0,
                "ubl_email_attachment": 0,
                "auto_archive_invoice": 0,
                "auto_archive_quote": 0,
                "auto_email_invoice": 1,
                "send_item_details": 0,
                "custom_fields": [],
                "background_image_id": null,
                "custom_messages": [],
                "is_custom_domain": 0,
                "show_product_notes": 0,
                "created_at": "2019-11-19 11:29:52",
                "updated_at": "2019-11-19 11:29:52",
                "deleted_at": null,
                "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
                "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
            },
            "current_user": null,
            "created_at": "2019-11-19T11:03:58.000000Z",
            "updated_at": "2019-12-09T08:35:35.000000Z"
}
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |
| 3601 | Trailer not found |

## Create
> **POST** https://api.hardman.app/api/v2/secondaryregnos

Create secondary regno

### Parameters
| Key     | Description          | Validation       |
| ------- | -------------------- | ---------------- |
| regno   | Trailer registration | Required, Text   |
| user_id | Identidfers's user   | Optional, Number |


### Response
~~~json
{
        "id": 16,
        "regno": "R 1234 KLB",
        "user": null,
        "tenant": {
            "id": 3,
            "name": "Tralavel SL",
            "token_intermodal": null,
            "timezone_id": null,
            "date_format_id": null,
            "datetime_format_id": null,
            "currency_id": 3,
            "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
            "last_login": null,
            "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
            "address2": null,
            "city": "La Galera",
            "state": "Tarragona",
            "postal_code": "43515",
            "country_id": 724,
            "invoice_terms": null,
            "email_footer": null,
            "industry_id": null,
            "size_id": null,
            "invoice_taxes": 1,
            "invoice_item_taxes": 0,
            "invoice_design_id": 11,
            "work_phone": null,
            "work_email": null,
            "language_id": 12,
            "custom_value1": null,
            "custom_value2": null,
            "fill_products": 1,
            "update_products": 1,
            "primary_color": null,
            "secondary_color": null,
            "hide_quantity": 0,
            "hide_paid_to_date": 0,
            "custom_invoice_taxes1": null,
            "custom_invoice_taxes2": null,
            "vat_number": "12345678",
            "invoice_number_prefix": null,
            "invoice_number_counter": 1,
            "quote_number_prefix": null,
            "quote_number_counter": 1,
            "share_counter": 1,
            "id_number": null,
            "token_billing_type_id": 4,
            "invoice_footer": null,
            "pdf_email_attachment": 0,
            "subdomain": null,
            "font_size": 9,
            "invoice_labels": null,
            "custom_design1": null,
            "show_item_taxes": 0,
            "iframe_url": null,
            "military_time": 0,
            "enable_reminder1": 0,
            "enable_reminder2": 0,
            "enable_reminder3": 0,
            "num_days_reminder1": 7,
            "num_days_reminder2": 14,
            "num_days_reminder3": 30,
            "recurring_hour": 8,
            "invoice_number_pattern": null,
            "quote_number_pattern": null,
            "quote_terms": null,
            "email_design_id": 1,
            "enable_email_markup": 0,
            "website": null,
            "direction_reminder1": 1,
            "direction_reminder2": 1,
            "direction_reminder3": 1,
            "field_reminder1": 1,
            "field_reminder2": 1,
            "field_reminder3": 1,
            "client_view_css": null,
            "header_font_id": 1,
            "body_font_id": 1,
            "auto_convert_quote": 1,
            "all_pages_footer": 1,
            "all_pages_header": 1,
            "show_currency_code": 1,
            "enable_portal_password": 0,
            "send_portal_password": 0,
            "recurring_invoice_number_prefix": "R",
            "enable_client_portal": 1,
            "invoice_fields": null,
            "devices": null,
            "logo": null,
            "logo_width": 1062,
            "logo_height": 263,
            "logo_size": 15153,
            "invoice_embed_documents": 0,
            "document_email_attachment": 0,
            "enable_client_portal_dashboard": 1,
            "company_id": 3,
            "page_size": "A4",
            "live_preview": 1,
            "invoice_number_padding": 4,
            "enable_second_tax_rate": 0,
            "auto_bill_on_due_date": 0,
            "start_of_week": 1,
            "enable_buy_now_buttons": 0,
            "include_item_taxes_inline": 0,
            "financial_year_start": null,
            "enabled_modules": 63,
            "enabled_dashboard_sections": 7,
            "show_accept_invoice_terms": 0,
            "show_accept_quote_terms": 0,
            "require_invoice_signature": 0,
            "require_quote_signature": 0,
            "client_number_prefix": null,
            "client_number_counter": 0,
            "client_number_pattern": null,
            "domain_id": 1,
            "payment_terms": null,
            "reset_counter_frequency_id": null,
            "payment_type_id": null,
            "gateway_fee_enabled": 0,
            "reset_counter_date": null,
            "tax_name1": null,
            "tax_rate1": "0.000",
            "tax_name2": null,
            "tax_rate2": "0.000",
            "quote_design_id": 1,
            "custom_design2": null,
            "custom_design3": null,
            "analytics_key": null,
            "credit_number_counter": 0,
            "credit_number_prefix": null,
            "credit_number_pattern": null,
            "task_rate": "0.0000",
            "inclusive_taxes": 0,
            "convert_products": 0,
            "enable_reminder4": 0,
            "signature_on_pdf": 0,
            "ubl_email_attachment": 0,
            "auto_archive_invoice": 0,
            "auto_archive_quote": 0,
            "auto_email_invoice": 1,
            "send_item_details": 0,
            "custom_fields": {},
            "background_image_id": null,
            "custom_messages": {},
            "is_custom_domain": 0,
            "show_product_notes": 0,
            "created_at": "2019-11-19 11:29:52",
            "updated_at": "2019-11-19 11:29:52",
            "deleted_at": null,
            "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
            "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
}
~~~

### Errors
| Code | Message |
| ---- | ------- |

## Create
> **PUT** https://api.hardman.app/api/v2/secondaryregnos/{id}

Update secondary regno

### Parameters
| Key   | Description          | Validation     |
| ----- | -------------------- | -------------- |
| regno | Trailer registration | Required, Text |


### Response
~~~json
{
        "id": 16,
        "regno": "R 4321 OPO",
        "user": null,
        "tenant": {
            "id": 3,
            "name": "Tralavel SL",
            "token_intermodal": null,
            "timezone_id": null,
            "date_format_id": null,
            "datetime_format_id": null,
            "currency_id": 3,
            "account_key": "Vn2GI0Ff4cXI6cRiRkfbhzVAPltcgud7",
            "last_login": null,
            "address1": "Carrer de Tarragona, 10, 43515 La Galera, Tarragona, España",
            "address2": null,
            "city": "La Galera",
            "state": "Tarragona",
            "postal_code": "43515",
            "country_id": 724,
            "invoice_terms": null,
            "email_footer": null,
            "industry_id": null,
            "size_id": null,
            "invoice_taxes": 1,
            "invoice_item_taxes": 0,
            "invoice_design_id": 11,
            "work_phone": null,
            "work_email": null,
            "language_id": 12,
            "custom_value1": null,
            "custom_value2": null,
            "fill_products": 1,
            "update_products": 1,
            "primary_color": null,
            "secondary_color": null,
            "hide_quantity": 0,
            "hide_paid_to_date": 0,
            "custom_invoice_taxes1": null,
            "custom_invoice_taxes2": null,
            "vat_number": "12345678",
            "invoice_number_prefix": null,
            "invoice_number_counter": 1,
            "quote_number_prefix": null,
            "quote_number_counter": 1,
            "share_counter": 1,
            "id_number": null,
            "token_billing_type_id": 4,
            "invoice_footer": null,
            "pdf_email_attachment": 0,
            "subdomain": null,
            "font_size": 9,
            "invoice_labels": null,
            "custom_design1": null,
            "show_item_taxes": 0,
            "iframe_url": null,
            "military_time": 0,
            "enable_reminder1": 0,
            "enable_reminder2": 0,
            "enable_reminder3": 0,
            "num_days_reminder1": 7,
            "num_days_reminder2": 14,
            "num_days_reminder3": 30,
            "recurring_hour": 8,
            "invoice_number_pattern": null,
            "quote_number_pattern": null,
            "quote_terms": null,
            "email_design_id": 1,
            "enable_email_markup": 0,
            "website": null,
            "direction_reminder1": 1,
            "direction_reminder2": 1,
            "direction_reminder3": 1,
            "field_reminder1": 1,
            "field_reminder2": 1,
            "field_reminder3": 1,
            "client_view_css": null,
            "header_font_id": 1,
            "body_font_id": 1,
            "auto_convert_quote": 1,
            "all_pages_footer": 1,
            "all_pages_header": 1,
            "show_currency_code": 1,
            "enable_portal_password": 0,
            "send_portal_password": 0,
            "recurring_invoice_number_prefix": "R",
            "enable_client_portal": 1,
            "invoice_fields": null,
            "devices": null,
            "logo": null,
            "logo_width": 1062,
            "logo_height": 263,
            "logo_size": 15153,
            "invoice_embed_documents": 0,
            "document_email_attachment": 0,
            "enable_client_portal_dashboard": 1,
            "company_id": 3,
            "page_size": "A4",
            "live_preview": 1,
            "invoice_number_padding": 4,
            "enable_second_tax_rate": 0,
            "auto_bill_on_due_date": 0,
            "start_of_week": 1,
            "enable_buy_now_buttons": 0,
            "include_item_taxes_inline": 0,
            "financial_year_start": null,
            "enabled_modules": 63,
            "enabled_dashboard_sections": 7,
            "show_accept_invoice_terms": 0,
            "show_accept_quote_terms": 0,
            "require_invoice_signature": 0,
            "require_quote_signature": 0,
            "client_number_prefix": null,
            "client_number_counter": 0,
            "client_number_pattern": null,
            "domain_id": 1,
            "payment_terms": null,
            "reset_counter_frequency_id": null,
            "payment_type_id": null,
            "gateway_fee_enabled": 0,
            "reset_counter_date": null,
            "tax_name1": null,
            "tax_rate1": "0.000",
            "tax_name2": null,
            "tax_rate2": "0.000",
            "quote_design_id": 1,
            "custom_design2": null,
            "custom_design3": null,
            "analytics_key": null,
            "credit_number_counter": 0,
            "credit_number_prefix": null,
            "credit_number_pattern": null,
            "task_rate": "0.0000",
            "inclusive_taxes": 0,
            "convert_products": 0,
            "enable_reminder4": 0,
            "signature_on_pdf": 0,
            "ubl_email_attachment": 0,
            "auto_archive_invoice": 0,
            "auto_archive_quote": 0,
            "auto_email_invoice": 1,
            "send_item_details": 0,
            "custom_fields": {},
            "background_image_id": null,
            "custom_messages": {},
            "is_custom_domain": 0,
            "show_product_notes": 0,
            "created_at": "2019-11-19 11:29:52",
            "updated_at": "2019-11-19 11:29:52",
            "deleted_at": null,
            "data_username": "eyJpdiI6ImFoVEY3SFlNRVdGSUY5QTBBM09vNUE9PSIsInZhbHVlIjoiQU1NSDRYdldRSHZXYXQwblVPXC9lcEhpdzE1WHJ0d1wvcTBGUEJzeWJ2OUt3PSIsIm1hYyI6ImNlYzhiNGZmMDhkYTBiMTQyOWE5YTdjZjAzZDQ3OTIxZDMwZGU3NDMwNzBmYWQ5NzFjODVmMmZhMzM5ZjU1NGQifQ==",
            "data_password": "eyJpdiI6InB2T1ljSDB0cGRnSjc3UUpZdlFoRVE9PSIsInZhbHVlIjoibUY3UUpMZFp5VUV3Ynl6cFlPbFdtVWlWREJNOEZUSURWZkpHQ2s4MUs3MD0iLCJtYWMiOiI5NjNlZjA5OWY4Y2IyYTEyYjVmMmVmM2ZkYzE2OGM5YzBmNzg3Njg1NTU5MjkyNmJhMTgyOWJlNmE0NjExMjdhIn0="
}
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |
| 3901 | Trailer not found |

## Delete
> **DELETE** https://api.hardman.app/api/v2/secondaryregnos/{id}

Delete secondary regno

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
        "success": true
}
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |
| 3801 | Trailer not found |

# Driver
## List
> **GET** https://api.hardman.app/api/v2/drivers

List all drivers

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 8,
            "api_key": "I4mKxp7DoVv4VaC6KpgI6FfwYgcbik6bSN8nq2YeqKHGwfVoZktVqQH2lYXn",
            "name": "Gerard",
            "surname": "García",
            "phone": "+34659878542",
            "email": "ggarcia@tralavel.com",
            "avatar": null,
            "superadmin": false,
            "device_token": "",
            "internal_id": "1",
            "current_tenant": null,
            "tenant": 3,
            "employer_of": null,
            "app_version": "",
            "platform": "",
            "fullname": "Gerard García",
            "roles": [
                {
                    "id": 1,
                    "name": "Administrador de empresa",
                    "guard_name": "web",
                    "description": "Permiso total sobre cualquier sección del sistema de la empresa",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:08",
                    "updated_at": "2019-11-19 10:52:08",
                    "has_role": false
                },
                {
                    "id": 2,
                    "name": "Gestor de usuarios",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con los usuarios del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:08",
                    "updated_at": "2019-11-19 10:52:08",
                    "has_role": false
                },
                {
                    "id": 3,
                    "name": "Gestor de clientes",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con los clientes del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 4,
                    "name": "Gestor de direcciones",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con las direcciones del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 5,
                    "name": "Gestor de viajes",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con los viajes del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 6,
                    "name": "Gestor de autónomos",
                    "guard_name": "web",
                    "description": "Encargado de buscar y entrar viajes para los autónomos",
                    "visible": 0,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 7,
                    "name": "Gestor de documentación",
                    "guard_name": "web",
                    "description": "Gestiona las documentaciones de los conductores",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 8,
                    "name": "Gestor de matriculas",
                    "guard_name": "web",
                    "description": "Gestiona las matriculas de la empresa",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 9,
                    "name": "Cancelar Intermodal",
                    "guard_name": "web",
                    "description": "Usuario capaz de cancelar un intermodal",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 10,
                    "name": "Modificar Intermodal",
                    "guard_name": "web",
                    "description": "Usuario capaz de modificar un intermodal",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 11,
                    "name": "Conductor",
                    "guard_name": "web",
                    "description": "Usuario de la aplicación móbil para realizar viajes",
                    "visible": 1,
                    "created_at": "2019-11-19 11:27:51",
                    "updated_at": "2019-11-19 11:27:51",
                    "has_role": true
                }
            ],
            "fullsearch":"{\"id\":8,\"name\":\"Gerard\",\"surname\":\"Garc\ía\",\"email\":\"ggarcia@tralavel.com\",\"phone\":\"+34659878542\",\"internal_id\":\"1\",\"api_key\":\"I4mKxp7DoVv4VaC6KpgI6FfwYgcbik6bSN8nq2YeqKHGwfVoZktVqQH2lYXn\",\"urlAvatar\":null,\"device_token\":\"\",\"platform\":\"\",\"app_version\":\"\",\"superadmin\":0,\"current_tenant\":null,\"tenant\":3,\"employer_of\":null,\"accepted_terms_version\":null,\"accepted_terms_timestamp\":null,\"accepted_terms_ip\":null,\"currency_id\":null,\"address1\":null,\"address2\":null,\"city\":null,\"state\":null,\"postal_code\":null,\"country_id\":null,\"created_at\":\"2019-11-19 11:49:39\",\"updated_at\":\"2019-12-09 09:26:30\",\"fullname\":\"Gerard Garc\ía\",\"roles\":[{\"id\":11,\"name\":\"Conductor\",\"guard_name\":\"web\",\"description\":\"Usuario de la aplicaci\ón m\óbil para realizar viajes\",\"visible\":1,\"created_at\":\"2019-11-19 11:27:51\",\"updated_at\":\"2019-11-19 11:27:51\",\"pivot\":{\"model_id\":8,\"role_id\":11,\"model_type\":\"App\\\\User\"}}]}",
            "tags": [],
            "created_at": "2019-11-19T10:49:39.000000Z",
            "available": false
},
...
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |

## Registers
> **GET** https://api.hardman.app/api/v2/analytics/drivers/registers/{year}

Registers driver

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
[
        0,
        0,
        0,
        0,
        0,
        0,
        0,
        0,
        0,
        0,
        3,
        0
]
~~~

### Errors
| Code | Message           |
| ---- | ----------------- |

## Trending
> **GET** https://api.hardman.app/api/v2/analytics/drivers/trending

Trending driver

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
        "user": {
            "id": 8,
            "api_key": "I4mKxp7DoVv4VaC6KpgI6FfwYgcbik6bSN8nq2YeqKHGwfVoZktVqQH2lYXn",
            "name": "Gerard",
            "surname": "García",
            "phone": "+34659878542",
            "email": "ggarcia@tralavel.com",
            "avatar": null,
            "superadmin": false,
            "device_token": "",
            "internal_id": "1",
            "current_tenant": null,
            "tenant": 3,
            "employer_of": null,
            "app_version": "",
            "platform": "",
            "fullname": "Gerard García",
            "roles": [
                {
                    "id": 1,
                    "name": "Administrador de empresa",
                    "guard_name": "web",
                    "description": "Permiso total sobre cualquier sección del sistema de la empresa",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:08",
                    "updated_at": "2019-11-19 10:52:08",
                    "has_role": false
                },
                {
                    "id": 2,
                    "name": "Gestor de usuarios",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con los usuarios del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:08",
                    "updated_at": "2019-11-19 10:52:08",
                    "has_role": false
                },
                {
                    "id": 3,
                    "name": "Gestor de clientes",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con los clientes del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 4,
                    "name": "Gestor de direcciones",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con las direcciones del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 5,
                    "name": "Gestor de viajes",
                    "guard_name": "web",
                    "description": "Encargado de gestionar todo lo relacionado con los viajes del sistema",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 6,
                    "name": "Gestor de autónomos",
                    "guard_name": "web",
                    "description": "Encargado de buscar y entrar viajes para los autónomos",
                    "visible": 0,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 7,
                    "name": "Gestor de documentación",
                    "guard_name": "web",
                    "description": "Gestiona las documentaciones de los conductores",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 8,
                    "name": "Gestor de matriculas",
                    "guard_name": "web",
                    "description": "Gestiona las matriculas de la empresa",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 9,
                    "name": "Cancelar Intermodal",
                    "guard_name": "web",
                    "description": "Usuario capaz de cancelar un intermodal",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 10,
                    "name": "Modificar Intermodal",
                    "guard_name": "web",
                    "description": "Usuario capaz de modificar un intermodal",
                    "visible": 1,
                    "created_at": "2019-11-19 10:52:09",
                    "updated_at": "2019-11-19 10:52:09",
                    "has_role": false
                },
                {
                    "id": 11,
                    "name": "Conductor",
                    "guard_name": "web",
                    "description": "Usuario de la aplicación móbil para realizar viajes",
                    "visible": 1,
                    "created_at": "2019-11-19 11:27:51",
                    "updated_at": "2019-11-19 11:27:51",
                    "has_role": true
                }
            ],
            "fullsearch":"{\"id\":8,\"name\":\"Gerard\",\"surname\":\"Garc\ía\",\"email\":\"ggarcia@tralavel.com\",\"phone\":\"+34659878542\",\"internal_id\":\"1\",\"api_key\":\"I4mKxp7DoVv4VaC6KpgI6FfwYgcbik6bSN8nq2YeqKHGwfVoZktVqQH2lYXn\",\"urlAvatar\":null,\"device_token\":\"\",\"platform\":\"\",\"app_version\":\"\",\"superadmin\":0,\"current_tenant\":null,\"tenant\":3,\"employer_of\":null,\"accepted_terms_version\":null,\"accepted_terms_timestamp\":null,\"accepted_terms_ip\":null,\"currency_id\":null,\"address1\":null,\"address2\":null,\"city\":null,\"state\":null,\"postal_code\":null,\"country_id\":null,\"created_at\":\"2019-11-19 11:49:39\",\"updated_at\":\"2019-12-09 09:26:30\",\"fullname\":\"Gerard Garc\ía\",\"roles\":[{\"id\":11,\"name\":\"Conductor\",\"guard_name\":\"web\",\"description\":\"Usuario de la aplicaci\ón m\óbil para realizar viajes\",\"visible\":1,\"created_at\":\"2019-11-19 11:27:51\",\"updated_at\":\"2019-11-19 11:27:51\",\"pivot\":{\"model_id\":8,\"role_id\":11,\"model_type\":\"App\\\\User\"}}]}",
            "tags": [],
            "created_at": "2019-11-19T10:49:39.000000Z",
            "available": false
        },
        "occurrences": 9
},
...
~~~

### Errors
| Code | Message |
| ---- | ------- |

# Phase
## List
> **GET** https://api.hardman.app/api/v2/phases/{travel_id}

List all phases

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
            "id": 40,
            "travel": {
                "id": 27,
                "customer_id": 5,
                "driver_id": 19,
                "primary_regno_id": null,
                "secondary_regno_id": null,
                "price_client": 0,
                "price_driver": 0,
                "offered": 0,
                "accepted": 0,
                "date_start": "2019-12-09 00:00:00",
                "date_end": "2019-12-13 00:00:00",
                "status_id": 1,
                "created_at": "2019-12-09 08:30:38",
                "updated_at": "2019-12-13 12:51:36",
                "deleted_at": null
            },
            "travel_id": "75d36b0b-54c4-4b61-8886-c648ff86f85a",
            "order": 0,
            "load": 1,
            "address": {
                "id": 1,
                "name": "Catedral de Barcelona",
                "address": "Pla de la Seu, s/n, 08002 Barcelona, España",
                "city": "Barcelona",
                "country_id": 724,
                "country": {
                    "id": 724,
                    "iso_3166_2": "ES",
                    "iso_3166_3": "ESP",
                    "name": "Spain",
                    "swap_postal_code": true,
                    "swap_currency_symbol": true,
                    "thousand_separator": null,
                    "decimal_separator": null
                },
                "postal_code": "08002",
                "phone": "+34 632548759",
                "email": "sfernandez@tralavelbarcelona.com",
                "contact_name": "Sergio Fernandez",
                "latitude": 41.383962,
                "longitude": 2.1761990999999625
            },
            "intermodal": null,
            "arrived": null,
            "comments": null,
            "goods": null,
            "done": null,
            "custom_inputs": []
},
...
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 4001 | Travel not found |

## Create
> **POST** https://api.hardman.app/api/v2/phases

Create phase

### Parameters
| Key           | Description             | Validation                             |
| ------------- | ----------------------- | -------------------------------------- |
| travel_id     | Identifier's travel     | Required                               |
| address_id    | Identifier's address    | Required without:intermodal_id, Number |
| load          | Upload or download      | Optional, Boolean                      |
| goods         | Goods                   | Optional, Text                         |
| comments      | Phase comment           | Optional, Text                         |
| intermodal_id | Identifier's intermodal | Required without:address_id, Number    |
| board         | Board                   | Optional                               |
| custom_inputs | Custom inputs           | Optional, Array                        |
| order         | Phase order             | Optional, Number                       |


### Response
~~~json
{
        "id": 45,
        "travel": {
            "id": 22,
            "customer_id": 5,
            "driver_id": null,
            "primary_regno_id": null,
            "secondary_regno_id": null,
            "price_client": 0,
            "price_driver": 0,
            "offered": 0,
            "accepted": 0,
            "date_start": "2019-12-05 00:00:00",
            "date_end": "2019-12-07 00:00:00",
            "status_id": 1,
            "created_at": "2019-12-05 08:28:40",
            "updated_at": "2019-12-05 08:28:59",
            "deleted_at": null
        },
        "travel_id": "55296b79-8e23-4cbb-83f0-7360a20272f6",
        "order": 3,
        "load": 0,
        "address": {
            "id": 2,
            "name": "Oslo City",
            "address": "Stenersgata 1, 0050 Oslo, Noruega",
            "city": "Oslo",
            "country_id": 578,
            "country": {
                "id": 578,
                "iso_3166_2": "NO",
                "iso_3166_3": "NOR",
                "name": "Norway",
                "swap_postal_code": false,
                "swap_currency_symbol": false,
                "thousand_separator": null,
                "decimal_separator": null
            },
            "postal_code": "0050",
            "phone": "+4 7625348579",
            "email": "modegaard@tralaveloslo.com",
            "contact_name": "Martin Odegaard",
            "latitude": 59.9126918,
            "longitude": 10.752917000000025
        },
        "intermodal": null,
        "arrived": null,
        "comments": null,
        "goods": null,
        "done": null,
        "custom_inputs": []
}
~~~

### Errors
| Code | Message                             |
| ---- | ----------------------------------- |
| 4101 | You're not the owner of this travel |
| 4102 | Travel not found                    |
| 4103 | Intermodal not found                |
| 4104 | Input not found                     |


## Update
> **PUT** https://api.hardman.app/api/v2/phases/{id}

Udate phase

### Parameters
| Key           | Description             | Validation                             |
| ------------- | ----------------------- | -------------------------------------- |
| travel_id     | Identifier's travel     | Required                               |
| address_id    | Identifier's address    | Required without:intermodal_id, Number |
| load          | Upload or download      | Optional, Boolean                      |
| goods         | Goods                   | Optional, Text                         |
| comments      | Phase comment           | Optional, Text                         |
| intermodal_id | Identifier's intermodal | Required without:address_id, Number    |
| board         | Board                   | Optional                               |
| custom_inputs | Custom inputs           | Optional, Array                        |
| order         | Phase order             | Optional, Number                       |


### Response
~~~json
{
        "id": 45,
        "travel": {
            "id": 22,
            "customer_id": 5,
            "driver_id": null,
            "primary_regno_id": null,
            "secondary_regno_id": null,
            "price_client": 0,
            "price_driver": 0,
            "offered": 0,
            "accepted": 0,
            "date_start": "2019-12-05 00:00:00",
            "date_end": "2019-12-07 00:00:00",
            "status_id": 1,
            "created_at": "2019-12-05 08:28:40",
            "updated_at": "2019-12-05 08:28:59",
            "deleted_at": null
        },
        "travel_id": "55296b79-8e23-4cbb-83f0-7360a20272f6",
        "order": 3,
        "load": 0,
        "address": {
            "id": 2,
            "name": "Oslo City",
            "address": "Stenersgata 1, 0050 Oslo, Noruega",
            "city": "Oslo",
            "country_id": 578,
            "country": {
                "id": 578,
                "iso_3166_2": "NO",
                "iso_3166_3": "NOR",
                "name": "Norway",
                "swap_postal_code": false,
                "swap_currency_symbol": false,
                "thousand_separator": null,
                "decimal_separator": null
            },
            "postal_code": "0050",
            "phone": "+4 7625348579",
            "email": "modegaard@tralaveloslo.com",
            "contact_name": "Martin Odegaard",
            "latitude": 59.9126918,
            "longitude": 10.752917000000025
        },
        "intermodal": null,
        "arrived": null,
        "comments": "Update comment",
        "goods": null,
        "done": null,
        "custom_inputs": []
}
~~~

### Errors
| Code | Message                             |
| ---- | ----------------------------------- |
| 4201 | You're not the owner of this travel |
| 4202 | Travel not found                    |
| 4203 | Phase not found                     |
| 4204 | Intermodal not found                |
| 4205 | Input not found                     |

## Delete
> **DELETE** https://api.hardman.app/api/v2/phases/{id}

Delete phase

### Parameters
| Key | Description | Validation |
| --- | ----------- | ---------- |


### Response
~~~json
{
    "data": true
}
~~~

### Errors
| Code | Message          |
| ---- | ---------------- |
| 4301 | Phase not found  |

## Reorder
> **POST** https://api.hardman.app/api/v2/phases/{travel_id}

Reorder phases

### Parameters
| Key    | Description         | Validation      |
| ------ | ------------------- | --------------- |
| phases | Identifier's phases | required, Array |


### Response
~~~json
[
    {
            "id": 32,
            "order": 0,
            "travel_id": 22,
            "goods": null,
            "address_id": 1,
            "load": 1,
            "comments": null,
            "arrived": null,
            "done": null,
            "created_at": "2019-12-05 08:28:50",
            "updated_at": "2019-12-05 08:28:50",
            "deleted_at": null
    },
...
]
~~~

### Errors
| Code | Message                           |
| ---- | --------------------------------- |
| 4401 | Travel not found                  |
| 4402 | Cannot reorder this travel phases |
| 4403 | Phase not found                   |

# Roles
## List
> **GET** https://api.hardman.app/api/v2/phases/roles

List all roles

### Parameters
| Key    | Description         | Validation      |
| ------ | ------------------- | --------------- |


### Response
~~~json
{
            "id": 1,
            "name": "Administrador de empresa",
            "guard_name": "web",
            "description": "Permiso total sobre cualquier sección del sistema de la empresa",
            "visible": 1,
            "created_at": "2019-11-19 10:52:08",
            "updated_at": "2019-11-19 10:52:08",
            "permissions": [
                {
                    "id": 1,
                    "name": "users.index",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:09.000000Z",
                    "updated_at": "2019-11-19T09:52:09.000000Z"
                },
                {
                    "id": 2,
                    "name": "users.update",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:11.000000Z",
                    "updated_at": "2019-11-19T09:52:11.000000Z"
                },
                {
                    "id": 3,
                    "name": "users.store",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:12.000000Z",
                    "updated_at": "2019-11-19T09:52:12.000000Z"
                },
                {
                    "id": 4,
                    "name": "users.destroy",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:13.000000Z",
                    "updated_at": "2019-11-19T09:52:13.000000Z"
                },
                {
                    "id": 5,
                    "name": "customers.index",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:13.000000Z",
                    "updated_at": "2019-11-19T09:52:13.000000Z"
                },
                {
                    "id": 6,
                    "name": "customers.update",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:14.000000Z",
                    "updated_at": "2019-11-19T09:52:14.000000Z"
                },
                {
                    "id": 7,
                    "name": "customers.store",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:16.000000Z",
                    "updated_at": "2019-11-19T09:52:16.000000Z"
                },
                {
                    "id": 8,
                    "name": "customers.destroy",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:17.000000Z",
                    "updated_at": "2019-11-19T09:52:17.000000Z"
                },
                {
                    "id": 9,
                    "name": "addresses.index",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:18.000000Z",
                    "updated_at": "2019-11-19T09:52:18.000000Z"
                },
                {
                    "id": 10,
                    "name": "addresses.update",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:19.000000Z",
                    "updated_at": "2019-11-19T09:52:19.000000Z"
                },
                {
                    "id": 11,
                    "name": "addresses.store",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:20.000000Z",
                    "updated_at": "2019-11-19T09:52:20.000000Z"
                },
                {
                    "id": 12,
                    "name": "addresses.destroy",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:21.000000Z",
                    "updated_at": "2019-11-19T09:52:21.000000Z"
                },
                {
                    "id": 13,
                    "name": "travels.index",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:22.000000Z",
                    "updated_at": "2019-11-19T09:52:22.000000Z"
                },
                {
                    "id": 14,
                    "name": "travels.update",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:23.000000Z",
                    "updated_at": "2019-11-19T09:52:23.000000Z"
                },
                {
                    "id": 15,
                    "name": "travels.store",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:24.000000Z",
                    "updated_at": "2019-11-19T09:52:24.000000Z"
                },
                {
                    "id": 16,
                    "name": "travels.destroy",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:25.000000Z",
                    "updated_at": "2019-11-19T09:52:25.000000Z"
                },
                {
                    "id": 17,
                    "name": "documents.index",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:26.000000Z",
                    "updated_at": "2019-11-19T09:52:26.000000Z"
                },
                {
                    "id": 18,
                    "name": "documents.update",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:27.000000Z",
                    "updated_at": "2019-11-19T09:52:27.000000Z"
                },
                {
                    "id": 19,
                    "name": "documents.store",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:28.000000Z",
                    "updated_at": "2019-11-19T09:52:28.000000Z"
                },
                {
                    "id": 20,
                    "name": "documents.destroy",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:29.000000Z",
                    "updated_at": "2019-11-19T09:52:29.000000Z"
                },
                {
                    "id": 21,
                    "name": "primary_regnos.index",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:30.000000Z",
                    "updated_at": "2019-11-19T09:52:30.000000Z"
                },
                {
                    "id": 22,
                    "name": "primary_regnos.store",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:31.000000Z",
                    "updated_at": "2019-11-19T09:52:31.000000Z"
                },
                {
                    "id": 23,
                    "name": "primary_regnos.delete",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:32.000000Z",
                    "updated_at": "2019-11-19T09:52:32.000000Z"
                },
                {
                    "id": 24,
                    "name": "primary_regnos.update",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:33.000000Z",
                    "updated_at": "2019-11-19T09:52:33.000000Z"
                },
                {
                    "id": 25,
                    "name": "secondary_regnos.index",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:34.000000Z",
                    "updated_at": "2019-11-19T09:52:34.000000Z"
                },
                {
                    "id": 26,
                    "name": "secondary_regnos.store",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:35.000000Z",
                    "updated_at": "2019-11-19T09:52:35.000000Z"
                },
                {
                    "id": 27,
                    "name": "secondary_regnos.delete",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:36.000000Z",
                    "updated_at": "2019-11-19T09:52:36.000000Z"
                },
                {
                    "id": 28,
                    "name": "secondary_regnos.update",
                    "guard_name": "web",
                    "description": null,
                    "visible": 1,
                    "has_permission": true,
                    "created_at": "2019-11-19T09:52:38.000000Z",
                    "updated_at": "2019-11-19T09:52:38.000000Z"
                }
            ]
},
...
~~~

### Errors
| Code | Message |
| ---- | ------- |
