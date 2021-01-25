
# order_customer_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|customerId|string(uuid)|false|none|none|
|orderId|string(uuid)|true|none|none|
|orderVersionId|string(uuid)|false|none|none|
|email|string|true|none|none|
|salutationId|string(uuid)|true|none|none|
|firstName|string|true|none|none|
|lastName|string|true|none|none|
|company|string|false|none|none|
|title|string|false|none|none|
|customerNumber|string|false|none|none|
|customFields|object|false|none|none|
|remoteAddress|string|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|order|[order_flat](/schema/order_flat)|false|none|Added since version: 6.0.0.0|
|salutation|[salutation_flat](/schema/salutation_flat)|false|none|Added since version: 6.0.0.0|
