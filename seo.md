---
name: Seo
---

# Seo

## Loads seo urls

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/seo-url`

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

List of [seo_url_flat](/schema/seo_url_flat.md)

{% code title="404" %}
```javascript
{
  "errors": [
    {
      "status": "404",
      "title": "Not Found",
      "description": "Resource with given parameter was not found."
    }
  ]
}
```
{% endcode %}

{% code title="404" %}
```javascript
{
  "errors": [
    {
      "status": "404",
      "title": "Not Found",
      "description": "Resource with given parameter was not found."
    }
  ]
}
```
{% endcode %}
