
# language_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|parentId|string(uuid)|false|none|none|
|localeId|string(uuid)|true|none|none|
|translationCodeId|string(uuid)|false|none|none|
|name|string|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|locale|[locale_flat](/schema/locale_flat)|false|none|Added since version: 6.0.0.0|
|translationCode|[locale_flat](/schema/locale_flat)|false|none|Added since version: 6.0.0.0|
|children|[language_flat](/schema/language_flat)|false|none|Added since version: 6.0.0.0|