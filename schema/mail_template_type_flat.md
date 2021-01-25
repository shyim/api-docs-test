
# mail_template_type_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|technicalName|string|true|none|none|
|availableEntities|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|customFields|object|false|none|none|
|translated|object|false|none|none|
|mailTemplates|[mail_template_flat](/schema/mail_template_flat)|false|none|Added since version: 6.0.0.0|
|salesChannels|[mail_template_sales_channel_flat](/schema/mail_template_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
