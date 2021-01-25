
# acl_role_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|name|string|true|none|none|
|description|string|false|none|none|
|privileges|[any]|true|none|none|
|app|[app_flat](/schema/app_flat.md)|false|none|Added since version: 6.3.1.0|
|integrations|[integration_flat](/schema/integration_flat.md)|false|none|Added since version: 6.0.0.0|
