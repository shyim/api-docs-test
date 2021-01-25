
# product_search_keyword_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|languageId|string(uuid)|true|none|none|
|productId|string(uuid)|true|none|none|
|productVersionId|string(uuid)|false|none|none|
|keyword|string|true|none|none|
|ranking|number(float)|true|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|product|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
|language|[language_flat](/schema/language_flat.md)|false|none|Added since version: 6.0.0.0|
