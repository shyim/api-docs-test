
# success

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|meta|[meta](/schema/meta.md)|false|none|Non-standard meta-information that can not be represented as an attribute or relationship.|
|links|any|false|none|Link members related to the primary data.|

{% hint style="info" %}

allOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|[links](/schema/links.md)|false|none|none|

{% hint style="info" %}

and

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|[pagination](/schema/pagination.md)|false|none|none|

{% hint style="info" %}

continued

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|data|[data](/schema/data.md)|true|none|The document's "primary data" is a representation of the resource or collection of resources targeted by a request.|
|included|[[resource](/schema/resource.md)]|false|none|To reduce the number of HTTP requests, servers **MAY** allow responses that include related resources along with the requested primary resources. Such responses are called "compound documents".|
