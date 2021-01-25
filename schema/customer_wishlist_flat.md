
# customer_wishlist_flat

{% hint style="info" %}

Added since version: 6.3.4.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|customerId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|products|[customer_wishlist_product_flat](/schema/customer_wishlist_product_flat.md)|false|none|Added since version: 6.3.4.0|
