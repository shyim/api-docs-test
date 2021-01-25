---
name: Category
---

# Category

## This route can be used to load categories

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/category`

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

Parameters:

- aggregations: `object` - Contains the requested aggregations
- elements: List of [category_flat](/schema/category_flat.md)
- total: `int64` - Found total entries
