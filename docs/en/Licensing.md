# **License Management**
The main purpose of this app is to help you with managing licenses for all of your different apps. This guide will show you how to use it.

### **Licenses page**
![img](..\assets\Licensing\LicensesPage.png)
This page displays data on all licenses and apps used by your customers, Including some data regarding their environment. Licenses are made to be one license per environment. You don't have to populate all of this data it is automatically populated by the app when the customer checks wether or not their license is valid. The main things you wil be changing here are the "expiration date" and "active" fields. At the top of this page you have actions that will open the other pages form this app.
### **App License Setups**
![img](..\assets\Licensing\AppLicenseSetupsPage.png)
App License Setups contains additional data about all the apps you have made. Here you can specify the length of the free trial and on what types of environments the app is free. You don't have to worry about making sure that all the app data is populated on this page before you publish your app because the licensing management app will automatically populate it when your customer tries to validate their license. The initial values for the "Is Sandbox Free", "Free Trial Length" and "is App Free" fields can be changed on the License Management Setup page. 
### **Customer Tenant Mapping**
![img](..\assets\Licensing\CustomerTenantMappingPage.png)
This page contains necessary data about your customers's tenants. Just like the previous 2 pages if an unknown tenant tries to validate their license their data will automatically populate this page the only thing you wil need to do is specify which customer uses this tenant by populating the "No" field.
### **License Management Setup**
![img](..\assets\Licensing\LicenseManagementSetupPage.png)
On this page you can change the initial values of licenses they are inserted for the first time by the app. 