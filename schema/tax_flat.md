
# tax_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|taxRate|number(float)|true|none|none|
|name|string|true|none|none|
|position|integer(int64)|true|none|Added since version: 6.4.0.0|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|products|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|shippingMethods|[shipping_method_flat](/schema/shipping_method_flat)|false|none|Added since version: 6.0.0.0|
