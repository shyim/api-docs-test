
# sales_channel_analytics_flat

{% hint style="info" %}

Added since version: 6.2.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|trackingId|string|false|none|none|
|active|boolean|false|none|none|
|trackOrders|boolean|false|none|none|
|anonymizeIp|boolean|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
