
# number_range_sales_channel_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|numberRangeId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|numberRangeTypeId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|numberRange|[number_range_flat](/schema/number_range_flat.md)|false|none|Added since version: 6.0.0.0|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
|numberRangeType|[number_range_type_flat](/schema/number_range_type_flat.md)|false|none|Added since version: 6.0.0.0|
