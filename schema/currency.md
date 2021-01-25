
# currency

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
|» factor|number(float)|true|none|none|
|» symbol|string|true|none|none|
|» isoCode|string|true|none|none|
|» shortName|string|true|none|none|
|» name|string|true|none|none|
|» decimalPrecision|integer(int64)|true|none|none|
|» position|integer(int64)|false|none|none|
|» isSystemDefault|boolean|false|none|none|
|» customFields|object|false|none|none|
|» createdAt|string(date-time)|true|read-only|none|
|» updatedAt|string(date-time)|false|read-only|none|
|» translated|object|false|none|none|
