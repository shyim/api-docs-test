
# document_type_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|technicalName|string|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|customFields|object|false|none|none|
|translated|object|false|none|none|
|documents|[document_flat](/schema/document_flat)|false|none|Added since version: 6.0.0.0|
|documentBaseConfigs|[document_base_config_flat](/schema/document_base_config_flat)|false|none|Added since version: 6.0.0.0|
|documentBaseConfigSalesChannels|[document_base_config_sales_channel_flat](/schema/document_base_config_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
