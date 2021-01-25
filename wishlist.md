---
name: Wishlist
---

# Wishlist

## Add a product into customer wishlist

{% hint style="info" %}
Available since: 6.3.4.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/customer/wishlist/add/{productId}`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following methods:
sw-access-key in Header
sw-context-token in Header
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `productId` - string - Product Id

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Fetch customer wishlist

{% hint style="info" %}
Available since: 6.3.4.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/customer/wishlist`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following methods:
sw-access-key in Header
sw-context-token in Header
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

Response: [WishlistLoadRouteResponse](/schema/wishlistloadrouteresponse.md)

## Merge wishlist products from anonymous users to registered users

{% hint style="info" %}
Available since: 6.3.4.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/customer/wishlist/merge`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following methods:
sw-access-key in Header
sw-context-token in Header
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "productIds": [
    "497f6eca-6276-4993-bfeb-53cbbbba6f08"
  ]
}
```

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Delete customer wishlist

{% hint style="info" %}
Available since: 6.3.4.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/customer/wishlist/delete/{productId}`

Method: `DELETE`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following methods:
sw-access-key in Header
sw-context-token in Header
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `productId` - string - Product Id

### Response

Response: [SuccessResponse](/schema/successresponse.md)
