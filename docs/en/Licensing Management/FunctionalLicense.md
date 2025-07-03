# **Functional License Management**

This guide explains how to use our ***License management application***.

## **1. License Management Setup Page**

![img](../../assets/Licensing/LicenceManagementSetupPage.png)

In the **New Extension Defaults** section, you can define the default license parameters that are automatically applied when a new license is created through the application. This ensures consistency and saves time by pre-populating key fields with standardized values.

In the **License List Setup** section, you can configure the visual indicators—specifically, the conditions under which licenses are highlighted in green on the **License List page**. This visual cue helps users quickly identify licenses that meet specific criteria, enhancing usability and streamlining license management.

## **2. App License Setup Page**

![img](../../assets/Licensing/AppLicenseSetupsPage.png)

*Extension Setup* offers information about the licenses for your extensions. You can use this section to set the free trial duration and define which environments the extension can be used in for free.

You don't need to manually populate all the licensing data on this page before publishing your app—this information will be automatically filled in by the *Licensing Management App* when a customer attempts to validate their license. The default values for "Is Sandbox Free", "Free Trial Length" and "Is App Free" can be adjusted later in the *License Management Setup* page.

## **3. Customer Tenant Mapping Page**

![img](../../assets/Licensing/CustomerTenantMappingPage.png)

This page contains necessary data about your **customers' tenants**. Just like the previous 2 pages, if an unknown tenant tries to validate their license, their data will automatically populate this page, the only thing you will need to do is *specify which customer uses this tenant by populating the "No" field*.

## **4. Tenants Page**

![img](../../assets/Licensing/TenantsList.png)

This page shows you data about the tenants your customers use. Just like the previous pages, if an unknown tenant tries to validate their license, the data will automatically populate this page. You can access this page by clicking on the tenant name on the *Licenses page*.

The action at the top of the page will open the *Licenses*, *Environment list* and *Company list* pages respectively. The *Environment list* and *Company list* pages show you more detailed data about your customers.

## **5. When Licenses Are Active**

The primary factor that determines whether a license is active is the **expiration date**. However, **if the expiration date is empty, the license is considered perpetual, and its status is determined by the "active"** field. There are a few exceptions to these rules:

- **Expired licenses** –  If the expiration date is in the past, the license is inactive—regardless of the "active" field value. This status is updated the next time the customer attempts to validate the license.

- **Free apps** – If the app is designated as free in the extension setup, the license remains active even if the expiration date has passed or the "active" field is false. This status is also refreshed upon the next validation attempt.
  
## **6. Licenses Page**

![img](../../assets/Licensing/LicensesPage.png)

This page displays data on all licenses and apps used by your customers, including some data regarding their environment.

 ***Licenses are made to be one license per environment***. You don't have to populate this data—it is automatically populated by the app when the customer tries to validate their license. The main fields you'll typically modify here are **expiration date** and **active**, because *they control whether the license is active*.
 
On the right side of the page you can find a fact box that shows you more detailed data from all companies from the related environment.

The actions at the top of the page open the *Extension Setup*, *Customer Tenant Mapping* and *License Management Setup* pages.