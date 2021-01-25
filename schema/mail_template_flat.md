
# mail_template_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|mailTemplateTypeId|string(uuid)|true|none|none|
|systemDefault|boolean|false|none|none|
|senderName|string|false|none|none|
|description|string|false|none|none|
|subject|string|true|none|none|
|contentHtml|string|true|none|none|
|contentPlain|string|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|salesChannels|[mail_template_sales_channel_flat](/schema/mail_template_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|mailTemplateType|[mail_template_type_flat](/schema/mail_template_type_flat)|false|none|Added since version: 6.0.0.0|
|media|[mail_template_media_flat](/schema/mail_template_media_flat)|false|none|Added since version: 6.0.0.0|
