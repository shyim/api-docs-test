
# cms_page_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|type|string|true|none|none|
|entity|string|false|none|none|
|config|object|false|none|none|
|» backgroundColor|string|false|none|none|
|previewMediaId|string(uuid)|false|none|none|
|customFields|object|false|none|none|
|locked|boolean|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|sections|[cms_section_flat](/schema/cms_section_flat)|false|none|Added since version: 6.0.0.0|
|previewMedia|[media_flat](/schema/media_flat)|false|none|Added since version: 6.0.0.0|
|categories|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
