---
name: Payment Method
---

# Payment Method

## Handles a payment for an order

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/handle-payment`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "orderId": "string",
  "finishUrl": "string",
  "errorUrl": "string"
}
```

## Loads all available payment methods

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/payment-method`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

{% hint style="warning" %}
You can use any Criteria parameter in this Request (e.g `filter`, `associations` load additional data).
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "onlyAvailable": true
}
```

### Response

List of [payment_method_flat](/schema/payment_method_flat.md)
