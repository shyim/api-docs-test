
# relationships

{% hint style="info" %}

Members of the relationships object ("relationships") represent references from the resource object in which it's defined to other resource objects.

{% endhint %}

### Properties

{% hint style="info" %}

anyOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|

{% hint style="info" %}

or

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|

{% hint style="info" %}

or

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|

{% hint style="info" %}

or

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|
|» links|[relationshipLinks](/schema/relationshiplinks)|false|none|A resource object **MAY** contain references to other resource objects ("relationships"). Relationships may be to-one or to-many. Relationships can be specified by including a member in a resource's links object.|
|» data|any|false|none|Member, whose value represents "resource linkage".|

{% hint style="info" %}

oneOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|»» *anonymous*|[relationshipToOne](/schema/relationshiptoone)|false|none|none|

{% hint style="info" %}

xor

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|»» *anonymous*|[relationshipToMany](/schema/relationshiptomany)|false|none|An array of objects each containing \"type\" and \"id\" members for to-many relationships.|
