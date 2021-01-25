
# main_category_flat

{% hint style="info" %}

Added since version: 6.1.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|categoryId|string(uuid)|true|none|none|
|categoryVersionId|string(uuid)|false|none|none|
|salesChannelId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|product|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|category|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
