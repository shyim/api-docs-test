
# document_base_config_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|documentTypeId|string(uuid)|true|none|none|
|logoId|string(uuid)|false|none|none|
|name|string|true|none|none|
|filenamePrefix|string|false|none|none|
|filenameSuffix|string|false|none|none|
|global|boolean|true|none|none|
|documentNumber|string|false|none|none|
|config|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|documentType|[document_type_flat](/schema/document_type_flat)|false|none|Added since version: 6.0.0.0|
|logo|[media_flat](/schema/media_flat)|false|none|Added since version: 6.0.0.0|
|salesChannels|[document_base_config_sales_channel_flat](/schema/document_base_config_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
