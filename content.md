---
name: Content
---

# Content

## Loads a category with the resolved cms page

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/category/{categoryId}`

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

- `categoryId` - string - Category ID

### Request

```javascript
{
  "categoryId": "337f5e5d-288b-40d5-be14-901cc3acacc0"
}
```

### Response

Response: [category_flat](/schema/category_flat.md)

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

## Resolves a cms page

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/cms/{id}`

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

- `id` - string - CMS ID

### Response

Response: [cms_page_flat](/schema/cms_page_flat.md)

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
