
# number_range_type_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|technicalName|string|false|none|none|
|typeName|string|true|none|none|
|global|boolean|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|numberRanges|[number_range_flat](/schema/number_range_flat.md)|false|none|Added since version: 6.0.0.0|
|numberRangeSalesChannels|[number_range_sales_channel_flat](/schema/number_range_sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
