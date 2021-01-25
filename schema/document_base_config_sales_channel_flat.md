
# document_base_config_sales_channel_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|documentBaseConfigId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|false|none|none|
|documentTypeId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|documentType|[document_type_flat](/schema/document_type_flat.md)|false|none|Added since version: 6.0.0.0|
|documentBaseConfig|[document_base_config_flat](/schema/document_base_config_flat.md)|false|none|Added since version: 6.0.0.0|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
