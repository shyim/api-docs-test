
# media_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|mimeType|string|false|read-only|none|
|fileExtension|string|false|read-only|none|
|uploadedAt|string(date-time)|false|read-only|none|
|fileName|string|false|read-only|none|
|fileSize|integer(int64)|false|read-only|none|
|metaData|object|false|read-only|none|
|alt|string|false|none|none|
|title|string|false|none|none|
|url|string|false|none|none|
|hasFile|boolean|false|none|none|
|private|boolean|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|tags|[tag_flat](/schema/tag_flat.md)|false|none|Added since version: 6.0.0.0|
|thumbnails|[media_thumbnail_flat](/schema/media_thumbnail_flat.md)|false|none|Added since version: 6.0.0.0|
