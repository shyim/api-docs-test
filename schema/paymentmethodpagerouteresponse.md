
# PaymentMethodPageRouteResponse

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|pluginId|string|false|none|none|
|handlerIdentifier|string|false|none|none|
|name|string|false|none|none|
|description|string|false|none|none|
|position|integer(int32)|false|none|none|
|active|boolean|false|none|none|
|plugin|object|false|none|none|
|» baseClass|string|false|none|none|
|» name|string|false|none|none|
|» composerName|string|false|none|none|
|» active|boolean|false|none|none|
|» managedByComposer|boolean|false|none|none|
|» path|string|false|none|none|
|» author|string|false|none|none|
|» copyright|string|false|none|none|
|» license|string|false|none|none|
|» version|string|false|none|none|
|» upgradeVersion|string|false|none|none|
|» installedAt|string(date-time)|false|none|none|
|» upgradedAt|string(date-time)|false|none|none|
|» iconRaw|string|false|none|none|
|» icon|string|false|none|none|
|» label|string|false|none|none|
|» description|string|false|none|none|
|» manufacturerLink|string|false|none|none|
|» supportLink|string|false|none|none|
|translations|[object]|false|none|none|
|» paymentMethodId|string|false|none|none|
|» name|string|false|none|none|
|» description|string|false|none|none|
|orderTransactions|[object]|false|none|none|
|» orderId|string|false|none|none|
|» paymentMethodId|string|false|none|none|
|» stateId|string|false|none|none|
|customers|[object]|false|none|none|
|» groupId|string|false|none|none|
|» defaultPaymentMethodId|string|false|none|none|
|» salesChannelId|string|false|none|none|
|» languageId|string|false|none|none|
|» lastPaymentMethodId|string|false|none|none|
|» defaultBillingAddressId|string|false|none|none|
|» defaultShippingAddressId|string|false|none|none|
|» customerNumber|string|false|none|none|
|» salutationId|string|false|none|none|
|» firstName|string|false|none|none|
|» lastName|string|false|none|none|
|» company|string|false|none|none|
|» password|string|false|none|none|
|» email|string|false|none|none|
|» title|string|false|none|none|
|» affiliateCode|string|false|none|none|
|» campaignCode|string|false|none|none|
|» active|boolean|false|none|none|
|» doubleOptInRegistration|boolean|false|none|none|
|» doubleOptInEmailSentDate|string(date-time)|false|none|none|
|» doubleOptInConfirmDate|string(date-time)|false|none|none|
|» hash|string|false|none|none|
|» guest|boolean|false|none|none|
|» firstLogin|string(date-time)|false|none|none|
|» lastLogin|string(date-time)|false|none|none|
|» newsletter|boolean|false|none|none|
|» birthday|string(date-time)|false|none|none|
|» lastOrderDate|string(date-time)|false|none|none|
|» orderCount|integer(int32)|false|none|none|
|» legacyEncoder|string|false|none|none|
|» legacyPassword|string|false|none|none|
|» autoIncrement|integer(int32)|false|none|none|
|» remoteAddress|string|false|none|none|
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
|formattedHandlerIdentifier|string|false|none|none|
