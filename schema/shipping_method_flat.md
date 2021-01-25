
# shipping_method_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|active|boolean|false|none|none|
|customFields|object|false|none|none|
|availabilityRuleId|string(uuid)|true|none|none|
|mediaId|string(uuid)|false|none|none|
|deliveryTimeId|string(uuid)|true|none|none|
|taxType|string|true|none|none|
|taxId|string(uuid)|false|none|none|
|description|string|false|none|none|
|trackingUrl|string|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|deliveryTime|[delivery_time_flat](/schema/delivery_time_flat)|false|none|Added since version: 6.0.0.0|
|availabilityRule|[rule_flat](/schema/rule_flat)|false|none|Added since version: 6.0.0.0|
|prices|[shipping_method_price_flat](/schema/shipping_method_price_flat)|false|none|Added since version: 6.0.0.0|
|media|[media_flat](/schema/media_flat)|false|none|Added since version: 6.0.0.0|
|tags|[tag_flat](/schema/tag_flat)|false|none|Added since version: 6.0.0.0|
|tax|[tax_flat](/schema/tax_flat)|false|none|Added since version: 6.0.0.0|
