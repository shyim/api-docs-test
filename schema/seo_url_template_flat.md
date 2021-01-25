
# seo_url_template_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|salesChannelId|string(uuid)|false|none|none|
|entityName|string|true|none|none|
|routeName|string|true|none|none|
|template|string|false|none|none|
|isValid|boolean|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
