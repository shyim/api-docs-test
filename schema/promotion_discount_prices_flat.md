
# promotion_discount_prices_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|discountId|string(uuid)|true|none|none|
|currencyId|string(uuid)|true|none|none|
|price|number(float)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|promotionDiscount|[promotion_discount_flat](/schema/promotion_discount_flat)|false|none|Added since version: 6.0.0.0|
|currency|[currency_flat](/schema/currency_flat)|false|none|Added since version: 6.0.0.0|
