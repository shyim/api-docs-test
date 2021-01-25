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
To perform this operation, you must be authenticated using following methods:
sw-access-key in Header
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "page": 0,
  "limit": 0,
  "term": "string",
  "filter": [
    {
      "type": "string",
      "field": "string",
      "value": "string"
    }
  ],
  "sort": [
    {
      "field": "string",
      "order": "string",
      "naturalSorting": true
    }
  ],
  "post-filter": [
    {
      "type": "string",
      "field": "string",
      "value": "string"
    }
  ],
  "associations": {},
  "aggregations": [
    {
      "name": "string",
      "type": "string",
      "field": "string"
    }
  ],
  "query": [
    {
      "score": 0,
      "query": {
        "type": "string",
        "field": "string",
        "value": "string"
      }
    }
  ],
  "grouping": [
    "string"
  ]
}
```

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
