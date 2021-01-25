
# property_group_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|description|string|false|none|none|
|displayType|string|true|none|none|
|sortingType|string|true|none|none|
|filterable|boolean|false|none|none|
|position|integer(int64)|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|options|[property_group_option_flat](/schema/property_group_option_flat)|false|none|Added since version: 6.0.0.0|
