
# product_configurator_setting_flat

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
|mediaId|string(uuid)|false|none|none|
|optionId|string(uuid)|true|none|none|
|price|object|false|none|none|
|position|integer(int64)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|product|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|media|[media_flat](/schema/media_flat)|false|none|Added since version: 6.0.0.0|
|option|[property_group_option_flat](/schema/property_group_option_flat)|false|none|Added since version: 6.0.0.0|
