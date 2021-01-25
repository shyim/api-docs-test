
# Cart

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|false|none|none|
|token|string|false|none|none|
|price|object|false|none|none|
|» netPrice|number(float)|false|none|none|
|» totalPrice|number(float)|false|none|none|
|» positionPrice|number(float)|false|none|none|
|» taxStatus|string|false|none|none|
|lineItems|[object]|false|none|none|
|» id|string|false|none|none|
|» referencedId|string|false|none|none|
|» label|string|false|none|none|
|» quantity|integer(int32)|false|none|none|
|» type|string|false|none|none|
|» good|boolean|false|none|none|
|» description|string|false|none|none|
|» removable|boolean|false|none|none|
|» stackable|boolean|false|none|none|
|» modified|boolean|false|none|none|
|errors|[object]|false|none|none|
|» key|string|false|none|none|
|» level|string|false|none|none|
|» message|string|false|none|none|
|transactions|[object]|false|none|none|
|» paymentMethodId|string|false|none|none|
|modified|boolean|false|none|none|
|customerComment|string|false|none|none|
|affiliateCode|string|false|none|none|
|campaignCode|string|false|none|none|
