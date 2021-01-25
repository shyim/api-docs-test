
# product_cross_selling_assigned_products_flat

{% hint style="info" %}

Added since version: 6.2.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|crossSellingId|string(uuid)|true|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|position|integer(int64)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|product|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|crossSelling|[product_cross_selling_flat](/schema/product_cross_selling_flat)|false|none|Added since version: 6.1.0.0|
