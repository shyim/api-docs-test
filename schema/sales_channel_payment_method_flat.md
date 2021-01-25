
# sales_channel_payment_method_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|salesChannelId|string(uuid)|true|none|none|
|paymentMethodId|string(uuid)|true|none|none|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|paymentMethod|[payment_method_flat](/schema/payment_method_flat)|false|none|Added since version: 6.0.0.0|
