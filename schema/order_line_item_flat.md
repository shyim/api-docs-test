
# order_line_item_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|orderId|string(uuid)|true|none|none|
|orderVersionId|string(uuid)|false|none|none|
|productId|string(uuid)|false|none|none|
|productVersionId|string(uuid)|false|none|none|
|parentId|string(uuid)|false|none|none|
|parentVersionId|string(uuid)|false|none|none|
|coverId|string(uuid)|false|none|none|
|identifier|string|true|none|none|
|referencedId|string|false|none|none|
|quantity|integer(int64)|true|none|none|
|label|string|true|none|none|
|payload|object|false|none|none|
|good|boolean|false|none|none|
|removable|boolean|false|none|none|
|stackable|boolean|false|none|none|
|position|integer(int64)|true|none|none|
|price|object|true|none|none|
|» unitPrice|number(float)|true|none|none|
|» totalPrice|number(float)|true|none|none|
|» quantity|integer(int64)|true|none|none|
|» calculatedTaxes|object|false|none|none|
|» taxRules|object|false|none|none|
|» referencePrice|object|false|none|none|
|» listPrice|object|false|none|none|
|»» price|number(float)|false|none|none|
|»» discount|number(float)|false|none|none|
|»» percentage|number(float)|false|none|none|
|priceDefinition|object|false|none|none|
|unitPrice|number(float)|false|none|none|
|totalPrice|number(float)|false|none|none|
|description|string|false|none|none|
|type|string|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|cover|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|order|[order_flat](/schema/order_flat.md)|false|none|Added since version: 6.0.0.0|
|product|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
|orderDeliveryPositions|[order_delivery_position_flat](/schema/order_delivery_position_flat.md)|false|none|Added since version: 6.0.0.0|
