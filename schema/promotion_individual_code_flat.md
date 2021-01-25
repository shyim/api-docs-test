
# promotion_individual_code_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|promotionId|string(uuid)|true|none|none|
|code|string|true|none|none|
|payload|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|promotion|[promotion_flat](/schema/promotion_flat.md)|false|none|Added since version: 6.0.0.0|
