# appsflyer-to-aki-prototype
appflyer-to-aki-prototype


# AppsFlyer Task 1:

Confirm appsflyer is capturing and able to send the below data on all app and web customers. Specifically: 

* β PageTitle -> (* Possibly "EVENT_NAME")
* β IdentifierCanonical -> ?
* β UrlCanonical -> ?
* β SearchKeywords -> ?
* π CategoryName -> D.N.E.
* β ProductSKU -> ?
* π ProductName -> D.N.E.
* π ProductBrand -> D.N.E.
* π ProductCategory -> D.N.E.
* π OrderItemQuantity -> D.N.E.
* β OrderItemPrice "EVENT_VALUE:af_price"
* π OrderShippingMode -> D.N.E.
* π OrderShippingPrice -> D.N.E.
* π OrderShippingTax -> D.N.E.
* π OrderPriceTotal -> D.N.E. (* Note even for "purchase" af events)
* β Currency -> [ "CURRENCY", "SELECTED_CURRENCY", "EVENT_VALUE:af_currency"]
* π DeliveryMode -> D.N.E.
* β AppVersion -> "APP_VERSION"
* β PhoneBrand -> "PLATFORM"
* β PhoneModel -> "DEVICE_MODEL"
* β PhoneLanguage -> "LANGUAGE"
* β PhoneOsVersion -> "OS_VERSION"
* π Screen_dpi -> D.N.E.
* π Screen_height -> D.N.E.
* π Screen_width -> D.N.E.
* β AdvertisingId -> ["IDFA", "EVENT_VALUE:af_customer_id", "CUSTOMER_USER_ID", "APPSFLYER_ID"]

# AppsFlyer Task 2:

Investigate whether weβre able to block appsflyer from sending any data to Aki for iOS 14.5 consented customers 

# iOS 14.5 Task 1:

[SNOWFLAKE QUERY FOR THAT] Investigate how we can generate a daily report of gopuff shopper iOS 14.5 consent opt-outs tied to their most recent IDFA.

# iOS 14.5 Task 2: 

Investigate how we can send that mapping file to Aki so that they can scrub these shoppers from their list.

We only want to send the list of shoppers whose IDFA was previously shared with Aki via Appsflyer (or another integration)

