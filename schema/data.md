
# data

{% hint style="info" %}

The document's "primary data" is a representation of the resource or collection of resources targeted by a request.

{% endhint %}

### Properties

{% hint style="info" %}

oneOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[resource](/schema/resource)|false|none|"Resource objects" appear in a JSON API document to represent resources.|

{% hint style="info" %}

xor

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[[resource](/schema/resource.md)]|false|none|An array of resource objects, an array of resource identifier objects, or an empty array ([]), for requests that target resource collections.|
