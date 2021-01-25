
# document_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|documentTypeId|string(uuid)|true|none|none|
|fileType|string|true|none|none|
|referencedDocumentId|string(uuid)|false|none|none|
|orderId|string(uuid)|true|none|none|
|documentMediaFileId|string(uuid)|false|none|none|
|orderVersionId|string(uuid)|false|none|none|
|config|object|true|none|none|
|sent|boolean|false|none|none|
|static|boolean|false|none|none|
|deepLinkCode|string|true|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|documentType|[document_type_flat](/schema/document_type_flat)|false|none|Added since version: 6.0.0.0|
|order|[order_flat](/schema/order_flat)|false|none|Added since version: 6.0.0.0|
|referencedDocument|[document_flat](/schema/document_flat)|false|none|Added since version: 6.0.0.0|
|dependentDocuments|[document_flat](/schema/document_flat)|false|none|Added since version: 6.0.0.0|
|documentMediaFile|[media_flat](/schema/media_flat)|false|none|Added since version: 6.0.0.0|
