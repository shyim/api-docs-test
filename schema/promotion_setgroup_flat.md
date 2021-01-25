
# promotion_setgroup_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|promotionId|string(uuid)|true|none|none|
|packagerKey|string|true|none|none|
|sorterKey|string|true|none|none|
|value|number(float)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|promotion|[promotion_flat](/schema/promotion_flat)|false|none|Added since version: 6.0.0.0|
|setGroupRules|[rule_flat](/schema/rule_flat)|false|none|Added since version: 6.0.0.0|
