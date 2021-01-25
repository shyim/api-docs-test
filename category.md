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

Parameters:

- aggregations: `object` - Contains the requested aggregations
- elements: List of [category_flat](/schema/category_flat.md)
- total: `int64` - Found total entries
