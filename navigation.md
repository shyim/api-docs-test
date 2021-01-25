---
name: Navigation
---

# Navigation

## Loads all available navigations

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/navigation/{requestActiveId}/{requestRootId}`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following methods:
sw-access-key in Header
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `requestActiveId` - string - Active Category ID

- `requestRootId` - string - Root Category ID

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
  ],
  "buildTree": true
}
```

### Response

Response: [NavigationRouteResponse](/schema/navigationrouteresponse.md)
