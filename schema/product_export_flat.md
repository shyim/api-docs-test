
# product_export_flat

{% hint style="info" %}

Added since version: 6.1.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|productStreamId|string(uuid)|true|none|none|
|storefrontSalesChannelId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|salesChannelDomainId|string(uuid)|true|none|none|
|currencyId|string(uuid)|true|none|none|
|fileName|string|true|none|none|
|accessKey|string|true|none|none|
|encoding|string|true|none|none|
|fileFormat|string|true|none|none|
|includeVariants|boolean|false|none|none|
|generateByCronjob|boolean|true|none|none|
|generatedAt|string(date-time)|false|none|none|
|interval|integer(int64)|true|none|none|
|headerTemplate|string|false|none|none|
|bodyTemplate|string|false|none|none|
|footerTemplate|string|false|none|none|
|pausedSchedule|boolean|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|productStream|[product_stream_flat](/schema/product_stream_flat.md)|false|none|Added since version: 6.0.0.0|
|storefrontSalesChannel|[sales_channel_flat](/schema/sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
|salesChannelDomain|[sales_channel_domain_flat](/schema/sales_channel_domain_flat.md)|false|none|Added since version: 6.0.0.0|
|currency|[currency_flat](/schema/currency_flat.md)|false|none|Added since version: 6.0.0.0|
