
# rule_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|priority|integer(int64)|true|none|none|
|description|string|false|none|none|
|invalid|boolean|false|read-only|none|
|customFields|object|false|none|none|
|moduleTypes|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|conditions|[rule_condition_flat](/schema/rule_condition_flat.md)|false|none|Added since version: 6.0.0.0|
