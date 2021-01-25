
# customer_wishlist_product_flat

{% hint style="info" %}

Added since version: 6.3.4.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|wishlistId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|wishlist|[customer_wishlist_flat](/schema/customer_wishlist_flat)|false|none|Added since version: 6.3.4.0|
|product|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
