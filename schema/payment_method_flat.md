
# payment_method_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|pluginId|string(uuid)|false|none|none|
|name|string|true|none|none|
|description|string|false|none|none|
|position|integer(int64)|false|none|none|
|active|boolean|false|none|none|
|afterOrderEnabled|boolean|false|none|none|
|customFields|object|false|none|none|
|availabilityRuleId|string(uuid)|false|none|none|
|mediaId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|media|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|availabilityRule|[rule_flat](/schema/rule_flat.md)|false|none|Added since version: 6.0.0.0|
