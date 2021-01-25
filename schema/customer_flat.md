
# customer_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|groupId|string(uuid)|true|none|none|
|defaultPaymentMethodId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|languageId|string(uuid)|true|none|none|
|lastPaymentMethodId|string(uuid)|false|none|none|
|defaultBillingAddressId|string(uuid)|true|none|none|
|defaultShippingAddressId|string(uuid)|true|none|none|
|autoIncrement|integer(int64)|false|read-only|none|
|customerNumber|string|true|none|none|
|salutationId|string(uuid)|true|none|none|
|firstName|string|true|none|none|
|lastName|string|true|none|none|
|company|string|false|none|none|
|email|string|true|none|none|
|title|string|false|none|none|
|vatIds|[string]|false|none|none|
|affiliateCode|string|false|none|none|
|campaignCode|string|false|none|none|
|active|boolean|false|none|none|
|doubleOptInRegistration|boolean|false|none|none|
|doubleOptInEmailSentDate|string(date-time)|false|none|none|
|doubleOptInConfirmDate|string(date-time)|false|none|none|
|hash|string|false|none|none|
|guest|boolean|false|none|none|
|firstLogin|string(date-time)|false|none|none|
|lastLogin|string(date-time)|false|none|none|
|newsletter|boolean|false|none|none|
|birthday|string|false|none|none|
|lastOrderDate|string(date-time)|false|read-only|none|
|orderCount|integer(int64)|false|read-only|none|
|customFields|object|false|none|none|
|remoteAddress|string|false|none|none|
|tagIds|[string]|false|read-only|none|
|requestedGroupId|string(uuid)|false|none|none|
|boundSalesChannelId|string(uuid)|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|group|[customer_group_flat](/schema/customer_group_flat)|false|none|Added since version: 6.0.0.0|
|defaultPaymentMethod|[payment_method_flat](/schema/payment_method_flat)|false|none|Added since version: 6.0.0.0|
|language|[language_flat](/schema/language_flat)|false|none|Added since version: 6.0.0.0|
|lastPaymentMethod|[payment_method_flat](/schema/payment_method_flat)|false|none|Added since version: 6.0.0.0|
|defaultBillingAddress|[customer_address_flat](/schema/customer_address_flat)|false|none|Added since version: 6.0.0.0|
|defaultShippingAddress|[customer_address_flat](/schema/customer_address_flat)|false|none|Added since version: 6.0.0.0|
|salutation|[salutation_flat](/schema/salutation_flat)|false|none|Added since version: 6.0.0.0|
|addresses|[customer_address_flat](/schema/customer_address_flat)|false|none|Added since version: 6.0.0.0|
|tags|[tag_flat](/schema/tag_flat)|false|none|Added since version: 6.0.0.0|
|promotions|[promotion_flat](/schema/promotion_flat)|false|none|Added since version: 6.0.0.0|
|productReviews|[product_review_flat](/schema/product_review_flat)|false|none|Added since version: 6.0.0.0|
|recoveryCustomer|[customer_recovery_flat](/schema/customer_recovery_flat)|false|none|Added since version: 6.1.0.0|
|requestedGroup|[customer_group_flat](/schema/customer_group_flat)|false|none|Added since version: 6.0.0.0|
|wishlists|[customer_wishlist_flat](/schema/customer_wishlist_flat)|false|none|Added since version: 6.3.4.0|
