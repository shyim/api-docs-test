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
  "customer": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
    "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
    "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
    "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
    "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
    "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
    "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
    "customerNumber": "string",
    "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
    "firstName": "string",
    "lastName": "string",
    "company": "string",
    "email": "string",
    "title": "string",
    "vatIds": [
      "string"
    ],
    "affiliateCode": "string",
    "campaignCode": "string",
    "active": true,
    "doubleOptInRegistration": true,
    "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
    "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
    "hash": "string",
    "guest": true,
    "firstLogin": "2019-08-24T14:15:22Z",
    "lastLogin": "2019-08-24T14:15:22Z",
    "newsletter": true,
    "birthday": "string",
    "customFields": {},
    "remoteAddress": "string",
    "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
    "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
    "group": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "displayGross": true,
      "customFields": {},
      "registrationActive": true,
      "registrationTitle": "string",
      "registrationIntroduction": "string",
      "registrationOnlyCompanyRegistration": true,
      "registrationSeoMetaDescription": "string",
      "translated": {}
    },
    "defaultPaymentMethod": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "pluginId": "91f8cbd0-11f2-4669-9910-90a5a0b7d84a",
      "name": "string",
      "description": "string",
      "position": 0,
      "active": true,
      "afterOrderEnabled": true,
      "customFields": {},
      "availabilityRuleId": "0663b9f4-e343-4d2c-8b2d-d04634bd73f4",
      "mediaId": "5a8ffac5-2288-485d-b463-90c3cd9941ad",
      "translated": {},
      "media": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "alt": "string",
        "title": "string",
        "url": "string",
        "hasFile": true,
        "private": true,
        "customFields": {},
        "translated": {},
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "thumbnails": {
          "id": null,
          "mediaId": null,
          "width": null,
          "height": null,
          "url": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "media": null
        }
      },
      "availabilityRule": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "name": "string",
        "priority": 0,
        "description": "string",
        "customFields": {},
        "moduleTypes": {},
        "conditions": {
          "id": null,
          "type": null,
          "ruleId": null,
          "parentId": null,
          "value": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "rule": null,
          "children": null
        }
      }
    },
    "language": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "parentId": "70850378-7d3c-4f45-91b7-942d4dfbbd43",
      "localeId": "65dddce3-df9b-4388-848d-c335be91b332",
      "translationCodeId": "0c50e320-8f49-4543-afca-9ac1efcdfe51",
      "name": "string",
      "customFields": {},
      "locale": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "code": "string",
        "name": "string",
        "territory": "string",
        "customFields": {},
        "translated": {},
        "languages": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        }
      },
      "translationCode": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "code": "string",
        "name": "string",
        "territory": "string",
        "customFields": {},
        "translated": {},
        "languages": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        }
      },
      "children": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "parentId": "70850378-7d3c-4f45-91b7-942d4dfbbd43",
        "localeId": "65dddce3-df9b-4388-848d-c335be91b332",
        "translationCodeId": "0c50e320-8f49-4543-afca-9ac1efcdfe51",
        "name": "string",
        "customFields": {},
        "locale": {
          "id": null,
          "code": null,
          "name": null,
          "territory": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "languages": null
        },
        "translationCode": {
          "id": null,
          "code": null,
          "name": null,
          "territory": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "languages": null
        },
        "children": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        }
      }
    },
    "lastPaymentMethod": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "pluginId": "91f8cbd0-11f2-4669-9910-90a5a0b7d84a",
      "name": "string",
      "description": "string",
      "position": 0,
      "active": true,
      "afterOrderEnabled": true,
      "customFields": {},
      "availabilityRuleId": "0663b9f4-e343-4d2c-8b2d-d04634bd73f4",
      "mediaId": "5a8ffac5-2288-485d-b463-90c3cd9941ad",
      "translated": {},
      "media": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "alt": "string",
        "title": "string",
        "url": "string",
        "hasFile": true,
        "private": true,
        "customFields": {},
        "translated": {},
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "thumbnails": {
          "id": null,
          "mediaId": null,
          "width": null,
          "height": null,
          "url": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "media": null
        }
      },
      "availabilityRule": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "name": "string",
        "priority": 0,
        "description": "string",
        "customFields": {},
        "moduleTypes": {},
        "conditions": {
          "id": null,
          "type": null,
          "ruleId": null,
          "parentId": null,
          "value": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "rule": null,
          "children": null
        }
      }
    },
    "defaultBillingAddress": {
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
      "customer": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
        "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
        "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
        "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
        "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
        "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
        "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
        "customerNumber": "string",
        "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
        "firstName": "string",
        "lastName": "string",
        "company": "string",
        "email": "string",
        "title": "string",
        "vatIds": [
          "string"
        ],
        "affiliateCode": "string",
        "campaignCode": "string",
        "active": true,
        "doubleOptInRegistration": true,
        "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
        "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
        "hash": "string",
        "guest": true,
        "firstLogin": "2019-08-24T14:15:22Z",
        "lastLogin": "2019-08-24T14:15:22Z",
        "newsletter": true,
        "birthday": "string",
        "customFields": {},
        "remoteAddress": "string",
        "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
        "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
        "group": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "defaultPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "language": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        },
        "lastPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "defaultBillingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "defaultShippingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "salutation": {
          "id": null,
          "salutationKey": null,
          "displayName": null,
          "letterName": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "addresses": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "promotions": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "recoveryCustomer": {
          "id": null,
          "hash": null,
          "customerId": null,
          "createdAt": null,
          "updatedAt": null
        },
        "requestedGroup": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "wishlists": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        }
      },
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
      },
      "salutation": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "salutationKey": "string",
        "displayName": "string",
        "letterName": "string",
        "translated": {}
      }
    },
    "defaultShippingAddress": {
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
      "customer": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
        "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
        "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
        "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
        "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
        "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
        "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
        "customerNumber": "string",
        "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
        "firstName": "string",
        "lastName": "string",
        "company": "string",
        "email": "string",
        "title": "string",
        "vatIds": [
          "string"
        ],
        "affiliateCode": "string",
        "campaignCode": "string",
        "active": true,
        "doubleOptInRegistration": true,
        "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
        "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
        "hash": "string",
        "guest": true,
        "firstLogin": "2019-08-24T14:15:22Z",
        "lastLogin": "2019-08-24T14:15:22Z",
        "newsletter": true,
        "birthday": "string",
        "customFields": {},
        "remoteAddress": "string",
        "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
        "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
        "group": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "defaultPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "language": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        },
        "lastPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "defaultBillingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "defaultShippingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "salutation": {
          "id": null,
          "salutationKey": null,
          "displayName": null,
          "letterName": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "addresses": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "promotions": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "recoveryCustomer": {
          "id": null,
          "hash": null,
          "customerId": null,
          "createdAt": null,
          "updatedAt": null
        },
        "requestedGroup": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "wishlists": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        }
      },
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
      },
      "salutation": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "salutationKey": "string",
        "displayName": "string",
        "letterName": "string",
        "translated": {}
      }
    },
    "salutation": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "salutationKey": "string",
      "displayName": "string",
      "letterName": "string",
      "translated": {}
    },
    "addresses": {
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
      "customer": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
        "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
        "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
        "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
        "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
        "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
        "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
        "customerNumber": "string",
        "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
        "firstName": "string",
        "lastName": "string",
        "company": "string",
        "email": "string",
        "title": "string",
        "vatIds": [
          "string"
        ],
        "affiliateCode": "string",
        "campaignCode": "string",
        "active": true,
        "doubleOptInRegistration": true,
        "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
        "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
        "hash": "string",
        "guest": true,
        "firstLogin": "2019-08-24T14:15:22Z",
        "lastLogin": "2019-08-24T14:15:22Z",
        "newsletter": true,
        "birthday": "string",
        "customFields": {},
        "remoteAddress": "string",
        "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
        "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
        "group": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "defaultPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "language": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        },
        "lastPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "defaultBillingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "defaultShippingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "salutation": {
          "id": null,
          "salutationKey": null,
          "displayName": null,
          "letterName": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "addresses": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "promotions": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "recoveryCustomer": {
          "id": null,
          "hash": null,
          "customerId": null,
          "createdAt": null,
          "updatedAt": null
        },
        "requestedGroup": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "wishlists": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        }
      },
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
      },
      "salutation": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "salutationKey": "string",
        "displayName": "string",
        "letterName": "string",
        "translated": {}
      }
    },
    "tags": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string"
    },
    "promotions": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "active": true,
      "validFrom": "2019-08-24T14:15:22Z",
      "validUntil": "2019-08-24T14:15:22Z",
      "maxRedemptionsGlobal": 0,
      "maxRedemptionsPerCustomer": 0,
      "exclusive": true,
      "code": "string",
      "useCodes": true,
      "useIndividualCodes": true,
      "individualCodePattern": "string",
      "useSetGroups": true,
      "customerRestriction": true,
      "exclusionIds": [
        "497f6eca-6276-4993-bfeb-53cbbbba6f08"
      ],
      "translated": {},
      "setgroups": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "promotionId": "3eaf888b-516c-4eac-ac00-1312640986a2",
        "packagerKey": "string",
        "sorterKey": "string",
        "value": 0,
        "promotion": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "setGroupRules": {
          "id": null,
          "name": null,
          "priority": null,
          "description": null,
          "invalid": null,
          "customFields": null,
          "moduleTypes": null,
          "createdAt": null,
          "updatedAt": null,
          "conditions": null
        }
      },
      "discounts": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "promotionId": "3eaf888b-516c-4eac-ac00-1312640986a2",
        "scope": "string",
        "type": "string",
        "value": 0,
        "considerAdvancedRules": true,
        "maxValue": 0,
        "sorterKey": "string",
        "applierKey": "string",
        "usageKey": "string",
        "pickerKey": "string",
        "promotion": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "discountRules": {
          "id": null,
          "name": null,
          "priority": null,
          "description": null,
          "invalid": null,
          "customFields": null,
          "moduleTypes": null,
          "createdAt": null,
          "updatedAt": null,
          "conditions": null
        },
        "promotionDiscountPrices": {
          "id": null,
          "discountId": null,
          "currencyId": null,
          "price": null,
          "createdAt": null,
          "updatedAt": null,
          "promotionDiscount": null,
          "currency": null
        }
      },
      "individualCodes": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "promotionId": "3eaf888b-516c-4eac-ac00-1312640986a2",
        "code": "string",
        "payload": {},
        "promotion": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        }
      }
    },
    "productReviews": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "productId": "dcd53ddb-8104-4e48-8cc0-5df1088c6113",
      "productVersionId": "5b05daeb-e87a-4ecb-b86e-5a255751de62",
      "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac",
      "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
      "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
      "title": "string",
      "content": "string",
      "points": 0,
      "status": true,
      "comment": "string",
      "product": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "versionId": "14707576-2549-4848-82ed-f68f8a1b47c7",
        "parentId": "70850378-7d3c-4f45-91b7-942d4dfbbd43",
        "parentVersionId": "abf80970-9686-419e-bc00-5ddcccc33ba6",
        "manufacturerId": "9ffb4bad-5601-46bd-b5e1-ad29632f5942",
        "productManufacturerVersionId": "5ef9ccce-1f92-4e66-8849-d8c0189982ac",
        "unitId": "b3eb5f92-604a-46b9-9881-9d84000fd7ed",
        "taxId": "ec2f3321-4009-45bd-9423-63aa80044823",
        "coverId": "5fd178bd-f51e-4f24-9612-1857445ad9a8",
        "productMediaVersionId": "3efabe4d-e6f2-4a60-8d52-da6b7965a512",
        "deliveryTimeId": "51e5fd22-fee3-465a-add1-953ad7b5b8a5",
        "productNumber": "string",
        "stock": 0,
        "restockTime": 0,
        "active": true,
        "isCloseout": true,
        "mainVariantId": "a9d54517-b96a-4591-954a-c25556fc138e",
        "manufacturerNumber": "string",
        "ean": "string",
        "purchaseSteps": 0,
        "maxPurchase": 0,
        "minPurchase": 0,
        "purchaseUnit": 0,
        "referenceUnit": 0,
        "shippingFree": true,
        "purchasePrice": 0,
        "markAsTopseller": true,
        "weight": 0,
        "width": 0,
        "height": 0,
        "length": 0,
        "releaseDate": "2019-08-24T14:15:22Z",
        "customFieldSetSelectionActive": true,
        "metaDescription": "string",
        "name": "string",
        "keywords": "string",
        "description": "string",
        "metaTitle": "string",
        "packUnit": "string",
        "packUnitPlural": "string",
        "customFields": {},
        "variation": [
          "string"
        ],
        "featureSetId": "2c884e24-6788-4ec2-9c3d-8b6baa0d5c24",
        "purchasePrices": {},
        "customSearchKeywords": [
          {}
        ],
        "canonicalProductId": "9d6b51f1-2410-4453-85db-e0d2bc76bed8",
        "calculatedPrice": {},
        "calculatedListingPrice": {},
        "calculatedPrices": [
          {}
        ],
        "calculatedMaxPurchase": 0,
        "isNew": true,
        "translated": {},
        "children": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "manufacturerId": null,
          "productManufacturerVersionId": null,
          "unitId": null,
          "taxId": null,
          "coverId": null,
          "productMediaVersionId": null,
          "deliveryTimeId": null,
          "productNumber": null,
          "stock": null,
          "restockTime": null,
          "autoIncrement": null,
          "active": null,
          "availableStock": null,
          "available": null,
          "isCloseout": null,
          "displayGroup": null,
          "mainVariantId": null,
          "manufacturerNumber": null,
          "ean": null,
          "purchaseSteps": null,
          "maxPurchase": null,
          "minPurchase": null,
          "purchaseUnit": null,
          "referenceUnit": null,
          "shippingFree": null,
          "purchasePrice": null,
          "markAsTopseller": null,
          "weight": null,
          "width": null,
          "height": null,
          "length": null,
          "releaseDate": null,
          "ratingAverage": null,
          "categoryTree": null,
          "propertyIds": null,
          "optionIds": null,
          "tagIds": null,
          "childCount": null,
          "customFieldSetSelectionActive": null,
          "sales": null,
          "metaDescription": null,
          "name": null,
          "keywords": null,
          "description": null,
          "metaTitle": null,
          "packUnit": null,
          "packUnitPlural": null,
          "customFields": null,
          "variation": null,
          "featureSetId": null,
          "purchasePrices": null,
          "customSearchKeywords": null,
          "canonicalProductId": null,
          "calculatedPrice": null,
          "calculatedListingPrice": null,
          "calculatedPrices": null,
          "calculatedMaxPurchase": null,
          "isNew": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "deliveryTime": null,
          "tax": null,
          "manufacturer": null,
          "unit": null,
          "cover": null,
          "media": null,
          "crossSellings": null,
          "crossSellingAssignedProducts": null,
          "productReviews": null,
          "mainCategories": null,
          "seoUrls": null,
          "options": null,
          "properties": null,
          "categories": null,
          "categoriesRo": null,
          "tags": null,
          "customFieldSets": null,
          "featureSet": null,
          "wishlists": null,
          "canonicalProduct": null,
          "seoCategory": null
        },
        "deliveryTime": {
          "id": null,
          "name": null,
          "min": null,
          "max": null,
          "unit": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "shippingMethods": null
        },
        "tax": {
          "id": null,
          "taxRate": null,
          "name": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null,
          "shippingMethods": null
        },
        "manufacturer": {
          "id": null,
          "versionId": null,
          "mediaId": null,
          "link": null,
          "name": null,
          "description": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "products": null
        },
        "unit": {
          "id": null,
          "shortCode": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "products": null
        },
        "cover": {
          "id": null,
          "versionId": null,
          "productId": null,
          "productVersionId": null,
          "mediaId": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "media": null
        },
        "media": {
          "id": null,
          "versionId": null,
          "productId": null,
          "productVersionId": null,
          "mediaId": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "media": null
        },
        "crossSellings": {
          "id": null,
          "name": null,
          "position": null,
          "sortBy": null,
          "sortDirection": null,
          "type": null,
          "active": null,
          "limit": null,
          "productId": null,
          "productVersionId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "product": null,
          "assignedProducts": null
        },
        "crossSellingAssignedProducts": {
          "id": null,
          "crossSellingId": null,
          "productId": null,
          "productVersionId": null,
          "position": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "crossSelling": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "mainCategories": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "categoryId": null,
          "categoryVersionId": null,
          "salesChannelId": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "category": null
        },
        "seoUrls": {
          "id": null,
          "salesChannelId": null,
          "languageId": null,
          "foreignKey": null,
          "routeName": null,
          "pathInfo": null,
          "seoPathInfo": null,
          "isCanonical": null,
          "isModified": null,
          "isDeleted": null,
          "url": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "language": null
        },
        "options": {
          "id": null,
          "groupId": null,
          "name": null,
          "position": null,
          "colorHexCode": null,
          "mediaId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "group": null,
          "productConfiguratorSettings": null,
          "productProperties": null,
          "productOptions": null
        },
        "properties": {
          "id": null,
          "groupId": null,
          "name": null,
          "position": null,
          "colorHexCode": null,
          "mediaId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "group": null,
          "productConfiguratorSettings": null,
          "productProperties": null,
          "productOptions": null
        },
        "categories": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "afterCategoryId": null,
          "afterCategoryVersionId": null,
          "mediaId": null,
          "displayNestedProducts": null,
          "autoIncrement": null,
          "breadcrumb": null,
          "level": null,
          "path": null,
          "childCount": null,
          "type": null,
          "productAssignmentType": null,
          "visible": null,
          "active": null,
          "name": null,
          "customFields": null,
          "slotConfig": null,
          "externalLink": null,
          "description": null,
          "metaTitle": null,
          "metaDescription": null,
          "keywords": null,
          "cmsPageId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "media": null,
          "products": null,
          "nestedProducts": null,
          "tags": null,
          "cmsPage": null,
          "productStream": null,
          "mainCategories": null,
          "seoUrls": null
        },
        "categoriesRo": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "afterCategoryId": null,
          "afterCategoryVersionId": null,
          "mediaId": null,
          "displayNestedProducts": null,
          "autoIncrement": null,
          "breadcrumb": null,
          "level": null,
          "path": null,
          "childCount": null,
          "type": null,
          "productAssignmentType": null,
          "visible": null,
          "active": null,
          "name": null,
          "customFields": null,
          "slotConfig": null,
          "externalLink": null,
          "description": null,
          "metaTitle": null,
          "metaDescription": null,
          "keywords": null,
          "cmsPageId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "media": null,
          "products": null,
          "nestedProducts": null,
          "tags": null,
          "cmsPage": null,
          "productStream": null,
          "mainCategories": null,
          "seoUrls": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "customFieldSets": {
          "id": null,
          "name": null,
          "config": null,
          "active": null,
          "global": null,
          "position": null,
          "appId": null,
          "createdAt": null,
          "updatedAt": null,
          "customFields": null,
          "relations": null,
          "products": null,
          "app": null
        },
        "featureSet": {
          "id": null,
          "name": null,
          "description": null,
          "features": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "products": null
        },
        "wishlists": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "wishlistId": null,
          "createdAt": null,
          "updatedAt": null,
          "wishlist": null,
          "product": null
        },
        "canonicalProduct": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "manufacturerId": null,
          "productManufacturerVersionId": null,
          "unitId": null,
          "taxId": null,
          "coverId": null,
          "productMediaVersionId": null,
          "deliveryTimeId": null,
          "productNumber": null,
          "stock": null,
          "restockTime": null,
          "autoIncrement": null,
          "active": null,
          "availableStock": null,
          "available": null,
          "isCloseout": null,
          "displayGroup": null,
          "mainVariantId": null,
          "manufacturerNumber": null,
          "ean": null,
          "purchaseSteps": null,
          "maxPurchase": null,
          "minPurchase": null,
          "purchaseUnit": null,
          "referenceUnit": null,
          "shippingFree": null,
          "purchasePrice": null,
          "markAsTopseller": null,
          "weight": null,
          "width": null,
          "height": null,
          "length": null,
          "releaseDate": null,
          "ratingAverage": null,
          "categoryTree": null,
          "propertyIds": null,
          "optionIds": null,
          "tagIds": null,
          "childCount": null,
          "customFieldSetSelectionActive": null,
          "sales": null,
          "metaDescription": null,
          "name": null,
          "keywords": null,
          "description": null,
          "metaTitle": null,
          "packUnit": null,
          "packUnitPlural": null,
          "customFields": null,
          "variation": null,
          "featureSetId": null,
          "purchasePrices": null,
          "customSearchKeywords": null,
          "canonicalProductId": null,
          "calculatedPrice": null,
          "calculatedListingPrice": null,
          "calculatedPrices": null,
          "calculatedMaxPurchase": null,
          "isNew": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "deliveryTime": null,
          "tax": null,
          "manufacturer": null,
          "unit": null,
          "cover": null,
          "media": null,
          "crossSellings": null,
          "crossSellingAssignedProducts": null,
          "productReviews": null,
          "mainCategories": null,
          "seoUrls": null,
          "options": null,
          "properties": null,
          "categories": null,
          "categoriesRo": null,
          "tags": null,
          "customFieldSets": null,
          "featureSet": null,
          "wishlists": null,
          "canonicalProduct": null,
          "seoCategory": null
        },
        "seoCategory": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "afterCategoryId": null,
          "afterCategoryVersionId": null,
          "mediaId": null,
          "displayNestedProducts": null,
          "autoIncrement": null,
          "breadcrumb": null,
          "level": null,
          "path": null,
          "childCount": null,
          "type": null,
          "productAssignmentType": null,
          "visible": null,
          "active": null,
          "name": null,
          "customFields": null,
          "slotConfig": null,
          "externalLink": null,
          "description": null,
          "metaTitle": null,
          "metaDescription": null,
          "keywords": null,
          "cmsPageId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "media": null,
          "products": null,
          "nestedProducts": null,
          "tags": null,
          "cmsPage": null,
          "productStream": null,
          "mainCategories": null,
          "seoUrls": null
        }
      }
    },
    "recoveryCustomer": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "hash": "string",
      "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac"
    },
    "requestedGroup": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "displayGross": true,
      "customFields": {},
      "registrationActive": true,
      "registrationTitle": "string",
      "registrationIntroduction": "string",
      "registrationOnlyCompanyRegistration": true,
      "registrationSeoMetaDescription": "string",
      "translated": {}
    },
    "wishlists": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac",
      "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
      "customFields": {},
      "products": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "productId": "dcd53ddb-8104-4e48-8cc0-5df1088c6113",
        "productVersionId": "5b05daeb-e87a-4ecb-b86e-5a255751de62",
        "wishlistId": "cbe1353c-385f-4d1b-807a-83768b4af636",
        "wishlist": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        },
        "product": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "manufacturerId": null,
          "productManufacturerVersionId": null,
          "unitId": null,
          "taxId": null,
          "coverId": null,
          "productMediaVersionId": null,
          "deliveryTimeId": null,
          "productNumber": null,
          "stock": null,
          "restockTime": null,
          "autoIncrement": null,
          "active": null,
          "availableStock": null,
          "available": null,
          "isCloseout": null,
          "displayGroup": null,
          "mainVariantId": null,
          "manufacturerNumber": null,
          "ean": null,
          "purchaseSteps": null,
          "maxPurchase": null,
          "minPurchase": null,
          "purchaseUnit": null,
          "referenceUnit": null,
          "shippingFree": null,
          "purchasePrice": null,
          "markAsTopseller": null,
          "weight": null,
          "width": null,
          "height": null,
          "length": null,
          "releaseDate": null,
          "ratingAverage": null,
          "categoryTree": null,
          "propertyIds": null,
          "optionIds": null,
          "tagIds": null,
          "childCount": null,
          "customFieldSetSelectionActive": null,
          "sales": null,
          "metaDescription": null,
          "name": null,
          "keywords": null,
          "description": null,
          "metaTitle": null,
          "packUnit": null,
          "packUnitPlural": null,
          "customFields": null,
          "variation": null,
          "featureSetId": null,
          "purchasePrices": null,
          "customSearchKeywords": null,
          "canonicalProductId": null,
          "calculatedPrice": null,
          "calculatedListingPrice": null,
          "calculatedPrices": null,
          "calculatedMaxPurchase": null,
          "isNew": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "deliveryTime": null,
          "tax": null,
          "manufacturer": null,
          "unit": null,
          "cover": null,
          "media": null,
          "crossSellings": null,
          "crossSellingAssignedProducts": null,
          "productReviews": null,
          "mainCategories": null,
          "seoUrls": null,
          "options": null,
          "properties": null,
          "categories": null,
          "categoriesRo": null,
          "tags": null,
          "customFieldSets": null,
          "featureSet": null,
          "wishlists": null,
          "canonicalProduct": null,
          "seoCategory": null
        }
      }
    }
  },
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

- `billingAddress` - [customer_address_flat](/schema/customer_address_flat)- Optional
Billingaddress

- `shippingAddress` - [customer_address_flat](/schema/customer_address_flat)- Optional
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
  "customer": {
    "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
    "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
    "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
    "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
    "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
    "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
    "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
    "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
    "customerNumber": "string",
    "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
    "firstName": "string",
    "lastName": "string",
    "company": "string",
    "email": "string",
    "title": "string",
    "vatIds": [
      "string"
    ],
    "affiliateCode": "string",
    "campaignCode": "string",
    "active": true,
    "doubleOptInRegistration": true,
    "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
    "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
    "hash": "string",
    "guest": true,
    "firstLogin": "2019-08-24T14:15:22Z",
    "lastLogin": "2019-08-24T14:15:22Z",
    "newsletter": true,
    "birthday": "string",
    "customFields": {},
    "remoteAddress": "string",
    "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
    "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
    "group": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "displayGross": true,
      "customFields": {},
      "registrationActive": true,
      "registrationTitle": "string",
      "registrationIntroduction": "string",
      "registrationOnlyCompanyRegistration": true,
      "registrationSeoMetaDescription": "string",
      "translated": {}
    },
    "defaultPaymentMethod": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "pluginId": "91f8cbd0-11f2-4669-9910-90a5a0b7d84a",
      "name": "string",
      "description": "string",
      "position": 0,
      "active": true,
      "afterOrderEnabled": true,
      "customFields": {},
      "availabilityRuleId": "0663b9f4-e343-4d2c-8b2d-d04634bd73f4",
      "mediaId": "5a8ffac5-2288-485d-b463-90c3cd9941ad",
      "translated": {},
      "media": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "alt": "string",
        "title": "string",
        "url": "string",
        "hasFile": true,
        "private": true,
        "customFields": {},
        "translated": {},
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "thumbnails": {
          "id": null,
          "mediaId": null,
          "width": null,
          "height": null,
          "url": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "media": null
        }
      },
      "availabilityRule": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "name": "string",
        "priority": 0,
        "description": "string",
        "customFields": {},
        "moduleTypes": {},
        "conditions": {
          "id": null,
          "type": null,
          "ruleId": null,
          "parentId": null,
          "value": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "rule": null,
          "children": null
        }
      }
    },
    "language": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "parentId": "70850378-7d3c-4f45-91b7-942d4dfbbd43",
      "localeId": "65dddce3-df9b-4388-848d-c335be91b332",
      "translationCodeId": "0c50e320-8f49-4543-afca-9ac1efcdfe51",
      "name": "string",
      "customFields": {},
      "locale": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "code": "string",
        "name": "string",
        "territory": "string",
        "customFields": {},
        "translated": {},
        "languages": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        }
      },
      "translationCode": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "code": "string",
        "name": "string",
        "territory": "string",
        "customFields": {},
        "translated": {},
        "languages": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        }
      },
      "children": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "parentId": "70850378-7d3c-4f45-91b7-942d4dfbbd43",
        "localeId": "65dddce3-df9b-4388-848d-c335be91b332",
        "translationCodeId": "0c50e320-8f49-4543-afca-9ac1efcdfe51",
        "name": "string",
        "customFields": {},
        "locale": {
          "id": null,
          "code": null,
          "name": null,
          "territory": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "languages": null
        },
        "translationCode": {
          "id": null,
          "code": null,
          "name": null,
          "territory": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "languages": null
        },
        "children": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        }
      }
    },
    "lastPaymentMethod": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "pluginId": "91f8cbd0-11f2-4669-9910-90a5a0b7d84a",
      "name": "string",
      "description": "string",
      "position": 0,
      "active": true,
      "afterOrderEnabled": true,
      "customFields": {},
      "availabilityRuleId": "0663b9f4-e343-4d2c-8b2d-d04634bd73f4",
      "mediaId": "5a8ffac5-2288-485d-b463-90c3cd9941ad",
      "translated": {},
      "media": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "alt": "string",
        "title": "string",
        "url": "string",
        "hasFile": true,
        "private": true,
        "customFields": {},
        "translated": {},
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "thumbnails": {
          "id": null,
          "mediaId": null,
          "width": null,
          "height": null,
          "url": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "media": null
        }
      },
      "availabilityRule": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "name": "string",
        "priority": 0,
        "description": "string",
        "customFields": {},
        "moduleTypes": {},
        "conditions": {
          "id": null,
          "type": null,
          "ruleId": null,
          "parentId": null,
          "value": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "rule": null,
          "children": null
        }
      }
    },
    "defaultBillingAddress": {
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
      "customer": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
        "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
        "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
        "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
        "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
        "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
        "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
        "customerNumber": "string",
        "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
        "firstName": "string",
        "lastName": "string",
        "company": "string",
        "email": "string",
        "title": "string",
        "vatIds": [
          "string"
        ],
        "affiliateCode": "string",
        "campaignCode": "string",
        "active": true,
        "doubleOptInRegistration": true,
        "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
        "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
        "hash": "string",
        "guest": true,
        "firstLogin": "2019-08-24T14:15:22Z",
        "lastLogin": "2019-08-24T14:15:22Z",
        "newsletter": true,
        "birthday": "string",
        "customFields": {},
        "remoteAddress": "string",
        "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
        "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
        "group": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "defaultPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "language": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        },
        "lastPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "defaultBillingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "defaultShippingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "salutation": {
          "id": null,
          "salutationKey": null,
          "displayName": null,
          "letterName": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "addresses": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "promotions": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "recoveryCustomer": {
          "id": null,
          "hash": null,
          "customerId": null,
          "createdAt": null,
          "updatedAt": null
        },
        "requestedGroup": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "wishlists": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        }
      },
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
      },
      "salutation": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "salutationKey": "string",
        "displayName": "string",
        "letterName": "string",
        "translated": {}
      }
    },
    "defaultShippingAddress": {
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
      "customer": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
        "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
        "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
        "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
        "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
        "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
        "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
        "customerNumber": "string",
        "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
        "firstName": "string",
        "lastName": "string",
        "company": "string",
        "email": "string",
        "title": "string",
        "vatIds": [
          "string"
        ],
        "affiliateCode": "string",
        "campaignCode": "string",
        "active": true,
        "doubleOptInRegistration": true,
        "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
        "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
        "hash": "string",
        "guest": true,
        "firstLogin": "2019-08-24T14:15:22Z",
        "lastLogin": "2019-08-24T14:15:22Z",
        "newsletter": true,
        "birthday": "string",
        "customFields": {},
        "remoteAddress": "string",
        "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
        "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
        "group": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "defaultPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "language": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        },
        "lastPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "defaultBillingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "defaultShippingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "salutation": {
          "id": null,
          "salutationKey": null,
          "displayName": null,
          "letterName": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "addresses": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "promotions": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "recoveryCustomer": {
          "id": null,
          "hash": null,
          "customerId": null,
          "createdAt": null,
          "updatedAt": null
        },
        "requestedGroup": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "wishlists": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        }
      },
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
      },
      "salutation": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "salutationKey": "string",
        "displayName": "string",
        "letterName": "string",
        "translated": {}
      }
    },
    "salutation": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "salutationKey": "string",
      "displayName": "string",
      "letterName": "string",
      "translated": {}
    },
    "addresses": {
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
      "customer": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "groupId": "eb54e96e-21b8-4f54-9cd4-80fccbd06f55",
        "defaultPaymentMethodId": "10098869-575b-49ae-a0bc-197f04f0018a",
        "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
        "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
        "lastPaymentMethodId": "16e78782-008a-455a-8181-0f62130fc490",
        "defaultBillingAddressId": "eb2384b3-6dee-468b-b9a8-1b94cb37cd8c",
        "defaultShippingAddressId": "b2cbeab7-b855-4dfe-adf6-922299155026",
        "customerNumber": "string",
        "salutationId": "cc59479a-c21a-4158-9032-b9f5abc752f5",
        "firstName": "string",
        "lastName": "string",
        "company": "string",
        "email": "string",
        "title": "string",
        "vatIds": [
          "string"
        ],
        "affiliateCode": "string",
        "campaignCode": "string",
        "active": true,
        "doubleOptInRegistration": true,
        "doubleOptInEmailSentDate": "2019-08-24T14:15:22Z",
        "doubleOptInConfirmDate": "2019-08-24T14:15:22Z",
        "hash": "string",
        "guest": true,
        "firstLogin": "2019-08-24T14:15:22Z",
        "lastLogin": "2019-08-24T14:15:22Z",
        "newsletter": true,
        "birthday": "string",
        "customFields": {},
        "remoteAddress": "string",
        "requestedGroupId": "aef91599-bf26-4df7-b178-f06a9364342f",
        "boundSalesChannelId": "2a1e0981-cfbd-4649-921b-81d2d568935e",
        "group": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "defaultPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "language": {
          "id": null,
          "parentId": null,
          "localeId": null,
          "translationCodeId": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "locale": null,
          "translationCode": null,
          "children": null
        },
        "lastPaymentMethod": {
          "id": null,
          "pluginId": null,
          "name": null,
          "description": null,
          "position": null,
          "active": null,
          "afterOrderEnabled": null,
          "customFields": null,
          "availabilityRuleId": null,
          "mediaId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "availabilityRule": null
        },
        "defaultBillingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "defaultShippingAddress": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "salutation": {
          "id": null,
          "salutationKey": null,
          "displayName": null,
          "letterName": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "addresses": {
          "id": null,
          "customerId": null,
          "countryId": null,
          "countryStateId": null,
          "salutationId": null,
          "firstName": null,
          "lastName": null,
          "zipcode": null,
          "city": null,
          "company": null,
          "street": null,
          "department": null,
          "title": null,
          "vatId": null,
          "phoneNumber": null,
          "additionalAddressLine1": null,
          "additionalAddressLine2": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "customer": null,
          "country": null,
          "countryState": null,
          "salutation": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "promotions": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "recoveryCustomer": {
          "id": null,
          "hash": null,
          "customerId": null,
          "createdAt": null,
          "updatedAt": null
        },
        "requestedGroup": {
          "id": null,
          "name": null,
          "displayGross": null,
          "customFields": null,
          "registrationActive": null,
          "registrationTitle": null,
          "registrationIntroduction": null,
          "registrationOnlyCompanyRegistration": null,
          "registrationSeoMetaDescription": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null
        },
        "wishlists": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        }
      },
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
      },
      "salutation": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "salutationKey": "string",
        "displayName": "string",
        "letterName": "string",
        "translated": {}
      }
    },
    "tags": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string"
    },
    "promotions": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "active": true,
      "validFrom": "2019-08-24T14:15:22Z",
      "validUntil": "2019-08-24T14:15:22Z",
      "maxRedemptionsGlobal": 0,
      "maxRedemptionsPerCustomer": 0,
      "exclusive": true,
      "code": "string",
      "useCodes": true,
      "useIndividualCodes": true,
      "individualCodePattern": "string",
      "useSetGroups": true,
      "customerRestriction": true,
      "exclusionIds": [
        "497f6eca-6276-4993-bfeb-53cbbbba6f08"
      ],
      "translated": {},
      "setgroups": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "promotionId": "3eaf888b-516c-4eac-ac00-1312640986a2",
        "packagerKey": "string",
        "sorterKey": "string",
        "value": 0,
        "promotion": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "setGroupRules": {
          "id": null,
          "name": null,
          "priority": null,
          "description": null,
          "invalid": null,
          "customFields": null,
          "moduleTypes": null,
          "createdAt": null,
          "updatedAt": null,
          "conditions": null
        }
      },
      "discounts": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "promotionId": "3eaf888b-516c-4eac-ac00-1312640986a2",
        "scope": "string",
        "type": "string",
        "value": 0,
        "considerAdvancedRules": true,
        "maxValue": 0,
        "sorterKey": "string",
        "applierKey": "string",
        "usageKey": "string",
        "pickerKey": "string",
        "promotion": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        },
        "discountRules": {
          "id": null,
          "name": null,
          "priority": null,
          "description": null,
          "invalid": null,
          "customFields": null,
          "moduleTypes": null,
          "createdAt": null,
          "updatedAt": null,
          "conditions": null
        },
        "promotionDiscountPrices": {
          "id": null,
          "discountId": null,
          "currencyId": null,
          "price": null,
          "createdAt": null,
          "updatedAt": null,
          "promotionDiscount": null,
          "currency": null
        }
      },
      "individualCodes": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "promotionId": "3eaf888b-516c-4eac-ac00-1312640986a2",
        "code": "string",
        "payload": {},
        "promotion": {
          "id": null,
          "name": null,
          "active": null,
          "validFrom": null,
          "validUntil": null,
          "maxRedemptionsGlobal": null,
          "maxRedemptionsPerCustomer": null,
          "exclusive": null,
          "code": null,
          "useCodes": null,
          "useIndividualCodes": null,
          "individualCodePattern": null,
          "useSetGroups": null,
          "customerRestriction": null,
          "orderCount": null,
          "ordersPerCustomerCount": null,
          "exclusionIds": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "setgroups": null,
          "discounts": null,
          "individualCodes": null
        }
      }
    },
    "productReviews": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "productId": "dcd53ddb-8104-4e48-8cc0-5df1088c6113",
      "productVersionId": "5b05daeb-e87a-4ecb-b86e-5a255751de62",
      "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac",
      "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
      "languageId": "089f4762-7257-4a78-9220-ca730f0b275d",
      "title": "string",
      "content": "string",
      "points": 0,
      "status": true,
      "comment": "string",
      "product": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "versionId": "14707576-2549-4848-82ed-f68f8a1b47c7",
        "parentId": "70850378-7d3c-4f45-91b7-942d4dfbbd43",
        "parentVersionId": "abf80970-9686-419e-bc00-5ddcccc33ba6",
        "manufacturerId": "9ffb4bad-5601-46bd-b5e1-ad29632f5942",
        "productManufacturerVersionId": "5ef9ccce-1f92-4e66-8849-d8c0189982ac",
        "unitId": "b3eb5f92-604a-46b9-9881-9d84000fd7ed",
        "taxId": "ec2f3321-4009-45bd-9423-63aa80044823",
        "coverId": "5fd178bd-f51e-4f24-9612-1857445ad9a8",
        "productMediaVersionId": "3efabe4d-e6f2-4a60-8d52-da6b7965a512",
        "deliveryTimeId": "51e5fd22-fee3-465a-add1-953ad7b5b8a5",
        "productNumber": "string",
        "stock": 0,
        "restockTime": 0,
        "active": true,
        "isCloseout": true,
        "mainVariantId": "a9d54517-b96a-4591-954a-c25556fc138e",
        "manufacturerNumber": "string",
        "ean": "string",
        "purchaseSteps": 0,
        "maxPurchase": 0,
        "minPurchase": 0,
        "purchaseUnit": 0,
        "referenceUnit": 0,
        "shippingFree": true,
        "purchasePrice": 0,
        "markAsTopseller": true,
        "weight": 0,
        "width": 0,
        "height": 0,
        "length": 0,
        "releaseDate": "2019-08-24T14:15:22Z",
        "customFieldSetSelectionActive": true,
        "metaDescription": "string",
        "name": "string",
        "keywords": "string",
        "description": "string",
        "metaTitle": "string",
        "packUnit": "string",
        "packUnitPlural": "string",
        "customFields": {},
        "variation": [
          "string"
        ],
        "featureSetId": "2c884e24-6788-4ec2-9c3d-8b6baa0d5c24",
        "purchasePrices": {},
        "customSearchKeywords": [
          {}
        ],
        "canonicalProductId": "9d6b51f1-2410-4453-85db-e0d2bc76bed8",
        "calculatedPrice": {},
        "calculatedListingPrice": {},
        "calculatedPrices": [
          {}
        ],
        "calculatedMaxPurchase": 0,
        "isNew": true,
        "translated": {},
        "children": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "manufacturerId": null,
          "productManufacturerVersionId": null,
          "unitId": null,
          "taxId": null,
          "coverId": null,
          "productMediaVersionId": null,
          "deliveryTimeId": null,
          "productNumber": null,
          "stock": null,
          "restockTime": null,
          "autoIncrement": null,
          "active": null,
          "availableStock": null,
          "available": null,
          "isCloseout": null,
          "displayGroup": null,
          "mainVariantId": null,
          "manufacturerNumber": null,
          "ean": null,
          "purchaseSteps": null,
          "maxPurchase": null,
          "minPurchase": null,
          "purchaseUnit": null,
          "referenceUnit": null,
          "shippingFree": null,
          "purchasePrice": null,
          "markAsTopseller": null,
          "weight": null,
          "width": null,
          "height": null,
          "length": null,
          "releaseDate": null,
          "ratingAverage": null,
          "categoryTree": null,
          "propertyIds": null,
          "optionIds": null,
          "tagIds": null,
          "childCount": null,
          "customFieldSetSelectionActive": null,
          "sales": null,
          "metaDescription": null,
          "name": null,
          "keywords": null,
          "description": null,
          "metaTitle": null,
          "packUnit": null,
          "packUnitPlural": null,
          "customFields": null,
          "variation": null,
          "featureSetId": null,
          "purchasePrices": null,
          "customSearchKeywords": null,
          "canonicalProductId": null,
          "calculatedPrice": null,
          "calculatedListingPrice": null,
          "calculatedPrices": null,
          "calculatedMaxPurchase": null,
          "isNew": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "deliveryTime": null,
          "tax": null,
          "manufacturer": null,
          "unit": null,
          "cover": null,
          "media": null,
          "crossSellings": null,
          "crossSellingAssignedProducts": null,
          "productReviews": null,
          "mainCategories": null,
          "seoUrls": null,
          "options": null,
          "properties": null,
          "categories": null,
          "categoriesRo": null,
          "tags": null,
          "customFieldSets": null,
          "featureSet": null,
          "wishlists": null,
          "canonicalProduct": null,
          "seoCategory": null
        },
        "deliveryTime": {
          "id": null,
          "name": null,
          "min": null,
          "max": null,
          "unit": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "shippingMethods": null
        },
        "tax": {
          "id": null,
          "taxRate": null,
          "name": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null,
          "shippingMethods": null
        },
        "manufacturer": {
          "id": null,
          "versionId": null,
          "mediaId": null,
          "link": null,
          "name": null,
          "description": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "products": null
        },
        "unit": {
          "id": null,
          "shortCode": null,
          "name": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "products": null
        },
        "cover": {
          "id": null,
          "versionId": null,
          "productId": null,
          "productVersionId": null,
          "mediaId": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "media": null
        },
        "media": {
          "id": null,
          "versionId": null,
          "productId": null,
          "productVersionId": null,
          "mediaId": null,
          "position": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "media": null
        },
        "crossSellings": {
          "id": null,
          "name": null,
          "position": null,
          "sortBy": null,
          "sortDirection": null,
          "type": null,
          "active": null,
          "limit": null,
          "productId": null,
          "productVersionId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "product": null,
          "assignedProducts": null
        },
        "crossSellingAssignedProducts": {
          "id": null,
          "crossSellingId": null,
          "productId": null,
          "productVersionId": null,
          "position": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "crossSelling": null
        },
        "productReviews": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "customerId": null,
          "salesChannelId": null,
          "languageId": null,
          "title": null,
          "content": null,
          "points": null,
          "status": null,
          "comment": null,
          "updatedAt": null,
          "createdAt": null,
          "product": null
        },
        "mainCategories": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "categoryId": null,
          "categoryVersionId": null,
          "salesChannelId": null,
          "createdAt": null,
          "updatedAt": null,
          "product": null,
          "category": null
        },
        "seoUrls": {
          "id": null,
          "salesChannelId": null,
          "languageId": null,
          "foreignKey": null,
          "routeName": null,
          "pathInfo": null,
          "seoPathInfo": null,
          "isCanonical": null,
          "isModified": null,
          "isDeleted": null,
          "url": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "language": null
        },
        "options": {
          "id": null,
          "groupId": null,
          "name": null,
          "position": null,
          "colorHexCode": null,
          "mediaId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "group": null,
          "productConfiguratorSettings": null,
          "productProperties": null,
          "productOptions": null
        },
        "properties": {
          "id": null,
          "groupId": null,
          "name": null,
          "position": null,
          "colorHexCode": null,
          "mediaId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "media": null,
          "group": null,
          "productConfiguratorSettings": null,
          "productProperties": null,
          "productOptions": null
        },
        "categories": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "afterCategoryId": null,
          "afterCategoryVersionId": null,
          "mediaId": null,
          "displayNestedProducts": null,
          "autoIncrement": null,
          "breadcrumb": null,
          "level": null,
          "path": null,
          "childCount": null,
          "type": null,
          "productAssignmentType": null,
          "visible": null,
          "active": null,
          "name": null,
          "customFields": null,
          "slotConfig": null,
          "externalLink": null,
          "description": null,
          "metaTitle": null,
          "metaDescription": null,
          "keywords": null,
          "cmsPageId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "media": null,
          "products": null,
          "nestedProducts": null,
          "tags": null,
          "cmsPage": null,
          "productStream": null,
          "mainCategories": null,
          "seoUrls": null
        },
        "categoriesRo": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "afterCategoryId": null,
          "afterCategoryVersionId": null,
          "mediaId": null,
          "displayNestedProducts": null,
          "autoIncrement": null,
          "breadcrumb": null,
          "level": null,
          "path": null,
          "childCount": null,
          "type": null,
          "productAssignmentType": null,
          "visible": null,
          "active": null,
          "name": null,
          "customFields": null,
          "slotConfig": null,
          "externalLink": null,
          "description": null,
          "metaTitle": null,
          "metaDescription": null,
          "keywords": null,
          "cmsPageId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "media": null,
          "products": null,
          "nestedProducts": null,
          "tags": null,
          "cmsPage": null,
          "productStream": null,
          "mainCategories": null,
          "seoUrls": null
        },
        "tags": {
          "id": null,
          "name": null,
          "createdAt": null,
          "updatedAt": null
        },
        "customFieldSets": {
          "id": null,
          "name": null,
          "config": null,
          "active": null,
          "global": null,
          "position": null,
          "appId": null,
          "createdAt": null,
          "updatedAt": null,
          "customFields": null,
          "relations": null,
          "products": null,
          "app": null
        },
        "featureSet": {
          "id": null,
          "name": null,
          "description": null,
          "features": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "products": null
        },
        "wishlists": {
          "id": null,
          "productId": null,
          "productVersionId": null,
          "wishlistId": null,
          "createdAt": null,
          "updatedAt": null,
          "wishlist": null,
          "product": null
        },
        "canonicalProduct": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "manufacturerId": null,
          "productManufacturerVersionId": null,
          "unitId": null,
          "taxId": null,
          "coverId": null,
          "productMediaVersionId": null,
          "deliveryTimeId": null,
          "productNumber": null,
          "stock": null,
          "restockTime": null,
          "autoIncrement": null,
          "active": null,
          "availableStock": null,
          "available": null,
          "isCloseout": null,
          "displayGroup": null,
          "mainVariantId": null,
          "manufacturerNumber": null,
          "ean": null,
          "purchaseSteps": null,
          "maxPurchase": null,
          "minPurchase": null,
          "purchaseUnit": null,
          "referenceUnit": null,
          "shippingFree": null,
          "purchasePrice": null,
          "markAsTopseller": null,
          "weight": null,
          "width": null,
          "height": null,
          "length": null,
          "releaseDate": null,
          "ratingAverage": null,
          "categoryTree": null,
          "propertyIds": null,
          "optionIds": null,
          "tagIds": null,
          "childCount": null,
          "customFieldSetSelectionActive": null,
          "sales": null,
          "metaDescription": null,
          "name": null,
          "keywords": null,
          "description": null,
          "metaTitle": null,
          "packUnit": null,
          "packUnitPlural": null,
          "customFields": null,
          "variation": null,
          "featureSetId": null,
          "purchasePrices": null,
          "customSearchKeywords": null,
          "canonicalProductId": null,
          "calculatedPrice": null,
          "calculatedListingPrice": null,
          "calculatedPrices": null,
          "calculatedMaxPurchase": null,
          "isNew": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "deliveryTime": null,
          "tax": null,
          "manufacturer": null,
          "unit": null,
          "cover": null,
          "media": null,
          "crossSellings": null,
          "crossSellingAssignedProducts": null,
          "productReviews": null,
          "mainCategories": null,
          "seoUrls": null,
          "options": null,
          "properties": null,
          "categories": null,
          "categoriesRo": null,
          "tags": null,
          "customFieldSets": null,
          "featureSet": null,
          "wishlists": null,
          "canonicalProduct": null,
          "seoCategory": null
        },
        "seoCategory": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "afterCategoryId": null,
          "afterCategoryVersionId": null,
          "mediaId": null,
          "displayNestedProducts": null,
          "autoIncrement": null,
          "breadcrumb": null,
          "level": null,
          "path": null,
          "childCount": null,
          "type": null,
          "productAssignmentType": null,
          "visible": null,
          "active": null,
          "name": null,
          "customFields": null,
          "slotConfig": null,
          "externalLink": null,
          "description": null,
          "metaTitle": null,
          "metaDescription": null,
          "keywords": null,
          "cmsPageId": null,
          "productStreamId": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "media": null,
          "products": null,
          "nestedProducts": null,
          "tags": null,
          "cmsPage": null,
          "productStream": null,
          "mainCategories": null,
          "seoUrls": null
        }
      }
    },
    "recoveryCustomer": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "hash": "string",
      "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac"
    },
    "requestedGroup": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "name": "string",
      "displayGross": true,
      "customFields": {},
      "registrationActive": true,
      "registrationTitle": "string",
      "registrationIntroduction": "string",
      "registrationOnlyCompanyRegistration": true,
      "registrationSeoMetaDescription": "string",
      "translated": {}
    },
    "wishlists": {
      "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
      "customerId": "87d8e330-2878-4742-a86f-dbbb3bf522ac",
      "salesChannelId": "4f66738e-5c3d-4e55-b112-356b1676e152",
      "customFields": {},
      "products": {
        "id": "497f6eca-6276-4993-bfeb-53cbbbba6f08",
        "productId": "dcd53ddb-8104-4e48-8cc0-5df1088c6113",
        "productVersionId": "5b05daeb-e87a-4ecb-b86e-5a255751de62",
        "wishlistId": "cbe1353c-385f-4d1b-807a-83768b4af636",
        "wishlist": {
          "id": null,
          "customerId": null,
          "salesChannelId": null,
          "customFields": null,
          "createdAt": null,
          "updatedAt": null,
          "products": null
        },
        "product": {
          "id": null,
          "versionId": null,
          "parentId": null,
          "parentVersionId": null,
          "manufacturerId": null,
          "productManufacturerVersionId": null,
          "unitId": null,
          "taxId": null,
          "coverId": null,
          "productMediaVersionId": null,
          "deliveryTimeId": null,
          "productNumber": null,
          "stock": null,
          "restockTime": null,
          "autoIncrement": null,
          "active": null,
          "availableStock": null,
          "available": null,
          "isCloseout": null,
          "displayGroup": null,
          "mainVariantId": null,
          "manufacturerNumber": null,
          "ean": null,
          "purchaseSteps": null,
          "maxPurchase": null,
          "minPurchase": null,
          "purchaseUnit": null,
          "referenceUnit": null,
          "shippingFree": null,
          "purchasePrice": null,
          "markAsTopseller": null,
          "weight": null,
          "width": null,
          "height": null,
          "length": null,
          "releaseDate": null,
          "ratingAverage": null,
          "categoryTree": null,
          "propertyIds": null,
          "optionIds": null,
          "tagIds": null,
          "childCount": null,
          "customFieldSetSelectionActive": null,
          "sales": null,
          "metaDescription": null,
          "name": null,
          "keywords": null,
          "description": null,
          "metaTitle": null,
          "packUnit": null,
          "packUnitPlural": null,
          "customFields": null,
          "variation": null,
          "featureSetId": null,
          "purchasePrices": null,
          "customSearchKeywords": null,
          "canonicalProductId": null,
          "calculatedPrice": null,
          "calculatedListingPrice": null,
          "calculatedPrices": null,
          "calculatedMaxPurchase": null,
          "isNew": null,
          "createdAt": null,
          "updatedAt": null,
          "translated": null,
          "children": null,
          "deliveryTime": null,
          "tax": null,
          "manufacturer": null,
          "unit": null,
          "cover": null,
          "media": null,
          "crossSellings": null,
          "crossSellingAssignedProducts": null,
          "productReviews": null,
          "mainCategories": null,
          "seoUrls": null,
          "options": null,
          "properties": null,
          "categories": null,
          "categoriesRo": null,
          "tags": null,
          "customFieldSets": null,
          "featureSet": null,
          "wishlists": null,
          "canonicalProduct": null,
          "seoCategory": null
        }
      }
    }
  },
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
