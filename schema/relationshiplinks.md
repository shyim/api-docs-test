
# relationshipLinks

{% hint style="info" %}

A resource object **MAY** contain references to other resource objects ("relationships"). Relationships may be to-one or to-many. Relationships can be specified by including a member in a resource's links object.

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|self|any|false|none|none|

{% hint style="info" %}

allOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|array|false|none|A `self` member, whose value is a URL for the relationship itself (a "relationship URL"). This URL allows the client to directly manipulate the relationship. For example, it would allow a client to remove an `author` from an `article` without deleting the people resource itself.|

{% hint style="info" %}

and

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|» *anonymous*|[link](/schema/link)|false|none|A link **MUST** be represented as either: a string containing the link's URL or a link object.|

{% hint style="info" %}

continued

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|related|[link](/schema/link)|false|none|A link **MUST** be represented as either: a string containing the link's URL or a link object.|
