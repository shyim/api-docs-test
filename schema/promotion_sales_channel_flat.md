
# promotion_sales_channel_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|promotionId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|priority|integer(int64)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|promotion|[promotion_flat](/schema/promotion_flat.md)|false|none|Added since version: 6.0.0.0|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
