
# sales_channel_shipping_method_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|salesChannelId|string(uuid)|true|none|none|
|shippingMethodId|string(uuid)|true|none|none|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|shippingMethod|[shipping_method_flat](/schema/shipping_method_flat)|false|none|Added since version: 6.0.0.0|
