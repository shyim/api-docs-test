
# order_flat

{% hint style="info" %}

Added since version: 6.0.0.0

{% endhint %}

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string(uuid)|false|none|none|
|versionId|string(uuid)|false|none|none|
|autoIncrement|integer(int64)|false|read-only|none|
|orderNumber|string|false|none|none|
|billingAddressId|string(uuid)|true|none|none|
|billingAddressVersionId|string(uuid)|false|none|none|
|currencyId|string(uuid)|true|none|none|
|languageId|string(uuid)|true|none|none|
|salesChannelId|string(uuid)|true|none|none|
|orderDateTime|string(date-time)|true|none|none|
|orderDate|string|false|read-only|none|
|price|object|false|none|none|
|» netPrice|number(float)|true|none|none|
|» totalPrice|number(float)|true|none|none|
|» calculatedTaxes|object|false|none|none|
|» taxRules|object|false|none|none|
|» positionPrice|number(float)|true|none|none|
|» taxStatus|string|true|none|none|
|amountTotal|number(float)|false|read-only|none|
|amountNet|number(float)|false|read-only|none|
|positionPrice|number(float)|false|read-only|none|
|taxStatus|string|false|read-only|none|
|shippingCosts|object|false|none|none|
|» unitPrice|number(float)|true|none|none|
|» totalPrice|number(float)|true|none|none|
|» quantity|integer(int64)|true|none|none|
|» calculatedTaxes|object|false|none|none|
|» taxRules|object|false|none|none|
|» referencePrice|object|false|none|none|
|» listPrice|object|false|none|none|
|»» price|number(float)|false|none|none|
|»» discount|number(float)|false|none|none|
|»» percentage|number(float)|false|none|none|
|shippingTotal|number(float)|false|read-only|none|
|currencyFactor|number(float)|true|none|none|
|deepLinkCode|string|false|none|none|
|affiliateCode|string|false|none|none|
|campaignCode|string|false|none|none|
|customerComment|string|false|none|none|
|stateId|string(uuid)|true|none|none|
|ruleIds|[string]|false|none|none|
|customFields|object|false|none|none|
|createdAt|string(date-time)|true|read-only|none|
|updatedAt|string(date-time)|false|read-only|none|
|stateMachineState|[state_machine_state_flat](/schema/state_machine_state_flat.md)|false|none|Added since version: 6.0.0.0|
|orderCustomer|[order_customer_flat](/schema/order_customer_flat.md)|false|none|Added since version: 6.0.0.0|
|currency|[currency_flat](/schema/currency_flat.md)|false|none|Added since version: 6.0.0.0|
|language|[language_flat](/schema/language_flat.md)|false|none|Added since version: 6.0.0.0|
|addresses|[order_address_flat](/schema/order_address_flat.md)|false|none|Added since version: 6.0.0.0|
|billingAddress|[order_address_flat](/schema/order_address_flat.md)|false|none|Added since version: 6.0.0.0|
|deliveries|[order_delivery_flat](/schema/order_delivery_flat.md)|false|none|Added since version: 6.0.0.0|
|lineItems|[order_line_item_flat](/schema/order_line_item_flat.md)|false|none|Added since version: 6.0.0.0|
|transactions|[order_transaction_flat](/schema/order_transaction_flat.md)|false|none|Added since version: 6.0.0.0|
|documents|[document_flat](/schema/document_flat.md)|false|none|Added since version: 6.0.0.0|
|tags|[tag_flat](/schema/tag_flat.md)|false|none|Added since version: 6.0.0.0|
