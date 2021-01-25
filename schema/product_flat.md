
# product_flat

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
|manufacturerId|string(uuid)|false|none|none|
|productManufacturerVersionId|string(uuid)|false|none|none|
|unitId|string(uuid)|false|none|none|
|taxId|string(uuid)|true|none|none|
|coverId|string(uuid)|false|none|none|
|productMediaVersionId|string(uuid)|false|none|none|
|deliveryTimeId|string(uuid)|false|none|none|
|productNumber|string|true|none|none|
|stock|integer(int64)|true|none|none|
|restockTime|integer(int64)|false|none|none|
|autoIncrement|integer(int64)|false|read-only|none|
|active|boolean|false|none|none|
|availableStock|integer(int64)|false|read-only|none|
|available|boolean|false|read-only|none|
|isCloseout|boolean|false|none|none|
|displayGroup|string|false|read-only|none|
|mainVariantId|string(uuid)|false|none|none|
|manufacturerNumber|string|false|none|none|
|ean|string|false|none|none|
|purchaseSteps|integer(int64)|false|none|none|
|maxPurchase|integer(int64)|false|none|none|
|minPurchase|integer(int64)|false|none|none|
|purchaseUnit|number(float)|false|none|none|
|referenceUnit|number(float)|false|none|none|
|shippingFree|boolean|false|none|none|
|purchasePrice|number(float)|false|none|none|
|markAsTopseller|boolean|false|none|none|
|weight|number(float)|false|none|none|
|width|number(float)|false|none|none|
|height|number(float)|false|none|none|
|length|number(float)|false|none|none|
|releaseDate|string(date-time)|false|none|none|
|ratingAverage|number(float)|false|read-only|none|
|categoryTree|[string]|false|read-only|none|
|propertyIds|[string]|false|read-only|none|
|optionIds|[string]|false|read-only|none|
|tagIds|[string]|false|read-only|none|
|childCount|integer(int64)|false|read-only|none|
|customFieldSetSelectionActive|boolean|false|none|none|
|sales|integer(int64)|false|read-only|none|
|metaDescription|string|false|none|none|
|name|string|true|none|none|
|keywords|string|false|none|none|
|description|string|false|none|none|
|metaTitle|string|false|none|none|
|packUnit|string|false|none|none|
|packUnitPlural|string|false|none|none|
|customFields|object|false|none|none|
|variation|[string]|false|none|none|
|featureSetId|string(uuid)|false|none|none|
|purchasePrices|object|false|none|none|
|customSearchKeywords|[any]|false|none|none|
|canonicalProductId|string(uuid)|false|none|none|
|calculatedPrice|object|false|none|none|
|calculatedListingPrice|object|false|none|none|
|calculatedPrices|[any]|false|none|none|
|calculatedMaxPurchase|integer(int64)|false|none|none|
|isNew|boolean|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|children|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|deliveryTime|[delivery_time_flat](/schema/delivery_time_flat)|false|none|Added since version: 6.0.0.0|
|tax|[tax_flat](/schema/tax_flat)|false|none|Added since version: 6.0.0.0|
|manufacturer|[product_manufacturer_flat](/schema/product_manufacturer_flat)|false|none|Added since version: 6.0.0.0|
|unit|[unit_flat](/schema/unit_flat)|false|none|Added since version: 6.0.0.0|
|cover|[product_media_flat](/schema/product_media_flat)|false|none|Added since version: 6.0.0.0|
|media|[product_media_flat](/schema/product_media_flat)|false|none|Added since version: 6.0.0.0|
|crossSellings|[product_cross_selling_flat](/schema/product_cross_selling_flat)|false|none|Added since version: 6.1.0.0|
|crossSellingAssignedProducts|[product_cross_selling_assigned_products_flat](/schema/product_cross_selling_assigned_products_flat)|false|none|Added since version: 6.2.0.0|
|productReviews|[product_review_flat](/schema/product_review_flat)|false|none|Added since version: 6.0.0.0|
|mainCategories|[main_category_flat](/schema/main_category_flat)|false|none|Added since version: 6.1.0.0|
|seoUrls|[seo_url_flat](/schema/seo_url_flat)|false|none|Added since version: 6.0.0.0|
|options|[property_group_option_flat](/schema/property_group_option_flat)|false|none|Added since version: 6.0.0.0|
|properties|[property_group_option_flat](/schema/property_group_option_flat)|false|none|Added since version: 6.0.0.0|
|categories|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
|categoriesRo|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
|tags|[tag_flat](/schema/tag_flat)|false|none|Added since version: 6.0.0.0|
|customFieldSets|[custom_field_set_flat](/schema/custom_field_set_flat)|false|none|Added since version: 6.0.0.0|
|featureSet|[product_feature_set_flat](/schema/product_feature_set_flat)|false|none|Added since version: 6.3.0.0|
|wishlists|[customer_wishlist_product_flat](/schema/customer_wishlist_product_flat)|false|none|Added since version: 6.3.4.0|
|canonicalProduct|[product_flat](/schema/product_flat)|false|none|Added since version: 6.0.0.0|
|seoCategory|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
