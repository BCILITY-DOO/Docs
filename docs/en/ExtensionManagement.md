# Extension Management in Dynamics 365 Business Central

Extension Management in Dynamics 365 Business Central allows organizations to enhance and customize the system by managing add-on applications known as **extensions**. These apps expand the standard functionality of Business Central without changing the core application, making the system flexible, upgrade-friendly, and adaptable to specific business needs.

Extensions can be developed by Microsoft, third-party partners, or internal development teams, and are either distributed through **Microsoft AppSource**, uploaded as **per-tenant extensions (PTEs)**, or created and tested in sandbox environments.

## **1. Accessing Extension Management**

The main hub for managing extensions is the **Extension Management** page. This page can be accessed from the Home screen or by using the "Tell Me" search bar. Once on the page, administrators can view a list of installed extensions, see version details, configure settings, update apps, uninstall them, or explore and install new apps from AppSource.

![img](..\assets\Extensions\extensions1.png)  

From the Extension Management page, it is also possible to monitor system behavior impacted by apps, such as additional fields or pages introduced by extensions, or connections to external services.

## **2. Installing and Updating Extensions**

To install a new app, users can open the **AppSource** marketplace directly from within Business Central. 

![img](..\assets\Extensions\extensions2.png)  

After browsing available solutions, users select an app, accept its terms, and proceed with installation. In many cases, further setup is required after installation—for instance, entering API credentials or configuring data mappings.

Updating extensions is equally straightforward. When updates are available, Business Central will notify users through Extension Management. These updates can be installed manually or as part of a scheduled release plan. It’s good practice to test updates in a sandbox environment before applying them in production.

## **3. Uninstalling and Reinstalling Extensions**

Extensions can be uninstalled at any time via the Extension Management page. 

![img](..\assets\Extensions\extensions3.png)  

If uninstalled, Business Central typically retains any data that was created by the extension. This means that if the app is later reinstalled, the existing data will still be available. However, some apps marked as “required” by Microsoft or partners cannot be removed.

## **4. Extension Types**

There are three primary types of extensions supported in Business Central:

- **AppSource apps** are publicly available, pre-certified solutions published by Microsoft or its partners.
- **Per-tenant extensions (PTEs)** are custom apps built for a specific customer, often by a partner or internal developer.
- **Developer extensions** are created in AL language using Visual Studio Code and are used mainly in sandbox environments for testing and development.

Note that **AppSource apps and PTEs can only be installed in online environments**. On-premises deployments do not support installing AppSource apps from the Extension Management page.

## **5. Permissions and Administration**

Only authorized users can manage extensions. To install or remove apps, a user must either:

- Be part of the `D365 Extension Mgt.` security group, or
- Be assigned the `EXTEN. MGT. - ADMIN` permission set.

These permissions allow access to installation, publishing, configuration, and uninstallation of extensions. Administrators can assign these permissions in the Microsoft 365 Admin Center or directly within Business Central.

## **6. Compliance and Risk Considerations**

Although extensions offer great flexibility, it's important to understand potential risks. Apps from external providers may interact with third-party services, store data outside your organization's region, or access sensitive business data. Always review the privacy policy and compliance information for each extension, especially when using AI-powered features or data-sharing integrations.

Extension functionality may also affect accessibility, interface language, and system performance. For these reasons, businesses are advised to evaluate each extension carefully before installation, and to restrict management access to trusted users.

## **7. Connectivity and Automation Apps**

From the 2022 release wave 2 onward, Business Central introduced **Connectivity Apps** and **Banking Apps** sections within Extension Management. These pages help users find regionally relevant extensions that automate workflows, such as bank reconciliation, document exchange, or cash flow forecasting. When opening these sections for the first time, users are prompted to allow Business Central to connect to external data services to suggest relevant apps.

## **8. Recommended Extensions**

Microsoft partners can also create curated lists of **recommended apps** for their customers. These will appear on a dedicated *Recommended Apps* page within *Extension Management*, making it easy to install extensions that align with industry best practices or a partner’s deployment strategy.

