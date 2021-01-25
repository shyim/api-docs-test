
# country_state_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|countryId|string(uuid)|true|none|none|
|shortCode|string|true|none|none|
|name|string|true|none|none|
|position|integer(int64)|false|none|none|
|active|boolean|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|country|[country_flat](/schema/country_flat.md)|false|none|Added since version: 6.0.0.0|
