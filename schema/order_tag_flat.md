
# order_tag_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|orderId|string(uuid)|true|none|none|
|orderVersionId|string(uuid)|false|none|none|
|tagId|string(uuid)|true|none|none|
|order|[order_flat](/schema/order_flat)|false|none|Added since version: 6.0.0.0|
|tag|[tag_flat](/schema/tag_flat)|false|none|Added since version: 6.0.0.0|
