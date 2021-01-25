
# import_export_file_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|originalName|string|true|none|none|
|path|string|true|none|none|
|expireDate|string(date-time)|true|none|none|
|size|integer(int64)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|accessToken|string|true|none|none|
|updatedAt|string(date-time)|false|read-only|none|
|log|[import_export_log_flat](/schema/import_export_log_flat)|false|none|Added since version: 6.0.0.0|
