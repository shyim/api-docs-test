
# import_export_log_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|activity|string|true|none|none|
|state|string|true|none|none|
|records|integer(int64)|true|none|none|
|userId|string(uuid)|false|none|none|
|profileId|string(uuid)|false|none|none|
|fileId|string(uuid)|false|none|none|
|invalidRecordsLogId|string(uuid)|false|none|none|
|username|string|false|none|none|
|profileName|string|false|none|none|
|config|object|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|profile|[import_export_profile_flat](/schema/import_export_profile_flat.md)|false|none|Added since version: 6.0.0.0|
|file|[import_export_file_flat](/schema/import_export_file_flat.md)|false|none|Added since version: 6.0.0.0|
|invalidRecordsLog|[import_export_log_flat](/schema/import_export_log_flat.md)|false|none|Added since version: 6.0.0.0|
|failedImportLog|[import_export_log_flat](/schema/import_export_log_flat.md)|false|none|Added since version: 6.0.0.0|
