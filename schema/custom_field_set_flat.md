
# custom_field_set_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|config|object|false|none|none|
|active|boolean|false|none|none|
|global|boolean|false|none|none|
|position|integer(int64)|false|none|none|
|appId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|customFields|[custom_field_flat](/schema/custom_field_flat)|false|none|Added since version: 6.0.0.0|
|relations|[custom_field_set_relation_flat](/schema/custom_field_set_relation_flat)|false|none|Added since version: 6.0.0.0|
|products|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|app|[app_flat](/schema/app_flat)|false|none|Added since version: 6.3.1.0|
