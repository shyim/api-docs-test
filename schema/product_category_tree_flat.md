
# product_category_tree_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|categoryId|string(uuid)|true|none|none|
|categoryVersionId|string(uuid)|false|none|none|
|product|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
|category|[category_flat](/schema/category_flat.md)|false|none|Added since version: 6.0.0.0|
