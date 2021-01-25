---
name: Account
---

# Account

## Change profile information

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/change-profile`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "salutationId": "string",
  "firstName": "string",
  "lastName": "string"
}
```

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Change email

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/change-email`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "email": "string",
  "emailConfirmation": "string",
  "password": "string"
}
```

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Change password

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/change-password`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "password": "string",
  "newPassword": "string",
  "newPasswordConfirm": "string"
}
```

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Change payment method

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/change-payment-method/{paymentMethodId}`

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

- `paymentMethodId` - string - Payment Method Id

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Change email

{% hint style="info" %}
Available since: 6.3.1.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/customer-group-registration/config/{customerGroupId}`

Method: `GET`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `customerGroupId` - string - Customer Group ID

### Response

Response: [CustomerGroup](/schema/customergroup.md)

## Returns informations about the loggedin customer

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/customer`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

{% hint style="info" %}
You can use any Criteria parameter in this Request (e.g `filter`, `associations`, `aggregations`, ...).
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

Response: [customer_flat](/schema/customer_flat.md)

## Delete customer profile

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/customer`

Method: `DELETE`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Deletes a customer address

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/address/{addressId}`

Method: `DELETE`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `addressId` - string - Address ID

## Update address

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/address/{addressId}`

Method: `PATCH`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `addressId` - string - Address ID

### Request

```javascript
{
  "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
  "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac",
  "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
  "countryStateId": "85904121-4fd9-4405-be13-53c6b1c08b0c",
  "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
  "firstName": "string",
  "lastName": "string",
  "zipcode": "string",
  "city": "string",
  "company": "string",
  "street": "string",
  "department": "string",
  "title": "string",
  "vatId": "string",
  "phoneNumber": "string",
  "additionalAddressLine1": "string",
  "additionalAddressLine2": "string",
  "customFields": {},
  "country": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "name": "string",
    "iso": "string",
    "position": 0,
    "taxFree": true,
    "active": true,
    "shippingAvailable": true,
    "iso3": "string",
    "displayStateInRegistration": true,
    "forceStateInRegistration": true,
    "companyTaxFree": true,
    "checkVatIdPattern": true,
    "vatIdPattern": "string",
    "customFields": {},
    "translated": {},
    "states": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
      "shortCode": "string",
      "name": "string",
      "position": 0,
      "active": true,
      "customFields": {},
      "translated": {},
      "country": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "name": "string",
        "iso": "string",
        "position": 0,
        "taxFree": true,
        "active": true,
        "shippingAvailable": true,
        "iso3": "string",
        "displayStateInRegistration": true,
        "forceStateInRegistration": true,
        "companyTaxFree": true,
        "checkVatIdPattern": true,
        "vatIdPattern": "string",
        "customFields": {},
        "translated": {},
        "states": {
          "id": null,
          "countryId": null,
          "shortCode": null,
          "name": null,
          "position": null,
          "active": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "country": null
        }
      }
    }
  },
  "countryState": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
    "shortCode": "string",
    "name": "string",
    "position": 0,
    "active": true,
    "customFields": {},
    "translated": {},
    "country": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "iso": "string",
      "position": 0,
      "taxFree": true,
      "active": true,
      "shippingAvailable": true,
      "iso3": "string",
      "displayStateInRegistration": true,
      "forceStateInRegistration": true,
      "companyTaxFree": true,
      "checkVatIdPattern": true,
      "vatIdPattern": "string",
      "customFields": {},
      "translated": {},
      "states": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
        "shortCode": "string",
        "name": "string",
        "position": 0,
        "active": true,
        "customFields": {},
        "translated": {},
        "country": {
          "id": null,
          "name": null,
          "iso": null,
          "position": null,
          "taxFree": null,
          "active": null,
          "shippingAvailable": null,
          "iso3": null,
          "displayStateInRegistration": null,
          "forceStateInRegistration": null,
          "companyTaxFree": null,
          "checkVatIdPattern": null,
          "vatIdPattern": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "states": null
        }
      }
    }
  },
  "salutation": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "salutationKey": "string",
    "displayName": "string",
    "letterName": "string",
    "translated": {}
  }
}
```

### Response

Response: [customer_address_flat](/schema/customer_address_flat.md)

## List address

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/list-address`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

{% hint style="info" %}
You can use any Criteria parameter in this Request (e.g `filter`, `associations`, `aggregations`, ...).
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Response

List of [customer_address_flat](/schema/customer_address_flat.md)

## Login as customer using password

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/login`

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
  "username": "string",
  "password": "string"
}
```

### Response

Response: [ContextTokenResponse](/schema/contexttokenresponse.md)

## Logouts current loggedin customer

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/logout`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

## Confirm double optin registration

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/register-confirm`

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
Hash from Link in Mail

- `em` - string- Optional
em from Link in Mail

## Register

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/register`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Query Parameters:

- `guest` - boolean- Optional
Create guest user

- `title` - string- Optional
Title

- `salutationId` - string- Optional
Salutation

- `firstName` - string- Optional
Firstname

- `lastName` - string- Optional
Lastname

- `email` - string- Optional
email

- `affiliateCode` - string- Optional
Affilicate Code

- `campaignCode` - string- Optional
Campaign Code

- `password` - string- Optional
Password

- `billingAddress` - [customer_address_flat](/schema/customer_address_flat.md)- Optional
Billingaddress

- `shippingAddress` - [customer_address_flat](/schema/customer_address_flat.md)- Optional
Shippingaddress

### Response

Response: [customer_flat](/schema/customer_flat.md)

## Resets password using recovery hash

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/recovery-password-confirm`

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
  "hash": "string",
  "newPassword": "string",
  "newPasswordConfirm": "string",
  "storefrontUrl": "string"
}
```

## Sends a recovery email for password recovery

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/recovery-password`

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
  "email": "string",
  "storefrontUrl": "string"
}
```

### Response

Response: [SuccessResponse](/schema/successresponse.md)

## Sets the default shipping address

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/address/default-shipping/{addressId}`

Method: `PATCH`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `addressId` - string - Address ID

## Sets the default billing address

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/address/default-billing/{addressId}`

Method: `PATCH`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

Path Parameters:

- `addressId` - string - Address ID

## Create a new address

{% hint style="info" %}
Available since: 6.3.2.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/account/address`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
  "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac",
  "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
  "countryStateId": "85904121-4fd9-4405-be13-53c6b1c08b0c",
  "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
  "firstName": "string",
  "lastName": "string",
  "zipcode": "string",
  "city": "string",
  "company": "string",
  "street": "string",
  "department": "string",
  "title": "string",
  "vatId": "string",
  "phoneNumber": "string",
  "additionalAddressLine1": "string",
  "additionalAddressLine2": "string",
  "customFields": {},
  "country": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "name": "string",
    "iso": "string",
    "position": 0,
    "taxFree": true,
    "active": true,
    "shippingAvailable": true,
    "iso3": "string",
    "displayStateInRegistration": true,
    "forceStateInRegistration": true,
    "companyTaxFree": true,
    "checkVatIdPattern": true,
    "vatIdPattern": "string",
    "customFields": {},
    "translated": {},
    "states": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
      "shortCode": "string",
      "name": "string",
      "position": 0,
      "active": true,
      "customFields": {},
      "translated": {},
      "country": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "name": "string",
        "iso": "string",
        "position": 0,
        "taxFree": true,
        "active": true,
        "shippingAvailable": true,
        "iso3": "string",
        "displayStateInRegistration": true,
        "forceStateInRegistration": true,
        "companyTaxFree": true,
        "checkVatIdPattern": true,
        "vatIdPattern": "string",
        "customFields": {},
        "translated": {},
        "states": {
          "id": null,
          "countryId": null,
          "shortCode": null,
          "name": null,
          "position": null,
          "active": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "country": null
        }
      }
    }
  },
  "countryState": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
    "shortCode": "string",
    "name": "string",
    "position": 0,
    "active": true,
    "customFields": {},
    "translated": {},
    "country": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "iso": "string",
      "position": 0,
      "taxFree": true,
      "active": true,
      "shippingAvailable": true,
      "iso3": "string",
      "displayStateInRegistration": true,
      "forceStateInRegistration": true,
      "companyTaxFree": true,
      "checkVatIdPattern": true,
      "vatIdPattern": "string",
      "customFields": {},
      "translated": {},
      "states": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "countryId": "bd2b151e-bbbf-43a3-8058-286e653dfac0",
        "shortCode": "string",
        "name": "string",
        "position": 0,
        "active": true,
        "customFields": {},
        "translated": {},
        "country": {
          "id": null,
          "name": null,
          "iso": null,
          "position": null,
          "taxFree": null,
          "active": null,
          "shippingAvailable": null,
          "iso3": null,
          "displayStateInRegistration": null,
          "forceStateInRegistration": null,
          "companyTaxFree": null,
          "checkVatIdPattern": null,
          "vatIdPattern": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "states": null
        }
      }
    }
  },
  "salutation": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "salutationKey": "string",
    "displayName": "string",
    "letterName": "string",
    "translated": {}
  }
}
```

### Response

Response: [customer_address_flat](/schema/customer_address_flat.md)

## set payment for an order

{% hint style="info" %}
Available since: 6.2.0.0
{% endhint %}

Endpoint: `https://my-store.shopware.store/store-api/order/payment`

Method: `POST`

{% hint style="warning" %}
To perform this operation, you must be authenticated using following headers:
sw-access-key
sw-context-token
{% endhint %}

Headers:

- Accept: `application/json`
- Content-Type: `application/json`

### Request

```javascript
{
  "paymentMethodId": "string",
  "orderId": "string"
}
```

### Response

Response: [SuccessResponse](/schema/successresponse.md)
