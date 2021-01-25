
# ShippingMethodPageRouteResponse

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|false|none|none|
|active|boolean|false|none|none|
|description|string|false|none|none|
|deliveryTimeId|string|false|none|none|
|deliveryTime|object|false|none|none|
|» name|string|false|none|none|
|» min|integer(int32)|false|none|none|
|» max|integer(int32)|false|none|none|
|» unit|string|false|none|none|
|translations|[object]|false|none|none|
|» shippingMethodId|string|false|none|none|
|» name|string|false|none|none|
|» description|string|false|none|none|
|orderDeliveries|[object]|false|none|none|
|» orderId|string|false|none|none|
|» shippingOrderAddressId|string|false|none|none|
|» shippingMethodId|string|false|none|none|
|» shippingDateEarliest|string(date-time)|false|none|none|
|» shippingDateLatest|string(date-time)|false|none|none|
|» stateId|string|false|none|none|
|salesChannelDefaultAssignments|[object]|false|none|none|
|» typeId|string|false|none|none|
|» languageId|string|false|none|none|
|» currencyId|string|false|none|none|
|» paymentMethodId|string|false|none|none|
|» shippingMethodId|string|false|none|none|
|» countryId|string|false|none|none|
|» navigationCategoryId|string|false|none|none|
|» navigationCategoryDepth|integer(int32)|false|none|none|
|» footerCategoryId|string|false|none|none|
|» serviceCategoryId|string|false|none|none|
|» name|string|false|none|none|
|» shortName|string|false|none|none|
|» accessKey|string|false|none|none|
|» active|boolean|false|none|none|
|» maintenance|boolean|false|none|none|
|» maintenanceIpWhitelist|string|false|none|none|
|» mailHeaderFooterId|string|false|none|none|
|» customerGroupId|string|false|none|none|
|» hreflangActive|boolean|false|none|none|
|» hreflangDefaultDomainId|string|false|none|none|
|salesChannels|[object]|false|none|none|
|» typeId|string|false|none|none|
|» languageId|string|false|none|none|
|» currencyId|string|false|none|none|
|» paymentMethodId|string|false|none|none|
|» shippingMethodId|string|false|none|none|
|» countryId|string|false|none|none|
|» navigationCategoryId|string|false|none|none|
|» navigationCategoryDepth|integer(int32)|false|none|none|
|» footerCategoryId|string|false|none|none|
|» serviceCategoryId|string|false|none|none|
|» name|string|false|none|none|
|» shortName|string|false|none|none|
|» accessKey|string|false|none|none|
|» active|boolean|false|none|none|
|» maintenance|boolean|false|none|none|
|» maintenanceIpWhitelist|string|false|none|none|
|» mailHeaderFooterId|string|false|none|none|
|» customerGroupId|string|false|none|none|
|» hreflangActive|boolean|false|none|none|
|» hreflangDefaultDomainId|string|false|none|none|
|availabilityRule|object|false|none|none|
|» name|string|false|none|none|
|» description|string|false|none|none|
|» priority|integer(int32)|false|none|none|
|» invalid|boolean|false|none|none|
|availabilityRuleId|string|false|none|none|
|prices|[object]|false|none|none|
|» shippingMethodId|string|false|none|none|
|» currencyId|string|false|none|none|
|» ruleId|string|false|none|none|
|» calculation|integer(int32)|false|none|none|
|» quantityStart|number(float)|false|none|none|
|» quantityEnd|number(float)|false|none|none|
|» price|number(float)|false|none|none|
|» calculationRuleId|string|false|none|none|
|mediaId|string|false|none|none|
|media|object|false|none|none|
|» userId|string|false|none|none|
|» mimeType|string|false|none|none|
|» fileExtension|string|false|none|none|
|» fileSize|integer(int32)|false|none|none|
|» title|string|false|none|none|
|» metaDataRaw|string|false|none|none|
|» mediaTypeRaw|string|false|none|none|
|» uploadedAt|string(date-time)|false|none|none|
|» alt|string|false|none|none|
|» url|string|false|none|none|
|» fileName|string|false|none|none|
|» mediaFolderId|string|false|none|none|
|» private|boolean|false|none|none|
|» thumbnailsRo|string|false|none|none|
|tags|[object]|false|none|none|
|» name|string|false|none|none|
