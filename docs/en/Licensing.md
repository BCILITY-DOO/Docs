# **License Management**
The main purpose of this app is to help you with managing licenses for all of your different apps. This guide will show you how to use it.

### **Licenses page**
![img](..\assets\Licensing\LicensesPage.png)
This page displays data on all licenses and apps used by your customers, Including some data regarding their environment. Licenses are made to be one license per environment. You don't have to populate all of this data it is automatically populated by the app when the customer checks wether or not their license is valid. The main things you wil be changing here are the "expiration date" and "active" fields. If you ever need to manually populate license data you need to start with the App and Tenant guid fields at the end of the page. At the top of this page you have actions that will open the other pages from this app.
### **App License Setups**
![img](..\assets\Licensing\AppLicenseSetupsPage.png)
App License Setups provides additional information about all the apps you've created. Here, you can define the free trial duration and specify which environments the app is free to use in. You don't need to manually populate all the licensing data on this page before publishing your app—this information will be automatically filled in by the Licensing Management App when a customer attempts to validate their license. The default values for "Is Sandbox Free", "Free Trial Length", and "Is App Free" can be adjusted later in the License Management Setup page.
### **Customer Tenant Mapping**
![img](..\assets\Licensing\CustomerTenantMappingPage.png)
This page contains necessary data about your customers's tenants. Just like the previous 2 pages if an unknown tenant tries to validate their license their data will automatically populate this page, the only thing you wil need to do is specify which customer uses this tenant by populating the "No" field. The tenant names that are shown on the licenses page are taken from this table.
### **License Management Setup**
![img](..\assets\Licensing\LicenseManagementSetupPage.png)
On this page, you can configure the default license values that are applied when a license is first created by the app.