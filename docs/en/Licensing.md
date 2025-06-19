# **License Management**
The main purpose of this app is to help you with managing licenses for all of your different apps. This guide will show you how to use it.

### **Licenses page**
![img](..\assets\Licensing\LicensesPage.png)
This page displays data on all licenses and apps used by your customers, including some data regarding their environment. *Licenses are made to be one license per environment*.

You don't have to populate all of this data—it is automatically populated by the app when the customer checks whether or not their license is valid. The main fields you'll typically modify here are **"expiration date"** and **"active"**, because *they control whether or not the license is active*.

If you ever need to manually populate license data you need to start with the App and Tenant guid fields at the end of the page. 

### **App License Setups**
![img](..\assets\Licensing\AppLicenseSetupsPage.png)
App License Setups offers detailed information about the licenses for your created apps. You can use this section to set the free trial duration and define which environments the app can be used in for free. 

You don't need to manually populate all the licensing data on this page before publishing your app—this information will be automatically filled in by the Licensing Management App when a customer attempts to validate their license. The default values for "Is Sandbox Free", "Free Trial Length" and "Is App Free" can be adjusted later in the License Management Setup page.
### **Customer Tenant Mapping**
![img](..\assets\Licensing\CustomerTenantMappingPage.png)
This page contains necessary data about your **customers tenants**. Just like the previous 2 pages if an unknown tenant tries to validate their license their data will automatically populate this page, the only thing you will need to do is *specify which customer uses this tenant by populating the "No" field*. 

The tenant names that are shown on the licenses page are taken from this table.
### **License Management Setup**
![img](..\assets\Licensing\LicenseManagementSetupPage.png)
On this page, you can configure the default license values that are applied when a license is first created by the app.
## **When Licenses Are Active**
Active licenses are those where the **"active"** field is set to true, with a few exceptions:

**Expired licenses** – If the license's expiration date is before today's date, it is considered inactive, even if the "active" field is true. This status will be updated the next time the customer attempts to validate the license.

**Free apps** – If the app is marked as free in its license configuration, the license may appear active but isn't, it will be updated upon the customer's next validation attempt.

An active license with no expiration date is treated as a lifetime license.