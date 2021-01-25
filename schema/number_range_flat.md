
# number_range_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|typeId|string(uuid)|true|none|none|
|global|boolean|true|none|none|
|name|string|true|none|none|
|description|string|false|none|none|
|pattern|string|true|none|none|
|start|integer(int64)|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|type|[number_range_type_flat](/schema/number_range_type_flat)|false|none|Added since version: 6.0.0.0|
|numberRangeSalesChannels|[number_range_sales_channel_flat](/schema/number_range_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|state|[number_range_state_flat](/schema/number_range_state_flat)|false|none|Added since version: 6.0.0.0|
