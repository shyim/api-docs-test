---
name: Language
---

# Language

## Loads all available languages

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/language`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

{% hint style="warning" %}
You can use any Criteria parameter in this Request (e.g `filter`, `associations` load additional data).
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

List of [language_flat](/schema/language_flat.md)
