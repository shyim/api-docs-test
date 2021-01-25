
# seo_url

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

{% hint style="info" %}

allOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[resource](/schema/resource)|false|none|"Resource objects" appear in a JSON API document to represent resources.|

{% hint style="info" %}

and

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|
|» id|string(uuid)|false|none|none|
|» salesChannelId|string(uuid)|false|none|none|
|» languageId|string(uuid)|true|none|none|
|» foreignKey|string(uuid)|true|none|none|
|» routeName|string|true|none|none|
|» pathInfo|string|true|none|none|
|» seoPathInfo|string|true|none|none|
|» isCanonical|boolean|false|none|none|
|» isModified|boolean|false|none|none|
|» isDeleted|boolean|false|none|none|
|» url|string|false|none|none|
|» customFields|object|false|none|none|
|» createdAt|string(date-time)|true|read-only|none|
|» updatedAt|string(date-time)|false|read-only|none|
|» relationships|object|false|none|none|
|»» language|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
