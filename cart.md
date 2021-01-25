---
name: Cart
---

# Cart

## Fetch current cart

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/checkout/cart`

Method: `GET`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

Response: [Cart](/schema/cart.md)

## Delete the cart

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/checkout/cart`

Method: `DELETE`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Add new line item entries

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/checkout/cart/line-item`

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
  "items": [
    {
      "id": "string",
      "referencedId": "string",
      "label": "string",
      "quantity": 0,
      "type": "string",
      "good": true,
      "description": "string",
      "removable": true,
      "stackable": true,
      "modified": true
    }
  ]
}
```

### Response

Response: [Cart](/schema/cart.md)

## Remove line item entries

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/checkout/cart/line-item`

Method: `DELETE`

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
  "ids": [
    "string"
  ]
}
```

### Response

Response: [Cart](/schema/cart.md)

## Update line item entries

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/checkout/cart/line-item`

Method: `PATCH`

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
  "items": [
    {
      "id": "string",
      "referencedId": "string",
      "label": "string",
      "quantity": 0,
      "type": "string",
      "good": true,
      "description": "string",
      "removable": true,
      "stackable": true,
      "modified": true
    }
  ]
}
```

### Response

Response: [Cart](/schema/cart.md)

## Create a new order from cart

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/checkout/order`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

Response: [order_flat](/schema/order_flat.md)
