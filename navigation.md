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
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

{% hint style="info" %}
You can use any Criteria parameter in this Request (e.g `filter`, `associations`, `aggregations`, ...).
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
  "buildTree": true
}
```

### Response

Response: [NavigationRouteResponse](/schema/navigationrouteresponse.md)
