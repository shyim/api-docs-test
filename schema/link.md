
# link

{% hint style="info" %}

A link **MUST** be represented as either: a string containing the link's URL or a link object.

{% endhint %}

### Properties

{% hint style="info" %}

oneOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|string(uri-reference)|false|none|A string containing the link's URL.|

{% hint style="info" %}

xor

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|
|» href|string(uri-reference)|true|none|A string containing the link's URL.|
|» meta|[meta](/schema/meta.md)|false|none|Non-standard meta-information that can not be represented as an attribute or relationship.|
