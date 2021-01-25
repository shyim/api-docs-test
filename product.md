---
name: Product
---

# Product

## Export product export

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/product-export/{accessKey}/{fileName}`

Method: `GET`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `accessKey` - string - Access Key

- `fileName` - string - File Name

## This route is used to load the cross sellings for a product. A product has several cross selling definitions in which several products are linked. The route returns the cross sellings together with the linked products

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/product/{productId}/cross-selling`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `productId` - string - Product ID

### Response

Response: [CrossSellingElementCollection](/schema/crosssellingelementcollection.md)

## This route is used to load a single product with the corresponding details. In addition to loading the data, the best variant of the product is determined when a parent id is passed.

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/product/{productId}`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `productId` - string - Product ID

### Response

Response: [product_flat](/schema/product_flat.md)

## Loads products from listing

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/product-listing/{categoryId}`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `categoryId` - string - Category ID

### Response

Response: [ProductListingResult](/schema/productlistingresult.md)

## This route can be used to load the products by specific filters

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/product`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
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
- elements: List of [product_flat](/schema/product_flat.md)
- total: `int64` - Found total entries

## 

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/product/{productId}/reviews`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `productId` - string - Product ID

### Response

List of [product_review_flat](/schema/product_review_flat.md)

## 

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/product/{productId}/review`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `productId` - string - Product ID
