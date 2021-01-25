
# product_property_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|optionId|string(uuid)|true|none|none|
|product|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
|option|[property_group_option_flat](/schema/property_group_option_flat.md)|false|none|Added since version: 6.0.0.0|
