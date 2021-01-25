
# tax_rule_type_flat

{% hint style="info" %}

Added since version: 6.1.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|technicalName|string|true|read-only|none|
|position|integer(int64)|true|none|none|
|typeName|string|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|rules|[tax_rule_flat](/schema/tax_rule_flat)|false|none|Added since version: 6.1.0.0|
