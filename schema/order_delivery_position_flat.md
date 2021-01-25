
# order_delivery_position_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|orderDeliveryId|string(uuid)|true|none|none|
|orderDeliveryVersionId|string(uuid)|false|none|none|
|orderLineItemId|string(uuid)|true|none|none|
|orderLineItemVersionId|string(uuid)|false|none|none|
|price|object|false|none|none|
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
|unitPrice|number(float)|false|none|none|
|totalPrice|number(float)|false|none|none|
|quantity|integer(int64)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|orderDelivery|[order_delivery_flat](/schema/order_delivery_flat.md)|false|none|Added since version: 6.0.0.0|
|orderLineItem|[order_line_item_flat](/schema/order_line_item_flat.md)|false|none|Added since version: 6.0.0.0|
