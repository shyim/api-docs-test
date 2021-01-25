
# theme_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|technicalName|string|false|none|none|
|name|string|true|none|none|
|author|string|true|none|none|
|description|string|false|none|none|
|labels|object|false|none|none|
|helpTexts|object|false|none|none|
|customFields|object|false|none|none|
|previewMediaId|string(uuid)|false|none|none|
|parentThemeId|string(uuid)|false|none|none|
|baseConfig|object|false|none|none|
|configValues|object|false|none|none|
|active|boolean|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|salesChannels|[sales_channel_flat](/schema/sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
|media|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|previewMedia|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|childThemes|[theme_flat](/schema/theme_flat.md)|false|none|Added since version: 6.0.0.0|
