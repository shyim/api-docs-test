
# import_export_profile_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|false|none|none|
|label|string|true|none|none|
|systemDefault|boolean|false|none|none|
|sourceEntity|string|true|none|none|
|fileType|string|true|none|none|
|delimiter|string|true|none|none|
|enclosure|string|true|none|none|
|mapping|object|false|none|none|
|config|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|importExportLogs|[import_export_log_flat](/schema/import_export_log_flat.md)|false|none|Added since version: 6.0.0.0|
