
# sales_channel_domain_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|url|string|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|languageId|string(uuid)|true|none|none|
|currencyId|string(uuid)|true|none|none|
|snippetSetId|string(uuid)|true|none|none|
|hreflangUseOnlyLocale|boolean|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|language|[language_flat](/schema/language_flat)|false|none|Added since version: 6.0.0.0|
|currency|[currency_flat](/schema/currency_flat)|false|none|Added since version: 6.0.0.0|
|snippetSet|[snippet_set_flat](/schema/snippet_set_flat)|false|none|Added since version: 6.0.0.0|
|salesChannelDefaultHreflang|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
