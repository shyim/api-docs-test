
# shipping_method_price_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|shippingMethodId|string(uuid)|true|none|none|
|ruleId|string(uuid)|false|none|none|
|calculation|integer(int64)|false|none|none|
|calculationRuleId|string(uuid)|false|none|none|
|quantityStart|number(float)|false|none|none|
|quantityEnd|number(float)|false|none|none|
|currencyPrice|object|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|shippingMethod|[shipping_method_flat](/schema/shipping_method_flat.md)|false|none|Added since version: 6.0.0.0|
|rule|[rule_flat](/schema/rule_flat.md)|false|none|Added since version: 6.0.0.0|
|calculationRule|[rule_flat](/schema/rule_flat.md)|false|none|Added since version: 6.0.0.0|
