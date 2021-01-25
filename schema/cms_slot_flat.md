
# cms_slot_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|type|string|true|none|none|
|slot|string|true|none|none|
|locked|boolean|false|none|none|
|config|object|false|none|none|
|customFields|object|false|none|none|
|data|object|false|read-only|none|
|blockId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|block|[cms_block_flat](/schema/cms_block_flat.md)|false|none|Added since version: 6.0.0.0|
