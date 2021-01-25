
# newsletter_recipient_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|email|string|true|none|none|
|title|string|false|none|none|
|firstName|string|false|none|none|
|lastName|string|false|none|none|
|zipCode|string|false|none|none|
|city|string|false|none|none|
|street|string|false|none|none|
|status|string|true|none|none|
|hash|string|true|none|none|
|customFields|object|false|none|none|
|confirmedAt|string(date-time)|false|none|none|
|salutationId|string(uuid)|false|none|none|
|languageId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|tags|[tag_flat](/schema/tag_flat.md)|false|none|Added since version: 6.0.0.0|
|salutation|[salutation_flat](/schema/salutation_flat.md)|false|none|Added since version: 6.0.0.0|
|language|[language_flat](/schema/language_flat.md)|false|none|Added since version: 6.0.0.0|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat.md)|false|none|Added since version: 6.0.0.0|
