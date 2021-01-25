---
name: Search
---

# Search

## Search

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/search`

Method: `GET`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Query Parameters:

- `search` - string- Optional
Search term

### Response

Response: [ProductListingResult](/schema/productlistingresult.md)

## Search suggests

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/search-suggest`

Method: `GET`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Query Parameters:

- `search` - string- Optional
Search term

### Response

Response: [ProductListingResult](/schema/productlistingresult.md)
