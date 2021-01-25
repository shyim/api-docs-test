
# country

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
|» name|string|true|none|none|
|» iso|string|false|none|none|
|» position|integer(int64)|false|none|none|
|» taxFree|boolean|false|none|none|
|» active|boolean|false|none|none|
|» shippingAvailable|boolean|false|none|none|
|» iso3|string|false|none|none|
|» displayStateInRegistration|boolean|false|none|none|
|» forceStateInRegistration|boolean|false|none|none|
|» companyTaxFree|boolean|false|none|none|
|» checkVatIdPattern|boolean|false|none|none|
|» vatIdPattern|string|false|none|none|
|» customFields|object|false|none|none|
|» createdAt|string(date-time)|true|read-only|none|
|» updatedAt|string(date-time)|false|read-only|none|
|» translated|object|false|none|none|
|» relationships|object|false|none|none|
|»» states|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
