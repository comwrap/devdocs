Attribute |  Data Type | Description
--- | --- | ---
`applied_coupon` | [`AppliedCoupon`][AppliedCoupon] | The `AppliedCoupon` object contains the `code` text attribute, which specifies the coupon code
`applied_gift_cards` | [[`AppliedGiftCard`]][AppliedGiftCard] | An array of `AppliedGiftCard` objects. An `AppliedGiftCard` object contains the `code` text attribute, which specifies the gift card code. `applied_gift_cards` is a Commerce-only attribute, defined in the GiftCardAccountGraphQl module
`applied_store_credit` | [`AppliedStoreCredit`][AppliedStoreCredit] | Contains store credit information applied to the cart. `applied_store_credit` is a Commerce-only attribute, defined in the CustomerBalanceGraphQl module
`available_payment_methods` | [AvailablePaymentMethod][AvailablePaymentMethod] | Available payment methods
`billing_address` | [BillingCartAddress][BillingCartAddress] | Contains the billing address specified in the customer's cart
`email` | String | The customer's email address
`items` | [CartItemInterface][CartItemInterface] | Contains the items in the customer's cart
`prices` | [CartPrices][CartPrices] | Contains subtotals and totals
`selected_payment_method` | [SelectedPaymentMethod][SelectedPaymentMethod] | Selected payment method
`shipping_addresses` | [ShippingCartAddress][ShippingCartAddress] | Contains one or more shipping addresses

[AppliedCoupon]: {{page.baseurl}}/graphql/reference/quote.html#AppliedCoupon
[AppliedGiftCard]: {{page.baseurl}}/graphql/reference/quote.html#AppliedGiftCard
[AppliedStoreCredit]: {{page.baseurl}}/graphql/reference/quote.html#AppliedStoreCredit
[AvailablePaymentMethod]: {{page.baseurl}}/graphql/reference/quote.html#AvailablePaymentMethod
[BillingCartAddress]: {{page.baseurl}}/graphql/reference/quote.html#BillingCartAddress
[CartItemInterface]: {{page.baseurl}}/graphql/reference/quote.html#CartItemInterface
[CartPrices]: {{page.baseurl}}/graphql/reference/quote.html#CartPrices
[SelectedPaymentMethod]: {{page.baseurl}}/graphql/reference/quote.html#SelectedPaymentMethod
[ShippingCartAddress]: {{page.baseurl}}/graphql/reference/quote.html#ShippingCartAddress
