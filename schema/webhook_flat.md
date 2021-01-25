
# webhook_flat

{% hint style="info" %}

Added since version: 6.3.1.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|eventName|string|true|none|none|
|url|string|true|none|none|
|appId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|app|[app_flat](/schema/app_flat)|false|none|Added since version: 6.3.1.0|
