
# mail_template_sales_channel_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|mailTemplateId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|mailTemplateTypeId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|mailTemplateType|[mail_template_type_flat](/schema/mail_template_type_flat)|false|none|Added since version: 6.0.0.0|
|mailTemplate|[mail_template_flat](/schema/mail_template_flat)|false|none|Added since version: 6.0.0.0|
|salesChannel|[sales_channel_flat](/schema/sales_channel_flat)|false|none|Added since version: 6.0.0.0|
