
# property_group_option_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|groupId|string(uuid)|true|none|none|
|name|string|true|none|none|
|position|integer(int64)|false|none|none|
|colorHexCode|string|false|none|none|
|mediaId|string(uuid)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|media|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|group|[property_group_flat](/schema/property_group_flat.md)|false|none|Added since version: 6.0.0.0|
|productConfiguratorSettings|[product_configurator_setting_flat](/schema/product_configurator_setting_flat.md)|false|none|Added since version: 6.0.0.0|
|productProperties|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
|productOptions|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
