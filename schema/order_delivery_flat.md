
# order_delivery_flat

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
|shippingOrderAddressId|string(uuid)|true|none|none|
|shippingOrderAddressVersionId|string(uuid)|false|none|none|
|shippingMethodId|string(uuid)|true|none|none|
|stateId|string(uuid)|true|none|none|
|trackingCodes|[string]|true|none|none|
|shippingDateEarliest|string(date-time)|true|none|none|
|shippingDateLatest|string(date-time)|true|none|none|
|shippingCosts|object|false|none|none|
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
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|stateMachineState|[state_machine_state_flat](/schema/state_machine_state_flat.md)|false|none|Added since version: 6.0.0.0|
|order|[order_flat](/schema/order_flat.md)|false|none|Added since version: 6.0.0.0|
|shippingOrderAddress|[order_address_flat](/schema/order_address_flat.md)|false|none|Added since version: 6.0.0.0|
|shippingMethod|[shipping_method_flat](/schema/shipping_method_flat.md)|false|none|Added since version: 6.0.0.0|
|positions|[order_delivery_position_flat](/schema/order_delivery_position_flat.md)|false|none|Added since version: 6.0.0.0|
