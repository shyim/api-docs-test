
# media_folder_configuration_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|createThumbnails|boolean|false|none|none|
|keepAspectRatio|boolean|false|none|none|
|thumbnailQuality|integer(int64)|false|none|none|
|private|boolean|false|none|none|
|noAssociation|boolean|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|mediaFolders|[media_folder_flat](/schema/media_folder_flat)|false|none|Added since version: 6.0.0.0|
|mediaThumbnailSizes|[media_thumbnail_size_flat](/schema/media_thumbnail_size_flat)|false|none|Added since version: 6.0.0.0|
