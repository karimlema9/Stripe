subscriptions CRUD
======
## List
By default, returns a list of subscriptions that have not been canceled. In order to list canceled subscriptions, specify status=canceled.

>Request Headers
~~~
Method:     GET
URI:        /subscriptions
Header:     Authorization 12345678901234567890
~~~
>Request Body
>Attributes with * are required (send without * in the name)
~~~json
{
    "collection_method":null,
    "created":null,
    "current_period_end":null,
    "current_period_start":null,
    "customer":null,
    "ending_before":null,
    "limit":null,
    "plan":null,
    "starting_After":null,
    "status":null
}
~~~
>Request Response
~~~json
{
  "id": "sub_G8PHMtgApHG2sS",
  "object": "subscription",
  "application_fee_percent": null,
  "billing_cycle_anchor": 1573123425,
  "billing_thresholds": null,
  "cancel_at_period_end": false,
  "canceled_at": null,
  "collection_method": "charge_automatically",
  "created": 1573123425,
  "current_period_end": 1573209825,
  "current_period_start": 1573123425,
  "customer": "cus_G21aZBFSzkBYk4",
  "days_until_due": null,
  "default_payment_method": null,
  "default_source": null,
  "default_tax_rates": [],
  "discount": null,
  "ended_at": null,
  "invoice_customer_balance_settings": {
    "consume_applied_balance_on_void": true
  },
  "items": {
    "object": "list",
    "data": [
      {
        "id": "si_G8PHFtKovSqd0t",
        "object": "subscription_item",
        "billing_thresholds": null,
        "created": 1573123426,
        "metadata": {},
        "plan": {
          "id": "plan_G8O7rR5w8wiKre",
          "object": "plan",
          "active": true,
          "aggregate_usage": null,
          "amount": 2200,
          "amount_decimal": "2200",
          "billing_scheme": "per_unit",
          "created": 1573119135,
          "currency": "eur",
          "interval": "day",
          "interval_count": 1,
          "livemode": false,
          "metadata": {},
          "nickname": null,
          "product": "prod_G8O79HQ3Xff1ZE",
          "tiers": null,
          "tiers_mode": null,
          "transform_usage": null,
          "trial_period_days": null,
          "usage_type": "licensed"
        },
        "quantity": 1,
        "subscription": "sub_G8PHMtgApHG2sS",
        "tax_rates": []
      }
    ],
    "has_more": false,
    "url": "/v1/subscription_items?subscription=sub_G8PHMtgApHG2sS"
  },
  "latest_invoice": "in_1Fc8SrDEGzEAMd49tLf3vnOe",
  "livemode": false,
  "metadata": {},
  "next_pending_invoice_item_invoice": null,
  "pending_invoice_item_interval": null,
  "pending_setup_intent": null,
  "plan": {
    "id": "plan_G8O7rR5w8wiKre",
    "object": "plan",
    "active": true,
    "aggregate_usage": null,
    "amount": 2200,
    "amount_decimal": "2200",
    "billing_scheme": "per_unit",
    "created": 1573119135,
    "currency": "eur",
    "interval": "day",
    "interval_count": 1,
    "livemode": false,
    "metadata": {},
    "nickname": null,
    "product": "prod_G8O79HQ3Xff1ZE",
    "tiers": null,
    "tiers_mode": null,
    "transform_usage": null,
    "trial_period_days": null,
    "usage_type": "licensed"
  },
  "quantity": 1,
  "start_date": 1573123425,
  "status": "active",
  "tax_percent": null,
  "trial_end": null,
  "trial_start": null
}
~~~

## Create
Creates a new subscription on an existing customer, in order to create a subscription you must first have created a plan

>Request Headers
~~~
Method:     GET
URI:        /subscriptions
Header:     Authorization 12345678901234567890
~~~
>Request Body
>Attributes with * are required (send without * in the name)
~~~json
{
    "*customer":"cus_G8jGnTTcHP6OUX",
    "application_fee_percent": null,
    "backdate_start_date": null,
    "billing_cycle_anchor": null,
    "billing_thresholds": null,
    "cancel_at_period_end": false,
    "canceled_at": null,
    "collection_method": null,
    "cupon": null,
    "days_until_due": null,
    "default_payment_method": null,
    "default_source": null,
    "default_tax_rates": [],
    "*items":[],
    "metadata":[],
    "off_session": null,
    "payment_behavior": null,
    "pending_invoice_item_interval": null,
    "prorate": null,
    "tax_percent": null,
    "trial_end": null,
    "trial_from_plan": null,
    "trial_period_days": null
}
~~~
>Request Response
~~~json
{
  "id": "sub_G8PHMtgApHG2sS",
  "object": "subscription",
  "application_fee_percent": null,
  "billing_cycle_anchor": 1573123425,
  "billing_thresholds": null,
  "cancel_at_period_end": false,
  "canceled_at": null,
  "collection_method": "charge_automatically",
  "created": 1573123425,
  "current_period_end": 1573209825,
  "current_period_start": 1573123425,
  "customer": "cus_G8jGnTTcHP6OUX",
  "days_until_due": null,
  "default_payment_method": null,
  "default_source": null,
  "default_tax_rates": [],
  "discount": null,
  "ended_at": null,
  "invoice_customer_balance_settings": {
    "consume_applied_balance_on_void": true
  },
  "items": {
    "object": "list",
    "data": [
      {
        "id": "si_G8PHFtKovSqd0t",
        "object": "subscription_item",
        "billing_thresholds": null,
        "created": 1573123426,
        "metadata": {},
        "plan": {
          "id": "plan_G8O7rR5w8wiKre",
          "object": "plan",
          "active": true,
          "aggregate_usage": null,
          "amount": 2200,
          "amount_decimal": "2200",
          "billing_scheme": "per_unit",
          "created": 1573119135,
          "currency": "eur",
          "interval": "day",
          "interval_count": 1,
          "livemode": false,
          "metadata": {},
          "nickname": null,
          "product": "prod_G8O79HQ3Xff1ZE",
          "tiers": null,
          "tiers_mode": null,
          "transform_usage": null,
          "trial_period_days": null,
          "usage_type": "licensed"
        },
        "quantity": 1,
        "subscription": "sub_G8PHMtgApHG2sS",
        "tax_rates": []
      }
    ],
    "has_more": false,
    "url": "/v1/subscription_items?subscription=sub_G8PHMtgApHG2sS"
  },
  "latest_invoice": "in_1Fc8SrDEGzEAMd49tLf3vnOe",
  "livemode": false,
  "metadata": {},
  "next_pending_invoice_item_invoice": null,
  "pending_invoice_item_interval": null,
  "pending_setup_intent": null,
  "plan": {
    "id": "plan_G8O7rR5w8wiKre",
    "object": "plan",
    "active": true,
    "aggregate_usage": null,
    "amount": 2200,
    "amount_decimal": "2200",
    "billing_scheme": "per_unit",
    "created": 1573119135,
    "currency": "eur",
    "interval": "day",
    "interval_count": 1,
    "livemode": false,
    "metadata": {},
    "nickname": null,
    "product": "prod_G8O79HQ3Xff1ZE",
    "tiers": null,
    "tiers_mode": null,
    "transform_usage": null,
    "trial_period_days": null,
    "usage_type": "licensed"
  },
  "quantity": 1,
  "start_date": 1573123425,
  "status": "active",
  "tax_percent": null,
  "trial_end": null,
  "trial_start": null
}
~~~

## Update
Updates an existing subscription to match the specified parameters. When changing plans or quantities, we will optionally prorate the price we charge next month to make up for any price changes. To preview how the proration will be calculated, use the upcoming invoice endpoint.

>Request Headers
~~~
Method:     GET
URI:        /subscriptions
Header:     Authorization 12345678901234567890
~~~
>Request Body
>Attributes with * are required (send without * in the name)
~~~json
{
    "application_fee_percent": null,
    "billing_cycle_anchor": null,
    "billing_thresholds": null,
    "cancel_at_period_end": true,
    "canceled_at": null,
    "collection_method": null,
    "cupon": null,
    "days_until_due": null,
    "default_payment_method": null,
    "default_source": null,
    "default_tax_rates": [],
    "items":[],
    "metadata":[],
    "off_session": null,
    "payment_behavior": null,
    "pending_invoice_item_interval": null,
    "prorate": null,
    "prorate_date": null,
    "tax_percent": null,
    "trial_end": null,
    "trial_from_plan": null,
}
~~~
>Request Response
~~~json
{
  "id": "sub_G8PHMtgApHG2sS",
  "object": "subscription",
  "application_fee_percent": null,
  "billing_cycle_anchor": 1573123425,
  "billing_thresholds": null,
  "cancel_at_period_end": true,
  "canceled_at": null,
  "collection_method": "charge_automatically",
  "created": 1573123425,
  "current_period_end": 1573209825,
  "current_period_start": 1573123425,
  "customer": "cus_G21aZBFSzkBYk4",
  "days_until_due": null,
  "default_payment_method": null,
  "default_source": null,
  "default_tax_rates": [],
  "discount": null,
  "ended_at": null,
  "invoice_customer_balance_settings": {
    "consume_applied_balance_on_void": true
  },
  "items": {
    "object": "list",
    "data": [
      {
        "id": "si_G8PHFtKovSqd0t",
        "object": "subscription_item",
        "billing_thresholds": null,
        "created": 1573123426,
        "metadata": {},
        "plan": {
          "id": "plan_G8O7rR5w8wiKre",
          "object": "plan",
          "active": true,
          "aggregate_usage": null,
          "amount": 2200,
          "amount_decimal": "2200",
          "billing_scheme": "per_unit",
          "created": 1573119135,
          "currency": "eur",
          "interval": "day",
          "interval_count": 1,
          "livemode": false,
          "metadata": {},
          "nickname": null,
          "product": "prod_G8O79HQ3Xff1ZE",
          "tiers": null,
          "tiers_mode": null,
          "transform_usage": null,
          "trial_period_days": null,
          "usage_type": "licensed"
        },
        "quantity": 1,
        "subscription": "sub_G8PHMtgApHG2sS",
        "tax_rates": []
      }
    ],
    "has_more": false,
    "url": "/v1/subscription_items?subscription=sub_G8PHMtgApHG2sS"
  },
  "latest_invoice": "in_1Fc8SrDEGzEAMd49tLf3vnOe",
  "livemode": false,
  "metadata": {
    "order_id": "6735"
  },
  "next_pending_invoice_item_invoice": null,
  "pending_invoice_item_interval": null,
  "pending_setup_intent": null,
  "plan": {
    "id": "plan_G8O7rR5w8wiKre",
    "object": "plan",
    "active": true,
    "aggregate_usage": null,
    "amount": 2200,
    "amount_decimal": "2200",
    "billing_scheme": "per_unit",
    "created": 1573119135,
    "currency": "eur",
    "interval": "day",
    "interval_count": 1,
    "livemode": false,
    "metadata": {},
    "nickname": null,
    "product": "prod_G8O79HQ3Xff1ZE",
    "tiers": null,
    "tiers_mode": null,
    "transform_usage": null,
    "trial_period_days": null,
    "usage_type": "licensed"
  },
  "quantity": 1,
  "start_date": 1573123425,
  "status": "active",
  "tax_percent": null,
  "trial_end": null,
  "trial_start": null
}
~~~

## Cancel
Cancels a customer’s subscription immediately. The customer will not be charged again for the subscription.

>Request Headers
~~~
Method:     GET
URI:        /subscriptions/:id
Header:     Authorization 12345678901234567890
~~~
>Request Body
>Attributes with * are required (send without * in the name)
~~~json
{
    "invoice_now": null,
    "prorate": null
}
~~~
>Request Response
~~~json
{
  "id": "sub_G8PHMtgApHG2sS",
  "object": "subscription",
  "application_fee_percent": null,
  "billing_cycle_anchor": 1573123425,
  "billing_thresholds": null,
  "cancel_at_period_end": false,
  "canceled_at": null,
  "collection_method": "charge_automatically",
  "created": 1573123425,
  "current_period_end": 1573209825,
  "current_period_start": 1573123425,
  "customer": "cus_G21aZBFSzkBYk4",
  "days_until_due": null,
  "default_payment_method": null,
  "default_source": null,
  "default_tax_rates": [],
  "discount": null,
  "ended_at": null,
  "invoice_customer_balance_settings": {
    "consume_applied_balance_on_void": true
  },
  "items": {
    "object": "list",
    "data": [
      {
        "id": "si_G8PHFtKovSqd0t",
        "object": "subscription_item",
        "billing_thresholds": null,
        "created": 1573123426,
        "metadata": {},
        "plan": {
          "id": "plan_G8O7rR5w8wiKre",
          "object": "plan",
          "active": true,
          "aggregate_usage": null,
          "amount": 2200,
          "amount_decimal": "2200",
          "billing_scheme": "per_unit",
          "created": 1573119135,
          "currency": "eur",
          "interval": "day",
          "interval_count": 1,
          "livemode": false,
          "metadata": {},
          "nickname": null,
          "product": "prod_G8O79HQ3Xff1ZE",
          "tiers": null,
          "tiers_mode": null,
          "transform_usage": null,
          "trial_period_days": null,
          "usage_type": "licensed"
        },
        "quantity": 1,
        "subscription": "sub_G8PHMtgApHG2sS",
        "tax_rates": []
      }
    ],
    "has_more": false,
    "url": "/v1/subscription_items?subscription=sub_G8PHMtgApHG2sS"
  },
  "latest_invoice": "in_1Fc8SrDEGzEAMd49tLf3vnOe",
  "livemode": false,
  "metadata": {},
  "next_pending_invoice_item_invoice": null,
  "pending_invoice_item_interval": null,
  "pending_setup_intent": null,
  "plan": {
    "id": "plan_G8O7rR5w8wiKre",
    "object": "plan",
    "active": true,
    "aggregate_usage": null,
    "amount": 2200,
    "amount_decimal": "2200",
    "billing_scheme": "per_unit",
    "created": 1573119135,
    "currency": "eur",
    "interval": "day",
    "interval_count": 1,
    "livemode": false,
    "metadata": {},
    "nickname": null,
    "product": "prod_G8O79HQ3Xff1ZE",
    "tiers": null,
    "tiers_mode": null,
    "transform_usage": null,
    "trial_period_days": null,
    "usage_type": "licensed"
  },
  "quantity": 1,
  "start_date": 1573123425,
  "status": "active",
  "tax_percent": null,
  "trial_end": null,
  "trial_start": null
}
~~~
