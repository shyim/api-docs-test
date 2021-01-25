
# product

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
|» manufacturerId|string(uuid)|false|none|none|
|» productManufacturerVersionId|string(uuid)|false|none|none|
|» unitId|string(uuid)|false|none|none|
|» taxId|string(uuid)|true|none|none|
|» coverId|string(uuid)|false|none|none|
|» productMediaVersionId|string(uuid)|false|none|none|
|» deliveryTimeId|string(uuid)|false|none|none|
|» productNumber|string|true|none|none|
|» stock|integer(int64)|true|none|none|
|» restockTime|integer(int64)|false|none|none|
|» autoIncrement|integer(int64)|false|read-only|none|
|» active|boolean|false|none|none|
|» availableStock|integer(int64)|false|read-only|none|
|» available|boolean|false|read-only|none|
|» isCloseout|boolean|false|none|none|
|» displayGroup|string|false|read-only|none|
|» mainVariantId|string(uuid)|false|none|none|
|» manufacturerNumber|string|false|none|none|
|» ean|string|false|none|none|
|» purchaseSteps|integer(int64)|false|none|none|
|» maxPurchase|integer(int64)|false|none|none|
|» minPurchase|integer(int64)|false|none|none|
|» purchaseUnit|number(float)|false|none|none|
|» referenceUnit|number(float)|false|none|none|
|» shippingFree|boolean|false|none|none|
|» purchasePrice|number(float)|false|none|none|
|» markAsTopseller|boolean|false|none|none|
|» weight|number(float)|false|none|none|
|» width|number(float)|false|none|none|
|» height|number(float)|false|none|none|
|» length|number(float)|false|none|none|
|» releaseDate|string(date-time)|false|none|none|
|» ratingAverage|number(float)|false|read-only|none|
|» categoryTree|[string]|false|read-only|none|
|» propertyIds|[string]|false|read-only|none|
|» optionIds|[string]|false|read-only|none|
|» tagIds|[string]|false|read-only|none|
|» childCount|integer(int64)|false|read-only|none|
|» customFieldSetSelectionActive|boolean|false|none|none|
|» sales|integer(int64)|false|read-only|none|
|» metaDescription|string|false|none|none|
|» name|string|true|none|none|
|» keywords|string|false|none|none|
|» description|string|false|none|none|
|» metaTitle|string|false|none|none|
|» packUnit|string|false|none|none|
|» packUnitPlural|string|false|none|none|
|» customFields|object|false|none|none|
|» variation|[string]|false|none|none|
|» featureSetId|string(uuid)|false|none|none|
|» purchasePrices|object|false|none|none|
|» customSearchKeywords|[any]|false|none|none|
|» canonicalProductId|string(uuid)|false|none|none|
|» calculatedPrice|object|false|none|none|
|» calculatedListingPrice|object|false|none|none|
|» calculatedPrices|[any]|false|none|none|
|» calculatedMaxPurchase|integer(int64)|false|none|none|
|» isNew|boolean|false|none|none|
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
|»» deliveryTime|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» tax|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» manufacturer|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» unit|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» cover|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» media|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» crossSellings|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» crossSellingAssignedProducts|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» productReviews|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
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
|»» options|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» properties|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» categories|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» categoriesRo|object|false|none|none|
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
|»» customFieldSets|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» featureSet|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» wishlists|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|[object]|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string|false|none|none|
|»» canonicalProduct|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
|»» seoCategory|object|false|none|none|
|»»» links|object|false|none|none|
|»»»» related|string(uri-reference)|false|none|none|
|»»» data|object|false|none|none|
|»»»» type|string|false|none|none|
|»»»» id|string(uuid)|false|none|none|
