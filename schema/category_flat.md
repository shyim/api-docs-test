
# category_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|parentId|string(uuid)|false|none|none|
|parentVersionId|string(uuid)|false|none|none|
|afterCategoryId|string(uuid)|false|none|none|
|afterCategoryVersionId|string(uuid)|false|none|none|
|mediaId|string(uuid)|false|none|none|
|displayNestedProducts|boolean|true|none|none|
|autoIncrement|integer(int64)|false|read-only|none|
|breadcrumb|[string]|false|read-only|none|
|level|integer(int64)|false|read-only|none|
|path|string|false|read-only|none|
|childCount|integer(int64)|false|read-only|none|
|type|string|true|none|none|
|productAssignmentType|string|true|none|none|
|visible|boolean|false|none|none|
|active|boolean|false|none|none|
|name|string|true|none|none|
|customFields|object|false|none|none|
|slotConfig|object|false|none|none|
|externalLink|string|false|none|none|
|description|string|false|none|none|
|metaTitle|string|false|none|none|
|metaDescription|string|false|none|none|
|keywords|string|false|none|none|
|cmsPageId|string(uuid)|false|none|none|
|productStreamId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|children|[category_flat](/schema/category_flat.md)|false|none|Added since version: 6.0.0.0|
|media|[media_flat](/schema/media_flat.md)|false|none|Added since version: 6.0.0.0|
|products|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
|nestedProducts|[product_flat](/schema/product_flat.md)|false|none|Added since version: 6.0.0.0|
|tags|[tag_flat](/schema/tag_flat.md)|false|none|Added since version: 6.0.0.0|
|cmsPage|[cms_page_flat](/schema/cms_page_flat.md)|false|none|Added since version: 6.0.0.0|
|productStream|[product_stream_flat](/schema/product_stream_flat.md)|false|none|Added since version: 6.0.0.0|
|mainCategories|[main_category_flat](/schema/main_category_flat.md)|false|none|Added since version: 6.1.0.0|
|seoUrls|[seo_url_flat](/schema/seo_url_flat.md)|false|none|Added since version: 6.0.0.0|
