
# product_review_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|customerId|string(uuid)|false|none|none|
|salesChannelId|string(uuid)|true|none|none|
|languageId|string(uuid)|true|none|none|
|title|string|true|none|none|
|content|string|true|none|none|
|points|number(float)|false|none|none|
|status|boolean|false|none|none|
|comment|string|false|none|none|
|updatedAt|string(date-time)|false|read-only|none|
|createdAt|string(date-time)|true|read-only|none|
|product|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
