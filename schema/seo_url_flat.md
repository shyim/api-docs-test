
# seo_url_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|salesChannelId|string(uuid)|false|none|none|
|languageId|string(uuid)|true|none|none|
|foreignKey|string(uuid)|true|none|none|
|routeName|string|true|none|none|
|pathInfo|string|true|none|none|
|seoPathInfo|string|true|none|none|
|isCanonical|boolean|false|none|none|
|isModified|boolean|false|none|none|
|isDeleted|boolean|false|none|none|
|url|string|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|language|[language_flat](/schema/language_flat)|false|none|Added since version: 6.0.0.0|
