
# category

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

{% hint style="info" %}

allOf

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[resource](/schema/resource.md)|false|none|"Resource objects" appear in a JSON API document to represent resources.|

{% hint style="info" %}

and

{% endhint %}

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|object|false|none|none|
|» id|string(uuid)|false|none|none|
|» versionId|string(uuid)|false|none|none|
|» parentId|string(uuid)|false|none|none|
|» parentVersionId|string(uuid)|false|none|none|
|» afterCategoryId|string(uuid)|false|none|none|
|» afterCategoryVersionId|string(uuid)|false|none|none|
|» mediaId|string(uuid)|false|none|none|
|» displayNestedProducts|boolean|true|none|none|
|» autoIncrement|integer(int64)|false|read-only|none|
|» breadcrumb|[string]|false|read-only|none|
|» level|integer(int64)|false|read-only|none|
|» path|string|false|read-only|none|
|» childCount|integer(int64)|false|read-only|none|
|» type|string|true|none|none|
|» productAssignmentType|string|true|none|none|
|» visible|boolean|false|none|none|
|» active|boolean|false|none|none|
|» name|string|true|none|none|
|» customFields|object|false|none|none|
|» slotConfig|object|false|none|none|
|» externalLink|string|false|none|none|
|» description|string|false|none|none|
|» metaTitle|string|false|none|none|
|» metaDescription|string|false|none|none|
|» keywords|string|false|none|none|
|» cmsPageId|string(uuid)|false|none|none|
|» productStreamId|string(uuid)|false|none|none|
|» createdAt|string(date-time)|true|read-only|none|
|» updatedAt|string(date-time)|false|read-only|none|
|» translated|object|false|none|none|
|» relationships|object|false|none|none|
|»» children|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» media|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» products|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» nestedProducts|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» tags|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» cmsPage|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» productStream|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» mainCategories|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» seoUrls|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
