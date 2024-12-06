# Card Verified

**Title:** Card Verified

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

| Property                                                       | Type    | Title/Description                                                        |
| -------------------------------------------------------------- | ------- | ------------------------------------------------------------------------ |
| + [action_id](#action_id )                                     | string  | The unique identifier of the action                                      |
| + [payment_type](#payment_type )                               | string  | The payment type                                                         |
| - [auth_code](#auth_code )                                     | string  | The authorization code                                                   |
| + [response_code](#response_code )                             | string  | The Gateway response code                                                |
| + [response_summary](#response_summary )                       | string  | The Gateway response summary                                             |
| - [scheme_id](#scheme_id )                                     | string  | The unique identifier of the scheme                                      |
| + [source](#source )                                           | object  | The originating location of the funds for a payment                      |
| - [customer](#customer )                                       | object  | Properties belonging to the customer who requested the payment           |
| - [processing](#processing )                                   | object  | The Processing settings object                                           |
| + [amount](#amount )                                           | integer | The amount in major units                                                |
| - [metadata](#metadata )                                       | object  | Additional data tracked by the merchant in the format of key value pairs |
| - [3ds](#3ds )                                                 | object  | The 3D Secure information                                                |
| + [risk](#risk )                                               | object  | The risk object                                                          |
| + [id](#id )                                                   | string  | The unique identifier of the payment                                     |
| + [currency](#currency )                                       | string  | The currency ISO alpha 3 code                                            |
| + [processed_on](#processed_on )                               | string  | ISO8601 formatted date time (UTC) that the payment was processed on      |
| - [reference](#reference )                                     | string  | The merchant's reference                                                 |
| - [event_links](#event_links )                                 | object  | The Event Links collection object                                        |
| - [upgrade_reason](#upgrade_reason )                           | string  | The 3ds upgrade reason                                                   |
| - [processing_channel_id](#processing_channel_id )             | string  | The processing channel id                                                |
| - [pan_type_processed](#pan_type_processed )                   | string  | The pan type used during authorization                                   |
| - [cko_network_token_available](#cko_network_token_available ) | boolean | Whether a CKO provisioned token is available                             |
| - [](#additionalProperties )                                   | object  | -                                                                        |

## <a name="action_id"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > action_id`

**Title:** The unique identifier of the action

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"act_sdcdhwmpjgberkbzkugqe7pfum"
```

## <a name="payment_type"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > payment_type`

**Title:** The payment type

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"REGULAR"
```

## <a name="auth_code"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > auth_code`

**Title:** The authorization code

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"075867"
```

## <a name="response_code"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > response_code`

**Title:** The Gateway response code

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"10000"
```

## <a name="response_summary"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > response_summary`

**Title:** The Gateway response summary

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"Approved"
```

## <a name="scheme_id"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > scheme_id`

**Title:** The unique identifier of the scheme

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"638284745624527"
```

## <a name="source"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > source`

**Title:** The originating location of the funds for a payment

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

| Property                                                  | Type    | Title/Description                                |
| --------------------------------------------------------- | ------- | ------------------------------------------------ |
| - [id](#source_id )                                       | string  | The unique identifier of the source              |
| + [type](#source_type )                                   | string  | The type of the source                           |
| - [vault_id](#source_vault_id )                           | string  | The unique identifier of the source in the vault |
| - [billing_address](#source_billing_address )             | object  | The Billing address associated to the source     |
| - [expiry_month](#source_expiry_month )                   | integer | The expiry month                                 |
| - [expiry_year](#source_expiry_year )                     | integer | The expiry year                                  |
| - [name](#source_name )                                   | string  | The source name                                  |
| - [scheme](#source_scheme )                               | string  | The card scheme                                  |
| - [last_4](#source_last_4 )                               | string  | The last 4 number of the card                    |
| - [fingerprint](#source_fingerprint )                     | string  | The fingerprint of the source                    |
| - [bin](#source_bin )                                     | string  | The bin number of the card                       |
| - [card_type](#source_card_type )                         | string  | The card type                                    |
| - [card_category](#source_card_category )                 | string  | The card category                                |
| - [card_wallet_type](#source_card_wallet_type )           | string  | The card wallet type                             |
| - [issuer](#source_issuer )                               | string  | The card issuer name                             |
| - [issuer_country](#source_issuer_country )               | string  | The card issuer country                          |
| - [product_id](#source_product_id )                       | string  | The unique identifier of the source product      |
| - [product_type](#source_product_type )                   | string  | The type of the source card                      |
| - [avs_check](#source_avs_check )                         | string  | The result of the AVS check                      |
| - [cvv_check](#source_cvv_check )                         | string  | The result of the CVV check                      |
| - [account_update_status](#source_account_update_status ) | string  | The account update status indicator value        |
| - [account_holder](#source_account_holder )               | object  | Account holder information                       |
| - [](#source_additionalProperties )                       | object  | -                                                |

### <a name="source_id"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > id`

**Title:** The unique identifier of the source

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"src_isu5yyegxg4e5l5yadnpu6y744"
```

### <a name="source_type"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > source > type`

**Title:** The type of the source

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"card"
```

### <a name="source_vault_id"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > vault_id`

**Title:** The unique identifier of the source in the vault

|          |          |
| -------- | -------- |
| **Type** | `string` |

### <a name="source_billing_address"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > billing_address`

**Title:** The Billing address associated to the source

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

| Property                                            | Type   | Title/Description |
| --------------------------------------------------- | ------ | ----------------- |
| - [](#source_billing_address_additionalProperties ) | object | -                 |

### <a name="source_expiry_month"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > expiry_month`

**Title:** The expiry month

|          |           |
| -------- | --------- |
| **Type** | `integer` |

**Example:** 

```json
12
```

### <a name="source_expiry_year"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > expiry_year`

**Title:** The expiry year

|          |           |
| -------- | --------- |
| **Type** | `integer` |

**Example:** 

```json
2025
```

### <a name="source_name"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > name`

**Title:** The source name

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"John Smith"
```

### <a name="source_scheme"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > scheme`

**Title:** The card scheme

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"VISA"
```

### <a name="source_last_4"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > last_4`

**Title:** The last 4 number of the card

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"4242"
```

### <a name="source_fingerprint"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > fingerprint`

**Title:** The fingerprint of the source

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"71580b426f1d190d29087ff265d8f48df1ad34ede41c27cbff9d23c1a14d1776"
```

### <a name="source_bin"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > bin`

**Title:** The bin number of the card

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"424242"
```

### <a name="source_card_type"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > card_type`

**Title:** The card type

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"Credit"
```

### <a name="source_card_category"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > card_category`

**Title:** The card category

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"Consumer"
```

### <a name="source_card_wallet_type"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > card_wallet_type`

**Title:** The card wallet type

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Examples:** 

```json
"googlepay"
```

```json
"applepay"
```

### <a name="source_issuer"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > issuer`

**Title:** The card issuer name

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"JPMORGAN CHASE BANK NA"
```

### <a name="source_issuer_country"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > issuer_country`

**Title:** The card issuer country

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"US"
```

### <a name="source_product_id"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > product_id`

**Title:** The unique identifier of the source product

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"A"
```

### <a name="source_product_type"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > product_type`

**Title:** The type of the source card

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"Visa Traditional"
```

### <a name="source_avs_check"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > avs_check`

**Title:** The result of the AVS check

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"S"
```

### <a name="source_cvv_check"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > cvv_check`

**Title:** The result of the CVV check

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
""
```

### <a name="source_account_update_status"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_update_status`

**Title:** The account update status indicator value

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"card_updated"
```

### <a name="source_account_holder"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_holder`

**Title:** Account holder information

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

| Property                                                               | Type             | Title/Description                      |
| ---------------------------------------------------------------------- | ---------------- | -------------------------------------- |
| - [type](#source_account_holder_type )                                 | enum (of string) | The type of the account holder         |
| - [first_name](#source_account_holder_first_name )                     | string           | The first name of the account holder   |
| - [middle_name](#source_account_holder_middle_name )                   | string           | The middle name of the account holder  |
| - [last_name](#source_account_holder_last_name )                       | string           | The last name of the account holder    |
| - [company_name](#source_account_holder_company_name )                 | string           | The company name of the account holder |
| - [account_name_inquiry](#source_account_holder_account_name_inquiry ) | string           | Account Name Inquiry result            |

#### <a name="source_account_holder_type"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_holder > type`

**Title:** The type of the account holder

|          |                    |
| -------- | ------------------ |
| **Type** | `enum (of string)` |

Must be one of:
* "individual"
* "corporate"
* "government"

#### <a name="source_account_holder_first_name"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_holder > first_name`

**Title:** The first name of the account holder

|          |          |
| -------- | -------- |
| **Type** | `string` |

#### <a name="source_account_holder_middle_name"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_holder > middle_name`

**Title:** The middle name of the account holder

|          |          |
| -------- | -------- |
| **Type** | `string` |

#### <a name="source_account_holder_last_name"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_holder > last_name`

**Title:** The last name of the account holder

|          |          |
| -------- | -------- |
| **Type** | `string` |

#### <a name="source_account_holder_company_name"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_holder > company_name`

**Title:** The company name of the account holder

|          |          |
| -------- | -------- |
| **Type** | `string` |

#### <a name="source_account_holder_account_name_inquiry"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > source > account_holder > account_name_inquiry`

**Title:** Account Name Inquiry result

|          |          |
| -------- | -------- |
| **Type** | `string` |

## <a name="customer"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > customer`

**Title:** Properties belonging to the customer who requested the payment

|                           |                                                                                                          |
| ------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                 |
| **Additional properties** | [![Not allowed](https://img.shields.io/badge/Not%20allowed-red)](# "Additional Properties not allowed.") |

| Property                    | Type   | Title/Description  |
| --------------------------- | ------ | ------------------ |
| - [id](#customer_id )       | string | The Id Schema      |
| - [email](#customer_email ) | string | The customer email |

### <a name="customer_id"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > customer > id`

**Title:** The Id Schema

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"cus_gs47qn23bqmefhkmlpokm7vzxm"
```

### <a name="customer_email"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > customer > email`

**Title:** The customer email

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"John.doe@email.com"
```

## <a name="processing"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > processing`

**Title:** The Processing settings object

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

**Example:** 

```json
{
    "acquirer_transaction_id": "8137549556",
    "retrieval_reference_number": "000007895269"
}
```

| Property                                | Type   | Title/Description |
| --------------------------------------- | ------ | ----------------- |
| - [](#processing_additionalProperties ) | object | -                 |

## <a name="amount"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > amount`

**Title:** The amount in major units

|             |           |
| ----------- | --------- |
| **Type**    | `integer` |
| **Default** | `0`       |

**Example:** 

```json
0
```

## <a name="metadata"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > metadata`

**Title:** Additional data tracked by the merchant in the format of key value pairs

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

| Property                              | Type   | Title/Description |
| ------------------------------------- | ------ | ----------------- |
| - [](#metadata_additionalProperties ) | object | -                 |

## <a name="3ds"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds`

**Title:** The 3D Secure information

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

| Property                                                   | Type    | Title/Description                                                                                                           |
| ---------------------------------------------------------- | ------- | --------------------------------------------------------------------------------------------------------------------------- |
| - [authentication_id](#3ds_authentication_id )             | string  | The unique identifier of the authentication                                                                                 |
| + [downgraded](#3ds_downgraded )                           | boolean | Whether the payment authentication was downgraded                                                                           |
| - [authentication_response](#3ds_authentication_response ) | string  | The authentication response                                                                                                 |
| - [eci](#3ds_eci )                                         | string  | The ECI (E-Commerce Indicator) security level associated with the transaction                                               |
| - [cavv](#3ds_cavv )                                       | string  | The unique Cardholder Authentication Verification Value (CAVV) associated with the transaction, provided by the card issuer |
| - [xid](#3ds_xid )                                         | string  | The unique identifier for the transaction, assigned by the MPI(Merchant Plug-In) (in this case, Secure Trading)             |
| + [version](#3ds_version )                                 | string  | The version of 3ds used                                                                                                     |
| - [enrolled](#3ds_enrolled )                               | string  | Indicates if the card is enrolled with 3DS                                                                                  |
| - [challenge_indicator](#3ds_challenge_indicator )         | string  | Indicates the preference for whether or not a 3DS challenge should be performed                                             |
| - [challenged](#3ds_challenged )                           | boolean | Indicates whether the authentication was challenged                                                                         |
| - [exemption](#3ds_exemption )                             | string  | The exemption reason used so that the payment was not processed using 3D Secure authentication                              |
| - [flow_type](#3ds_flow_type )                             | string  | Indicates whether the 3D Secure 2 authentication was challenged or frictionless                                             |
| - [upgrade_reason](#3ds_upgrade_reason )                   | string  | The reason the payment was upgraded to 3D Secure                                                                            |
| - [redirect_url](#3ds_redirect_url )                       | string  | The 3ds redirect url                                                                                                        |
| - [](#3ds_additionalProperties )                           | object  | -                                                                                                                           |

### <a name="3ds_authentication_id"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > authentication_id`

**Title:** The unique identifier of the authentication

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"sid_isu5yyegxg4e5l5yadnpu6y744"
```

### <a name="3ds_downgraded"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > 3ds > downgraded`

**Title:** Whether the payment authentication was downgraded

|          |           |
| -------- | --------- |
| **Type** | `boolean` |

**Examples:** 

```json
true
```

```json
false
```

### <a name="3ds_authentication_response"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > authentication_response`

**Title:** The authentication response

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Examples:** 

```json
"Y"
```

```json
"N"
```

### <a name="3ds_eci"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > eci`

**Title:** The ECI (E-Commerce Indicator) security level associated with the transaction

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"05"
```

### <a name="3ds_cavv"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > cavv`

**Title:** The unique Cardholder Authentication Verification Value (CAVV) associated with the transaction, provided by the card issuer

|          |          |
| -------- | -------- |
| **Type** | `string` |

### <a name="3ds_xid"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > xid`

**Title:** The unique identifier for the transaction, assigned by the MPI(Merchant Plug-In) (in this case, Secure Trading)

|          |          |
| -------- | -------- |
| **Type** | `string` |

### <a name="3ds_version"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > 3ds > version`

**Title:** The version of 3ds used

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"2.1.0"
```

### <a name="3ds_enrolled"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > enrolled`

**Title:** Indicates if the card is enrolled with 3DS

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"Y"
```

### <a name="3ds_challenge_indicator"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > challenge_indicator`

**Title:** Indicates the preference for whether or not a 3DS challenge should be performed

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Examples:** 

```json
"no_preference"
```

```json
"no_challenge_requested"
```

```json
"challenge_requested"
```

```json
"challenge_requested_mandate"
```

### <a name="3ds_challenged"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > challenged`

**Title:** Indicates whether the authentication was challenged

|          |           |
| -------- | --------- |
| **Type** | `boolean` |

**Example:** 

```json
false
```

### <a name="3ds_exemption"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > exemption`

**Title:** The exemption reason used so that the payment was not processed using 3D Secure authentication

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"low_value"
```

### <a name="3ds_flow_type"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > flow_type`

**Title:** Indicates whether the 3D Secure 2 authentication was challenged or frictionless

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Examples:** 

```json
"frictionless"
```

```json
"challenged"
```

```json
"frictionless_delegated"
```

### <a name="3ds_upgrade_reason"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > upgrade_reason`

**Title:** The reason the payment was upgraded to 3D Secure

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"sca_retry"
```

### <a name="3ds_redirect_url"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > 3ds > redirect_url`

**Title:** The 3ds redirect url

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"https://api.checkout.com/redirect/here"
```

## <a name="risk"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > risk`

**Title:** The risk object

|                           |                                                                                                          |
| ------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                 |
| **Additional properties** | [![Not allowed](https://img.shields.io/badge/Not%20allowed-red)](# "Additional Properties not allowed.") |

| Property                    | Type    | Title/Description                    |
| --------------------------- | ------- | ------------------------------------ |
| - [flagged](#risk_flagged ) | boolean | Whether the payment has been flagged |
| - [score](#risk_score )     | number  | Score determined by Prism            |

### <a name="risk_flagged"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > risk > flagged`

**Title:** Whether the payment has been flagged

|          |           |
| -------- | --------- |
| **Type** | `boolean` |

**Example:** 

```json
false
```

### <a name="risk_score"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > risk > score`

**Title:** Score determined by Prism

|          |          |
| -------- | -------- |
| **Type** | `number` |

**Example:** 

```json
69
```

## <a name="id"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > id`

**Title:** The unique identifier of the payment

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"pay_sdcdhwmpjgberkbzkugqe7pfum"
```

## <a name="currency"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > currency`

**Title:** The currency ISO alpha 3 code

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"EUR"
```

## <a name="processed_on"></a>![Required](https://img.shields.io/badge/Required-blue) Property `Card Verified > processed_on`

**Title:** ISO8601 formatted date time (UTC) that the payment was processed on

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"2019-06-07T08:29:35Z"
```

## <a name="reference"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > reference`

**Title:** The merchant's reference

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"ORD-5023-4E89"
```

## <a name="event_links"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > event_links`

**Title:** The Event Links collection object

|                           |                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Type**                  | `object`                                                                                                                          |
| **Additional properties** | [![Any type: allowed](https://img.shields.io/badge/Any%20type-allowed-green)](# "Additional Properties of any type are allowed.") |

**Example:** 

```json
{
    "payment": "http://api.checkout.com/payment/pay_sdcdhwmpjgberkbzkugqe7pfum",
    "payment_action": "http://api.checkout.com/payment/pay_sdcdhwmpjgberkbzkugqe7pfum/actions"
}
```

| Property                                 | Type   | Title/Description |
| ---------------------------------------- | ------ | ----------------- |
| - [](#event_links_additionalProperties ) | object | -                 |

## <a name="upgrade_reason"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > upgrade_reason`

**Title:** The 3ds upgrade reason

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"sca_retry"
```

## <a name="processing_channel_id"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > processing_channel_id`

**Title:** The processing channel id

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Example:** 

```json
"pc_ubrkt23ju7mu7pcz4yqw4anyxm"
```

## <a name="pan_type_processed"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > pan_type_processed`

**Title:** The pan type used during authorization

|          |          |
| -------- | -------- |
| **Type** | `string` |

**Examples:** 

```json
"dpan"
```

```json
"fpan"
```

## <a name="cko_network_token_available"></a>![Optional](https://img.shields.io/badge/Optional-yellow) Property `Card Verified > cko_network_token_available`

**Title:** Whether a CKO provisioned token is available

|          |           |
| -------- | --------- |
| **Type** | `boolean` |

**Examples:** 

```json
"true"
```

```json
"false"
```

----------------------------------------------------------------------------------------------------------------------------
