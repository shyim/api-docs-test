
# custom_field_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|type|string|true|none|none|
|config|object|false|none|none|
|active|boolean|false|none|none|
|customFieldSetId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|customFieldSet|[custom_field_set_flat](/schema/custom_field_set_flat)|false|none|Added since version: 6.0.0.0|
