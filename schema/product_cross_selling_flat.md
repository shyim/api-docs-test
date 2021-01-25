
# product_cross_selling_flat

{% hint style="info" %}

Added since version: 6.1.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|position|integer(int64)|true|none|none|
|sortBy|string|false|none|none|
|sortDirection|string|false|none|none|
|type|string|true|none|none|
|active|boolean|false|none|none|
|limit|integer(int64)|false|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|productStreamId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|product|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|assignedProducts|[product_cross_selling_assigned_products_flat](/schema/product_cross_selling_assigned_products_flat)|false|none|Added since version: 6.2.0.0|
