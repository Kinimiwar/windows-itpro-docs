<!-- ## Allow sideloading of Extensions
>*Supported versions: Microsoft Edge on Windows 10, next major version*<br> -->
>*Default setting: Enabled (Allowed)*

[!INCLUDE [allow-sideloading-of-extensions-shortdesc](../shortdesc/allow-sideloading-of-extensions-shortdesc.md)]

### Supported values

|Group Policy  |MDM |Registry |Description |Most restricted |
|---|:---:|:---:|---|:---:|
|Disabled or not configured |0 |0 |Prevented/not allowed. Disabling does not prevent sideloading of extensions using Add-AppxPackage via PowerShell. To prevent this, enable **Allows development of Windows Store apps and installing them from an integrated development environment (IDE)** policy, located at Windows Components > App Package Deployment.<p>For the MDM setting, set the **ApplicationManagement/AllowDeveloperUnlock** policy to 1 (enabled). |![Most restricted value](../images/check-gn.png) |
|Enabled<br>**(default)** |1 |1 |Allowed. | |
---

### ADMX info and settings

#### ADMX info
- **GP English name:** Allow sideloading of Extensions
- **GP name:** AllowSideloadingOfExtensions
- **GP path:** Windows Components/Microsoft Edge
- **GP ADMX file name:** MicrosoftEdge.admx

#### MDM settings
- **MDM name:** Browser/[AllowSideloadingExtensions](../new-policies.md#allow-sideloading-of-extensions)
- **Supported devices:** Desktop 
- **URI full path:** ./Vendor/MSFT/Policy/Config/Browser/AllowSideloadingExtensions 
- **Data type:** Integer

#### Registry settings
- **Path:** HLKM\Software\Policies\Microsoft\MicrosoftEdge\Extensions 
- **Value name:** AllowSideloadingOfExtensions
- **Value type:** REG_DWORD

### Related policies

- [Allows development of Windows Store apps and installing them from an integrated development environment (IDE)](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-applicationmanagement#applicationmanagement-allowdeveloperunlock): When you enable this policy and the **Allow all trusted apps to install** policy, you allow users to develop Windows Store apps and install them directly from an IDE.

- [Allow all trusted apps to install](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-applicationmanagement#applicationmanagement-allowalltrustedapps): When you enable this policy, you can manage the installation of trusted line-of-business (LOB) or developer-signed Windows Store apps.

### Related topics

[Enable your device for development](https://docs.microsoft.com/en-us/windows/uwp/get-started/enable-your-device-for-development): Access development features, along with other developer-focused settings to make it possible for you to develop, test, and debug apps. Learn how to configure your environment for development, the difference between Developer Mode and sideloading, and the security risks of Developer mode. 

<hr>