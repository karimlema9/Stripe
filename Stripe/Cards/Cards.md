Cards CRUD
======
## List cards
You can see a list of the cards belonging to a customer. Note that the 10 most recent sources are always available on the Customer object. If you need more than those 10, you can use this API method and the limit and starting_after parameters to page through additional cards.

>Request Headers
~~~
Method:     GET
URI:        /cards
Header:     Authorization 12345678901234567890
~~~
>Request Body
>Attributes with * are required (send without * in the name)
~~~json
{
    "*customer":"cus_G21aZBFSzkBYk4",
    "limit":"1",
    "object":"card",
}
~~~
>Request Response
~~~json
{
    "data": [
        {
            "id": "card_1FWJTKDEGzEAMd49b7yvxJHb",
            "object": "card",
            "address_city": null,
            "address_country": null,
            "address_line1": null,
            "address_line1_check": null,
            "address_line2": null,
            "address_state": null,
            "address_zip": null,
            "address_zip_check": null,
            "brand": "Visa",
            "country": "US",
            "customer": "cus_G21aZBFSzkBYk4",
            "cvc_check": null,
            "dynamic_last4": null,
            "exp_month": 10,
            "exp_year": 2022,
            "fingerprint": "zWn5VWWEdMfDR55X",
            "funding": "credit",
            "last4": "4242",
            "metadata": [],
            "name": "karim",
            "tokenization_method": null
        }
    ]
}
~~~

## Create
To create a card you need to create a card token before. It contains the sensible card information and then it's associated to the new card object with another Stripe API request.

You cannot modify this sensible information. If your information is not correct you have to delete the card and create it again.

>Request Headers
~~~
Method:     POST
URI:        /cards
Header:     Authorization 12345678901234567890
~~~
>Request Body
`*First we create the card token and then we create the card using the token id that we created previously`
>Attributes with * are required (send without * in the name)
~~~json
{
    "*number":4242424242424242,
    "*cvc":158,
    "*exp_month":09,
    "*exp_year":2024,
    "*currency":"EUR",
    "name":"Karim Lemaallam",
    "address_line1":"C/x 10",
    "address_state":"Tarragona",
    "address_zip":43515,
    "address_city":"La Galera",
    "address_country":"Spain"
}

{
    "customer":"cus_G21aZBFSzkBYk4",
    "*source":"$token->id"
}
~~~

>Request Response
~~~json
{
    "data": {
        "id": "card_1FYeTcBXm1E9efrFeoqWX85D",
        "object": "card",
        "address_city": "La Galera",
        "address_country": "Spain",
        "address_line1": "C/x 10",
        "address_line1_check": "pass",
        "address_line2": null,
        "address_state": "Tarragona",
        "address_zip": "43515",
        "address_zip_check": "pass",
        "brand": "Visa",
        "country": "US",
        "customer": "cus_G21aZBFSzkBYk4",
        "cvc_check": "pass",
        "dynamic_last4": null,
        "exp_month": 9,
        "exp_year": 2024,
        "fingerprint": "YW0cpMxsxfKQF9v2",
        "funding": "debit",
        "last4": "4242",
        "metadata": [],
        "name": "Karim Lemaallam",
        "tokenization_method": null
    }
}
~~~

## Update
If you need to update only some card details, like the billing address or expiration date, you can do so without having to re-enter the full card details. Also, Stripe works directly with card networks so that your customers can continue using your service without interruption.

When you update a card, Stripe will automatically validate the card.

>Request Headers
~~~
Method:     PUT
URI:        /cards/{id}
Header:     Authorization 12345678901234567890
~~~
>Request Body
>Attributes with * are required (send without * in the name)
~~~json
{
    "customer":"cus_G21aZBFSzkBYk4",
    "*id":"card_1FYeTcBXm1E9efrFeoqWX85D",
    "address_city":"",
    "address_country":"",
    "address_line1":"",
    "address_line1":"",
    "address_state":"",
    "address_zip":"",
    "exp_month": 02,
    "exp_year": 2024,
    "metadata":"",
    "name":""
}
~~~

>Request Response
~~~json
{
  "id": "card_1FYeTcBXm1E9efrFeoqWX85D",
  "object": "card",
  "address_city": null,
  "address_country": null,
  "address_line1": null,
  "address_line1_check": null,
  "address_line2": null,
  "address_state": null,
  "address_zip": null,
  "address_zip_check": null,
  "brand": "Visa",
  "country": "US",
  "customer": "cus_G21aZBFSzkBYk4",
  "cvc_check": null,
  "dynamic_last4": null,
  "exp_month": 02,
  "exp_year": 2024,
  "fingerprint": "zWn5VWWEdMfDR55X",
  "funding": "credit",
  "last4": "4242",
  "metadata": {},
  "name": "Karim Lemaallam",
  "tokenization_method": null
}
~~~

## Delete
You can delete cards from a customer.
If you delete a card that is currently the default source, then the most recently added source will become the new default. If you delete a card that is the last remaining source on the customer, then the default_source attribute will become null.

For recipients: if you delete the default card, then the most recently added card will become the new default. If you delete the last remaining card on a recipient, then the default_card attribute will become null.

Note that for cards belonging to customers, you might want to prevent customers on paid subscriptions from deleting all cards on file, so that there is at least one default card for the next invoice payment attempt.

>Request Headers
~~~
Method:     DELETE
URI:        /cards/{id}
Header:     Authorization 12345678901234567890
~~~
>Request Body
>Attributes with * are required (send without * in the name)
~~~json
{
    "customer":"cus_G21aZBFSzkBYk4",
    "*id":"card_1FYeTcBXm1E9efrFeoqWX85D",
}
~~~

>Request Response
~~~json
{
  "id": "card_1FYeTcBXm1E9efrFeoqWX85D",
  "object": "card",
  "deleted": true
}
~~~