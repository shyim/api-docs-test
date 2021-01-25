
# integration_role_flat

{% hint style="info" %}

Added since version: 6.3.3.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|integrationId|string(uuid)|true|none|none|
|aclRoleId|string(uuid)|true|none|none|
|integration|[integration_flat](/schema/integration_flat.md)|false|none|Added since version: 6.0.0.0|
|role|[acl_role_flat](/schema/acl_role_flat.md)|false|none|Added since version: 6.0.0.0|
