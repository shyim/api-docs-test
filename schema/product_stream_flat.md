
# product_stream_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|apiFilter|object|false|read-only|none|
|invalid|boolean|false|read-only|none|
|name|string|true|none|none|
|description|string|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|filters|[product_stream_filter_flat](/schema/product_stream_filter_flat.md)|false|none|Added since version: 6.0.0.0|
|productCrossSellings|[product_cross_selling_flat](/schema/product_cross_selling_flat.md)|false|none|Added since version: 6.1.0.0|
|productExports|[product_export_flat](/schema/product_export_flat.md)|false|none|Added since version: 6.1.0.0|
|categories|[category_flat](/schema/category_flat.md)|false|none|Added since version: 6.0.0.0|
