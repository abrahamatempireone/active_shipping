# ActiveShipping CHANGELOG

### v0.10.1

 - Canada Post PWS: Makes wrapper act more consistently with the rest of the API [jnormore]
 - UPS: Adds insurance charge to package object declarations [pbonnell]
 - USPS: Improves how unavailable delivery information is handled [cyu]
 - Shipment Packer: Prevents packing errors and consistently return an array when packing [christianblais]
 - General: Improves tests such that they work with ruby 2.0 [Sirupsen]

### 2011/04/21

* USPS updated to use new APIs [james]
* new :gift boolean option for Package [james]
* Location's :address_type can be "po_box" [james]

### Earlier

* New Zealand Post [AbleTech]
* Include address name for rate requests to Shipwire if provided [dennis]
* Add support for address name to Location [dennis]
* Add fix for updated USPS API to strip any encoded html and trailing asterisks from rate names [dennis]
* Add carrier CanadaPost [william]
* Update FedEx rates and added ability to auto-generate rate name from code that gets returned by FedEx [dennis]
* Assume test_helper is in load path when running tests [cody]
* Add support Kunaki rating service [cody]
* Require active_support instead of activesupport to avoid deprecation warning in Rails 2.3.5 [cody]
* Remove ftools for Rails 1.9 compatibility and remove xml logging, as logging is now included in the connection [cody]
* Update connection code from ActiveMerchant [cody]
* Fix space-ridden USPS usernames when validating credentials [james]
* Remove extra slash from USPS URLs [james]
* Update Shipwire endpoint hostname [cody]
* Add missing ISO countries [Edward Ocampo-Gooding]
* Add support for Guernsey to country.rb [cody]
* Use :words_connector instead of connector in RequiresParameters [cody]
* Fix extra slash in UPS endpoints [cody]
* Add name to Shipwire class [cody]
* Improve FedEx handling of some error conditions [cody]
* Add support for validating credentials to Shipwire [cody]
* Add support for ssl_get to PostsData. Update Carriers to use PostsData module. Turn on retry safety for carriers [cody]
* Add support for Shipwire Shipping Rate API [cody]
* Cleanup package tests [cody]
* Remove unused Carrier#setup method [cody]
* Don't use Array splat in Regex comparisons in Package [cody]
* Default the Location to use the :alpha2 country code format [cody]
* Add configurable timeouts from Active Merchant [cody]
* Update xml_node.rb from XML Node [cody]
* Update requires_parameters from ActiveMerchant [cody]
* Sync posts_data.rb with ActiveMerchant [cody]
* Don't use credentials fixtures in local tests [cody]
