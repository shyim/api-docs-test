
# integration_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|label|string|true|none|none|
|accessKey|string|true|none|none|
|secretAccessKey|string|true|none|none|
|writeAccess|boolean|false|none|none|
|lastUsageAt|string(date-time)|false|none|none|
|admin|boolean|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|app|[app_flat](/schema/app_flat.md)|false|none|Added since version: 6.3.1.0|
|aclRoles|[acl_role_flat](/schema/acl_role_flat.md)|false|none|Added since version: 6.0.0.0|
