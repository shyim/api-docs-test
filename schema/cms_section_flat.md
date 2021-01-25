
# cms_section_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|position|integer(int64)|true|none|none|
|type|string|true|none|none|
|locked|boolean|false|none|none|
|name|string|false|none|none|
|sizingMode|string|false|none|none|
|mobileBehavior|string|false|none|none|
|backgroundColor|string|false|none|none|
|backgroundMediaId|string(uuid)|false|none|none|
|backgroundMediaMode|string|false|none|none|
|cssClass|string|false|none|none|
|pageId|string(uuid)|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|page|[cms_page_flat](/schema/cms_page_flat.md)|false|none|Added since version: 6.0.0.0|
|backgroundMedia|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|blocks|[cms_block_flat](/schema/cms_block_flat.md)|false|none|Added since version: 6.0.0.0|
