
# sales_channel_type_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|coverUrl|string|false|none|none|
|iconName|string|false|none|none|
|screenshotUrls|[string]|false|none|none|
|name|string|true|none|none|
|manufacturer|string|false|none|none|
|description|string|false|none|none|
|descriptionLong|string|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|salesChannels|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
