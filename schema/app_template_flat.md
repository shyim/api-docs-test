
# app_template_flat

{% hint style="info" %}

Added since version: 6.3.1.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|template|string|true|none|none|
|path|string|true|none|none|
|active|boolean|true|none|none|
|appId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|app|[app_flat](/schema/app_flat.md)|false|none|Added since version: 6.3.1.0|
