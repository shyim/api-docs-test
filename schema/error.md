
# error

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string|false|none|A unique identifier for this particular occurrence of the problem.|
|links|[links](/schema/links)|false|none|none|
|status|string|false|none|The HTTP status code applicable to this problem, expressed as a string value.|
|code|string|false|none|An application-specific error code, expressed as a string value.|
|title|string|false|none|A short, human-readable summary of the problem. It **SHOULD NOT** change from occurrence to occurrence of the problem, except for purposes of localization.|
|detail|string|false|none|A human-readable explanation specific to this occurrence of the problem.|
|source|object|false|none|none|
|» pointer|string|false|none|A JSON Pointer [RFC6901] to the associated entity in the request document [e.g. "/data" for a primary data object, or "/data/attributes/title" for a specific attribute].|
|» parameter|string|false|none|A string indicating which query parameter caused the error.|
|meta|[meta](/schema/meta)|false|none|Non-standard meta-information that can not be represented as an attribute or relationship.|
