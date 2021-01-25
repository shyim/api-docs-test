---
name: Context
---

# Context

## Read the context

{% hint style="info" %}
Available since: 6.3.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/context`

Method: `GET`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

Response: [SalesChannelContext](/schema/saleschannelcontext.md)

## Update the context

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/context`

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
  "currencyId": "2a59a322-927b-4fc7-bac8-d295c634b295",
  "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
  "billingAddressId": "b19f2d6f-7332-4fea-a0d5-33be6fb6b7b4",
  "shippingAddressId": "622fc513-c50b-4df6-b9e2-85298a2851fb",
  "paymentMethodId": "b6df8625-cd25-4123-b345-638aa7b5d011",
  "shippingMethodId": "ea3a5f49-4f0a-4467-bd32-114aa00d0649",
  "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
  "countryStateId": "85904121-4fd9-4405-be13-53c6b1c08b0c"
}
```

### Response

Response: [ContextTokenResponse](/schema/contexttokenresponse.md)
