
# delivery_time_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|min|integer(int64)|true|none|none|
|max|integer(int64)|true|none|none|
|unit|string|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|shippingMethods|[shipping_method_flat](/schema/shipping_method_flat)|false|none|Added since version: 6.0.0.0|
