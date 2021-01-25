
# resource

{% hint style="info" %}

"Resource objects" appear in a JSON API document to represent resources.

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|type|string|true|none|none|
|id|string|true|none|none|
|attributes|[attributes](/schema/attributes.md)|false|none|Members of the attributes object ("attributes") represent information about the resource object in which it's defined.|
|relationships|[relationships](/schema/relationships.md)|false|none|Members of the relationships object ("relationships") represent references from the resource object in which it's defined to other resource objects.|
|links|[links](/schema/links.md)|false|none|none|
|meta|[meta](/schema/meta.md)|false|none|Non-standard meta-information that can not be represented as an attribute or relationship.|
