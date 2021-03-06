---
group: graphql
title: giftCardAccount query
ee_only: True
---

The `giftCardAccount` query returns information for a specific gift card.

## Syntax

 `giftCardAccount(code: String!): GiftCardAccount`

## Example usage

The following example returns information about the `01PNC9L76H4H` gift card code.

**Request**

``` text
query {
  giftCardAccount(input: {gift_card_code: "01PNC9L76H4H"}){
    code
    balance {
      currency
      value
    }
    expiration_date
  }
}
```

**Response**

```json
{
  "data": {
    "giftCardAccount": {
      "code": "01PNC9L76H4H",
      "balance": {
        "currency": "USD",
        "value": 25
      },
      "expiration_date": null
    }
  }
}
```

## Input attributes

The `giftCardAccount` query requires the `gift_card_code`.

### GiftCardAccount object {#GiftCardAccount}

The `GiftCardAccount` object must contain the following attribute:

Attribute | Data Type | Description
--- | --- | ---
`gift_card_code` | String! | The gift card code

## Output attributes

The `GiftCardAccount` object returns the following attributes:

Attribute |  Data Type | Description
--- | --- | ---
`balance` | Money | Returns the currency and remaining balance of the gift card
`code` | String | Returns the gift card code
`expiration_date` | String | Returns the date when the gift card expires, if any
