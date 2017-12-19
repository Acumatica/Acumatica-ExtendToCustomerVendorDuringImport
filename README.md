[![Project Status](http://opensource.box.com/badges/active.svg)](http://opensource.box.com/badges)

Automate Extend To Customer and/or Vendor via Import Scenario 
==================================
An Extension that allows to automate Extend To Customer/Vendor during Import.

Out-of-box Extend To Vendor or Extend To Customer actions cannot be used in Import Scenario since it redirects to vendor and customer screen respectively with pre-populated data and user has to manually save the vendor.

In this customization, we are creating a new hidden actions which invokes base action and persists the data rather redirecting to screen.

### Prerequisites
* Acumatica 6.10 or higher

Quick Start
-----------

### Installation

##### Install the customization deployment package
1. Download PXExtendToCustomerAndVendor.zip from this repository
2. In your Acumatica ERP instance, navigate to System -> Customization -> Customization Projects (SM204505), import PXExtendToCustomerAndVendor.zip as a customization project
3. Publish the customization project.

### Usage

After publishing the customization,
1. Modify Import Scenario for Customers (SM206025) and add new Extend To Vendor Ext action after Save Action.
![Screenshot](/_ReadMeImages/SM206025IC.png)
2. Modify Import Scenario for Vendors (SM206025) and add new Extend To Customer Ext action after Save Action.
![Screenshot](/_ReadMeImages/SM206025IV.png)

Customization Package exposes the similar hidden actions for Business Account (CR303000) as well which can be used similarly in Import Scenario to convert to Customer and/or Vendor while importing Business Accounts.

Known Issues
------------
None at the moment

## Copyright and License

Copyright © `2017` `Acumatica`

This component is licensed under the MIT License, a copy of which is available online [here](LICENSE.md)
