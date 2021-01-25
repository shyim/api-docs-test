
# product_stream_filter_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|productStreamId|string(uuid)|true|none|none|
|parentId|string(uuid)|false|none|none|
|type|string|true|none|none|
|field|string|false|none|none|
|operator|string|false|none|none|
|value|string|false|none|none|
|parameters|object|false|none|none|
|position|integer(int64)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|productStream|[product_stream_flat](/schema/product_stream_flat.md)|false|none|Added since version: 6.0.0.0|
|queries|[product_stream_filter_flat](/schema/product_stream_filter_flat.md)|false|none|Added since version: 6.0.0.0|
