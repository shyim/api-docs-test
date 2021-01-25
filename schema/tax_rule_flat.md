
# tax_rule_flat

{% hint style="info" %}

Added since version: 6.1.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|taxRuleTypeId|string(uuid)|true|none|none|
|countryId|string(uuid)|true|none|none|
|taxRate|number(float)|true|none|none|
|data|object|false|none|none|
|» states|[any]|false|none|none|
|» zipCode|string|false|none|none|
|» fromZipCode|string|false|none|none|
|» toZipCode|string|false|none|none|
|taxId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|type|[tax_rule_type_flat](/schema/tax_rule_type_flat)|false|none|Added since version: 6.1.0.0|
|country|[country_flat](/schema/country_flat)|false|none|Added since version: 6.0.0.0|
|tax|[tax_flat](/schema/tax_flat)|false|none|Added since version: 6.0.0.0|
