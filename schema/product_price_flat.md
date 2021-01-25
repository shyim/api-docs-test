
# product_price_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|ruleId|string(uuid)|true|none|none|
|price|object|true|none|none|
|quantityStart|integer(int64)|true|none|none|
|quantityEnd|integer(int64)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|product|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
