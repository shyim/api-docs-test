
# SalesChannelContext

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|token|string|false|none|none|
|currentCustomerGroup|object|false|none|none|
|» name|string|false|none|none|
|» displayGross|boolean|false|none|none|
|fallbackCustomerGroup|object|false|none|none|
|» name|string|false|none|none|
|» displayGross|boolean|false|none|none|
|currency|object|false|none|none|
|» isoCode|string|false|none|none|
|» factor|integer|false|none|none|
|» symbol|string|false|none|none|
|» shortName|string|false|none|none|
|» name|string|false|none|none|
|» position|integer(int32)|false|none|none|
|» decimalPrecision|integer(int32)|false|none|none|
|» isSystemDefault|boolean|false|none|none|
|salesChannel|object|false|none|none|
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
|» analyticsId|string|false|none|none|
|taxRules|[object]|false|none|none|
|» taxRate|number(float)|false|none|none|
|» name|string|false|none|none|
|customer|object|false|none|none|
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
|paymentMethod|object|false|none|none|
|» pluginId|string|false|none|none|
|» handlerIdentifier|string|false|none|none|
|» name|string|false|none|none|
|» description|string|false|none|none|
|» position|integer(int32)|false|none|none|
|» active|boolean|false|none|none|
|» availabilityRuleId|string|false|none|none|
|» mediaId|string|false|none|none|
|» formattedHandlerIdentifier|string|false|none|none|
|shippingMethod|object|false|none|none|
|» name|string|false|none|none|
|» active|boolean|false|none|none|
|» description|string|false|none|none|
|» trackingUrl|string|false|none|none|
|» deliveryTimeId|string|false|none|none|
|» availabilityRuleId|string|false|none|none|
|» mediaId|string|false|none|none|
|context|object|false|none|none|
|» versionId|string|false|none|none|
|» currencyId|string|false|none|none|
|» currencyFactor|integer|false|none|none|
|» currencyPrecision|integer(int32)|false|none|none|
|» scope|string|false|none|none|
|» source|string|false|none|none|
|» taxState|string|false|none|none|
|» useCache|boolean|false|none|none|
