---
name: Currency
---

# Currency

## Loads all available currency

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/currency`

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

### Response

Response: [currency_flat](/schema/currency_flat.md)
