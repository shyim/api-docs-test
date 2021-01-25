
# sales_channel_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|typeId|string(uuid)|true|none|none|
|languageId|string(uuid)|true|none|none|
|customerGroupId|string(uuid)|true|none|none|
|currencyId|string(uuid)|true|none|none|
|paymentMethodId|string(uuid)|true|none|none|
|shippingMethodId|string(uuid)|true|none|none|
|countryId|string(uuid)|true|none|none|
|analyticsId|string(uuid)|false|none|none|
|navigationCategoryId|string(uuid)|true|none|none|
|navigationCategoryVersionId|string(uuid)|false|none|none|
|navigationCategoryDepth|integer(int64)|false|none|none|
|footerCategoryId|string(uuid)|false|none|none|
|footerCategoryVersionId|string(uuid)|false|none|none|
|serviceCategoryId|string(uuid)|false|none|none|
|serviceCategoryVersionId|string(uuid)|false|none|none|
|mailHeaderFooterId|string(uuid)|false|none|none|
|hreflangDefaultDomainId|string(uuid)|false|none|none|
|name|string|true|none|none|
|shortName|string|false|none|none|
|taxCalculationType|string|false|none|none|
|accessKey|string|true|none|none|
|configuration|object|false|none|none|
|active|boolean|false|none|none|
|hreflangActive|boolean|false|none|none|
|maintenance|boolean|false|none|none|
|maintenanceIpWhitelist|[any]|false|none|none|
|customFields|object|false|none|none|
|paymentMethodIds|[string]|false|read-only|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|translated|object|false|none|none|
|currencies|[currency_flat](/schema/currency_flat)|false|none|Added since version: 6.0.0.0|
|languages|[language_flat](/schema/language_flat)|false|none|Added since version: 6.0.0.0|
|countries|[country_flat](/schema/country_flat)|false|none|Added since version: 6.0.0.0|
|paymentMethods|[payment_method_flat](/schema/payment_method_flat)|false|none|Added since version: 6.0.0.0|
|shippingMethods|[shipping_method_flat](/schema/shipping_method_flat)|false|none|Added since version: 6.0.0.0|
|type|[sales_channel_type_flat](/schema/sales_channel_type_flat)|false|none|Added since version: 6.0.0.0|
|language|[language_flat](/schema/language_flat)|false|none|Added since version: 6.0.0.0|
|customerGroup|[customer_group_flat](/schema/customer_group_flat)|false|none|Added since version: 6.0.0.0|
|currency|[currency_flat](/schema/currency_flat)|false|none|Added since version: 6.0.0.0|
|paymentMethod|[payment_method_flat](/schema/payment_method_flat)|false|none|Added since version: 6.0.0.0|
|shippingMethod|[shipping_method_flat](/schema/shipping_method_flat)|false|none|Added since version: 6.0.0.0|
|country|[country_flat](/schema/country_flat)|false|none|Added since version: 6.0.0.0|
|orders|[order_flat](/schema/order_flat)|false|none|Added since version: 6.0.0.0|
|domains|[sales_channel_domain_flat](/schema/sales_channel_domain_flat)|false|none|Added since version: 6.0.0.0|
|systemConfigs|[system_config_flat](/schema/system_config_flat)|false|none|Added since version: 6.0.0.0|
|navigationCategory|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
|footerCategory|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
|serviceCategory|[category_flat](/schema/category_flat)|false|none|Added since version: 6.0.0.0|
|productVisibilities|[product_visibility_flat](/schema/product_visibility_flat)|false|none|Added since version: 6.0.0.0|
|hreflangDefaultDomain|[sales_channel_domain_flat](/schema/sales_channel_domain_flat)|false|none|Added since version: 6.0.0.0|
|mailHeaderFooter|[mail_header_footer_flat](/schema/mail_header_footer_flat)|false|none|Added since version: 6.0.0.0|
|newsletterRecipients|[newsletter_recipient_flat](/schema/newsletter_recipient_flat)|false|none|Added since version: 6.0.0.0|
|mailTemplates|[mail_template_sales_channel_flat](/schema/mail_template_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|numberRangeSalesChannels|[number_range_sales_channel_flat](/schema/number_range_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|promotionSalesChannels|[promotion_sales_channel_flat](/schema/promotion_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|documentBaseConfigSalesChannels|[document_base_config_sales_channel_flat](/schema/document_base_config_sales_channel_flat)|false|none|Added since version: 6.0.0.0|
|productReviews|[product_review_flat](/schema/product_review_flat)|false|none|Added since version: 6.0.0.0|
|seoUrls|[seo_url_flat](/schema/seo_url_flat)|false|none|Added since version: 6.0.0.0|
|seoUrlTemplates|[seo_url_template_flat](/schema/seo_url_template_flat)|false|none|Added since version: 6.0.0.0|
|mainCategories|[main_category_flat](/schema/main_category_flat)|false|none|Added since version: 6.1.0.0|
|analytics|[sales_channel_analytics_flat](/schema/sales_channel_analytics_flat)|false|none|Added since version: 6.2.0.0|
|customerGroupsRegistrations|[customer_group_flat](/schema/customer_group_flat)|false|none|Added since version: 6.0.0.0|
|wishlists|[customer_wishlist_flat](/schema/customer_wishlist_flat)|false|none|Added since version: 6.3.4.0|
