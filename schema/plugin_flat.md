
# plugin_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|baseClass|string|true|none|none|
|name|string|true|none|none|
|composerName|string|false|none|none|
|autoload|object|true|none|none|
|active|boolean|false|none|none|
|managedByComposer|boolean|false|none|none|
|path|string|false|none|none|
|author|string|false|none|none|
|copyright|string|false|none|none|
|license|string|false|none|none|
|version|string|true|none|none|
|upgradeVersion|string|false|none|none|
|installedAt|string(date-time)|false|none|none|
|upgradedAt|string(date-time)|false|none|none|
|icon|string|false|read-only|none|
|label|string|true|none|none|
|description|string|false|none|none|
|manufacturerLink|string|false|none|none|
|supportLink|string|false|none|none|
|changelog|object|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|paymentMethods|[payment_method_flat](/schema/payment_method_flat.md)|false|none|Added since version: 6.0.0.0|
