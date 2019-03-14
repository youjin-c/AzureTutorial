# Prerequisite
PC, VR/MR headset(or just a headset), Unity(2017.4) installed, Azure account[Sign up for Azure FREE trial](https://azure.microsoft.com/en-us/free/)
# Access 'Mixed Reality' settings on Windows 10
1. Use the **Windows key + R** keyboard shortcut to open the **Run** command.<br/>
2. Type **regedit**, and click **OK** to open the **Registry**.<br/>
3. Browse the following path:<br/>
```HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Holographic```<br/>
Right-click the **Holographic** (folder) key, select **New** and click on **DWORD (32-bit) Value**.<br/>
4. Name the key **FirstRunSucceeded** and press **Enter**.<br/>
5. Double-click the newly created key and change its value from **0** to **1**.<br/>
    **Quick Tip**: If you want to remove the "Mixed Reality" section from the Settings app, you can leave the **FirstRunSucceeded** key with the default value of **0**.<br/>
    Click **OK**.




![CreateResource](/azure000.jpg)
![CreateResource](/azure001.png)
Choose a Resource Group or create a new one.<br/> 
A resource group provides a way to monitor, control access, provision and manage billing for a collection of Azure assets.<br/>
It is recommended to keep all the Azure services associated with a single project  under a common resource group.<br/>
Sign in Luis.ai with the same credential with MS Azure.<br/>


- *Intent*, represents the method that will be called following a query from the user. <br/>
- An *INTENT* may have one or more *ENTITIES*.<br/>
- *Entity*, is a component of the query that describes information relevant to the *INTENT*.<br/>
- *Utterances*, are examples of queries provided by the developer, that LUIS will use to train itself.<br/>
