
# language

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

{% hint style="info" %}

allOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[resource](/schema/resource.md)|false|none|"Resource objects" appear in a JSON API document to represent resources.|

{% hint style="info" %}

and

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|
|» id|string(uuid)|false|none|none|
|» parentId|string(uuid)|false|none|none|
|» localeId|string(uuid)|true|none|none|
|» translationCodeId|string(uuid)|false|none|none|
|» name|string|true|none|none|
|» customFields|object|false|none|none|
|» createdAt|string(date-time)|true|read-only|none|
|» updatedAt|string(date-time)|false|read-only|none|
|» relationships|object|false|none|none|
|»» locale|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» translationCode|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» children|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
