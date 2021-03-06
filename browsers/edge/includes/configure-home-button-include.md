<!-- ## Configure Home Button
>*Supported versions: Microsoft Edge on Windows 10*<br> -->
>*Default setting: Disabled or not configured (Show home button and load the Start page)*


[!INCLUDE [configure-home-button-shortdesc](../shortdesc/configure-home-button-shortdesc.md)]


### Supported values

|Group Policy  |MDM |Registry |Description |
|---|:---:|:---:|---|
|Disabled or not configured<br>**(default)** |0 |0 |Show home button and load the Start page. |
|Enabled |1 |1 |Show home button and load the New tab page. |
|Enabled |2 |2 |Show home button and load the custom URL defined in the Set Home Button URL policy. |
|Enabled |3 |3 |Hide home button. |
---

>[!TIP]
>If you want to make changes to this policy:<ol><li>Enable the **Unlock Home Button** policy.</li><li>Make changes to the **Configure Home Button** policy or **Set Home Button URL** policy.</li><li>Disable the **Unlock Home Button** policy.</li></ol>



### Configuration options

![Show home button and load Start page or New tab page](../images/home-button-start-new-tab-page-v4-sm.png)

![Show home button and load custom URL](../images/home-buttom-custom-url-v4-sm.png)

![Hide home button](../images/home-button-hide-v4-sm.png)

### ADMX info and settings
#### ADMX info
- **GP English name:** Configure Home Button
- **GP name:** ConfigureHomeButton
- **GP element:** ConfigureHomeButtonDropdown
- **GP path:** Windows Components/Microsoft Edge
- **GP ADMX file name:** MicrosoftEdge.admx

#### MDM settings
- **MDM name:** Browser/[ConfigureHomeButton](../new-policies.md#configure-home-button)
- **Supported devices:** Desktop and Mobile
- **URI full path:** ./Vendor/MSFT/Policy/Config/Browser/ConfigureHomeButton 
- **Data type:** Integer

#### Registry settings
- **Path:** HLKM\Software\Policies\Microsoft\MicrosoftEdge\Internet Settings 
- **Value name:** ConfigureHomeButton
- **Value type:** REG_DWORD

### Related policies

- [Set Home button URL](../new-policies.md#set-home-button-url): [!INCLUDE [set-home-button-url-shortdesc](../shortdesc/set-home-button-url-shortdesc.md)]
 
- [Unlock Home button](../new-policies.md#unlock-home-button): [!INCLUDE [unlock-home-button-shortdesc](../shortdesc/unlock-home-button-shortdesc.md)] 


<hr>