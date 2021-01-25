
# app_flat

{% hint style="info" %}

Added since version: 6.3.1.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|path|string|true|none|none|
|author|string|false|none|none|
|copyright|string|false|none|none|
|license|string|false|none|none|
|active|boolean|true|none|none|
|configurable|boolean|true|none|none|
|privacy|string|false|none|none|
|version|string|true|none|none|
|icon|string|false|read-only|none|
|modules|[object]|false|none|none|
|cookies|[object]|false|none|none|
|label|string|true|none|none|
|description|string|false|none|none|
|privacyPolicyExtensions|string|false|none|none|
|integrationId|string(uuid)|true|none|none|
|aclRoleId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|integration|[integration_flat](/schema/integration_flat)|false|none|Added since version: 6.0.0.0|
|aclRole|[acl_role_flat](/schema/acl_role_flat)|false|none|Added since version: 6.0.0.0|
|customFieldSets|[custom_field_set_flat](/schema/custom_field_set_flat)|false|none|Added since version: 6.0.0.0|
|actionButtons|[app_action_button_flat](/schema/app_action_button_flat)|false|none|Added since version: 6.3.1.0|
|templates|[app_template_flat](/schema/app_template_flat)|false|none|Added since version: 6.3.1.0|
|webhooks|[webhook_flat](/schema/webhook_flat)|false|none|Added since version: 6.3.1.0|
