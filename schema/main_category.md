
# main_category

{% hint style="info" %}

Added since version: 6.1.0.0

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
|» productId|string(uuid)|true|none|none|
|» productVersionId|string(uuid)|false|none|none|
|» categoryId|string(uuid)|true|none|none|
|» categoryVersionId|string(uuid)|false|none|none|
|» salesChannelId|string(uuid)|true|none|none|
|» createdAt|string(date-time)|true|read-only|none|
|» updatedAt|string(date-time)|false|read-only|none|
|» relationships|object|false|none|none|
|»» product|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» category|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
