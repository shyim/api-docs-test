
# user_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|localeId|string(uuid)|true|none|none|
|avatarId|string(uuid)|false|none|none|
|username|string|true|none|none|
|firstName|string|true|none|none|
|lastName|string|true|none|none|
|title|string|false|none|none|
|email|string|true|none|none|
|active|boolean|false|none|none|
|admin|boolean|false|none|none|
|lastUpdatedPasswordAt|string(date-time)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|locale|[locale_flat](/schema/locale_flat.md)|false|none|Added since version: 6.0.0.0|
|avatarMedia|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|media|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|accessKeys|[user_access_key_flat](/schema/user_access_key_flat.md)|false|none|Added since version: 6.0.0.0|
|configs|[user_config_flat](/schema/user_config_flat.md)|false|none|Added since version: 6.3.5.0|
|stateMachineHistoryEntries|[state_machine_history_flat](/schema/state_machine_history_flat.md)|false|none|Added since version: 6.0.0.0|
|importExportLogEntries|[import_export_log_flat](/schema/import_export_log_flat.md)|false|none|Added since version: 6.0.0.0|
|createdOrders|[order_flat](/schema/order_flat.md)|false|none|Added since version: 6.0.0.0|
|updatedOrders|[order_flat](/schema/order_flat.md)|false|none|Added since version: 6.0.0.0|
