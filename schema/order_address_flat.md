
# order_address_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|countryId|string(uuid)|true|none|none|
|countryStateId|string(uuid)|false|none|none|
|orderId|string(uuid)|true|none|none|
|orderVersionId|string(uuid)|false|none|none|
|salutationId|string(uuid)|true|none|none|
|firstName|string|true|none|none|
|lastName|string|true|none|none|
|street|string|true|none|none|
|zipcode|string|true|none|none|
|city|string|true|none|none|
|company|string|false|none|none|
|department|string|false|none|none|
|title|string|false|none|none|
|vatId|string|false|none|none|
|phoneNumber|string|false|none|none|
|additionalAddressLine1|string|false|none|none|
|additionalAddressLine2|string|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|country|[country_flat](/schema/country_flat.md)|false|none|Added since version: 6.0.0.0|
|countryState|[country_state_flat](/schema/country_state_flat.md)|false|none|Added since version: 6.0.0.0|
|order|[order_flat](/schema/order_flat.md)|false|none|Added since version: 6.0.0.0|
|orderDeliveries|[order_delivery_flat](/schema/order_delivery_flat.md)|false|none|Added since version: 6.0.0.0|
|salutation|[salutation_flat](/schema/salutation_flat.md)|false|none|Added since version: 6.0.0.0|
