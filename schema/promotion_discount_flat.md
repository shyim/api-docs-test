
# promotion_discount_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|promotionId|string(uuid)|true|none|none|
|scope|string|true|none|none|
|type|string|true|none|none|
|value|number(float)|true|none|none|
|considerAdvancedRules|boolean|true|none|none|
|maxValue|number(float)|false|none|none|
|sorterKey|string|false|none|none|
|applierKey|string|false|none|none|
|usageKey|string|false|none|none|
|pickerKey|string|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|promotion|[promotion_flat](/schema/promotion_flat.md)|false|none|Added since version: 6.0.0.0|
|discountRules|[rule_flat](/schema/rule_flat.md)|false|none|Added since version: 6.0.0.0|
|promotionDiscountPrices|[promotion_discount_prices_flat](/schema/promotion_discount_prices_flat.md)|false|none|Added since version: 6.0.0.0|
