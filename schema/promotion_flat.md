
# promotion_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|active|boolean|true|none|none|
|validFrom|string(date-time)|false|none|none|
|validUntil|string(date-time)|false|none|none|
|maxRedemptionsGlobal|integer(int64)|false|none|none|
|maxRedemptionsPerCustomer|integer(int64)|false|none|none|
|exclusive|boolean|true|none|none|
|code|string|false|none|none|
|useCodes|boolean|true|none|none|
|useIndividualCodes|boolean|true|none|none|
|individualCodePattern|string|false|none|none|
|useSetGroups|boolean|true|none|none|
|customerRestriction|boolean|false|none|none|
|orderCount|integer(int64)|false|read-only|none|
|ordersPerCustomerCount|object|false|read-only|none|
|exclusionIds|[string]|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|setgroups|[promotion_setgroup_flat](/schema/promotion_setgroup_flat)|false|none|Added since version: 6.0.0.0|
|discounts|[promotion_discount_flat](/schema/promotion_discount_flat)|false|none|Added since version: 6.0.0.0|
|individualCodes|[promotion_individual_code_flat](/schema/promotion_individual_code_flat)|false|none|Added since version: 6.0.0.0|
