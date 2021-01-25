
# customer_group_registration_sales_channels_flat

{% hint style="info" %}

Added since version: 6.3.1.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|customerGroupId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|customerGroup|[customer_group_flat](/schema/customer_group_flat)|false|none|Added since version: 6.0.0.0|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
