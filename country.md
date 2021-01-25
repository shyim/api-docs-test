---
name: Country
---

# Country

## Loads all available countries

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/country`

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
  "onlyAvailable": 0
}
```

### Response

List of [country_flat](/schema/country_flat.md)
