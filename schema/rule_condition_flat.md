
# rule_condition_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|type|string|false|none|none|
|ruleId|string(uuid)|true|none|none|
|parentId|string(uuid)|false|none|none|
|value|object|false|none|none|
|position|integer(int64)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|rule|[rule_flat](/schema/rule_flat)|false|none|Added since version: 6.0.0.0|
|children|[rule_condition_flat](/schema/rule_condition_flat)|false|none|Added since version: 6.0.0.0|
