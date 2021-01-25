---
name: Newsletter
---

# Newsletter

## Confirm newsletter registration

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/newsletter/confirm`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Query Parameters:

- `hash` - string- Optional
Hash from Mail

- `em` - string- Optional
Hash from Mail

## Subscribe to newsletter

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/newsletter/subscribe`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Query Parameters:

- `email` - string- Optional
Email

- `salutationId` - string- Optional
Salutation

- `firstName` - string- Optional
Firstname

- `lastName` - string- Optional
Lastname

- `street` - string- Optional
Street

- `city` - string- Optional
City

- `zipCode` - string- Optional
Zipcode

## Unsubscribe to newsletter

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/newsletter/unsubscribe`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Query Parameters:

- `email` - string- Optional
Email
