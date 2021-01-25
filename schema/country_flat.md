
# country_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|name|string|true|none|none|
|iso|string|false|none|none|
|position|integer(int64)|false|none|none|
|taxFree|boolean|false|none|none|
|active|boolean|false|none|none|
|shippingAvailable|boolean|false|none|none|
|iso3|string|false|none|none|
|displayStateInRegistration|boolean|false|none|none|
|forceStateInRegistration|boolean|false|none|none|
|companyTaxFree|boolean|false|none|none|
|checkVatIdPattern|boolean|false|none|none|
|vatIdPattern|string|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|states|[country_state_flat](/schema/country_state_flat)|false|none|Added since version: 6.0.0.0|
