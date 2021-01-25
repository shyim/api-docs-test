---
name: Order
---

# Order

## Cancel a order

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/order/state/cancel`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "orderId": "string"
}
```

### Response

Response: [state_machine_state_flat](/schema/state_machine_state_flat.md)

## Listing orders

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/order`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

{% hint style="info" %}
You can use any Criteria parameter in this Request (e.g `filter`, `associations`, `aggregations`, ...).
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "checkPromotion": "string"
}
```

### Response

List of [order_flat](/schema/order_flat.md)
