
# Quick-start for Installing and Using ownCloud

> ## Index

| Task Title           | Task Number    |
|---------------|---------------:|
| Install and configure an Owncloud server as an administrator|1|
| Virtual Machine (VM) Installation| 1.1    |
| Install and configure an ownCloud server| 1.2    |
| Enable users to connect to the ownCloud server using the server's IP address and port 8080| 2   |
| Installing Ubuntu 20.04 OS in Virtual Box VM| 2.1   |
| IP address and port 8080 configuration| 2.2    |
| Adding User Account in the ownCloud Server| 3    |
| Connecting ownCloud server by using a desktop or mobile client| 4    |
| Connecting ownCloud server by using a desktop client| 4.1    |
| Connecting ownCloud server by using a mobile client| 4.2    |

##  1. Install and configure an Owncloud server as an administrator

### 1.1.	Virtual Machine (VM) Installation

This procedure describes how to install the virtual machine in system. VM is mandatory for installing ownCloud server. 

A virtual machine is a digital version of a physical computer. Virtual machine software can run programs and operating systems, store data, connect to networks, and do other computing functions. It allow to run an operating system in an app window on the desktop that behaves like a full and separate computer and it allows multiple operating systems (OS) environments to exist simultaneously on the same machine.

The one of the main reason to install the ownCloud in virtual machine is simple deployment and speed.

**Step 1:** Go to the website https://www.virtualbox.org/ in the browser.

**Step** 2: Click **Download VirtualBox 6.1** icon from the main page or select **Downloads** from the option list, it is present left side corner of the page.

**Step 3:** Select required platform packages from the list.

> **Note:** Windows hosts has used for this procedure.

![](ownCloud%20Images/VB%20package%20selection.png)

**Step 4:** After selection, the file started to download in the system. 

> **Note:** After download is successful, save the file to the required folder from the download folder, if required.

**Step 5:** Double-click on the downloaded file.

> **Note:** Oracle VM VirtualBox 6.1.22 type of virtual machine is used for this procedure.

**Step result:** **Oracle VM VirtualBox 6.1.22** Setup dialog box opens.

**Step 6:** Click **Next**.
 
 ![](ownCloud%20Images/VB%20setup%20popup.png)
 
**Step result:** Second dialog box opens with another set of options.

**Step 7:** By Default, VirtualBox Application is selected, if required user can change the settings. If not, proceed with default settings and click **Next**. 

![](ownCloud%20Images/VB%20setup%202.png)
 
**Step 8:** By default, all the check boxes are selected. User can deselects the check box if they do not required any given option, then click **Next**.

![](ownCloud%20Images/VB%20setup%203.png)

**Step result:** Dialog box opens with the warning message.

**Step 9:** Read the message and click **Yes**.
 
![](ownCloud%20Images/VB%20Setup%204.png)

**Step 10:** Click **Install**.
 
![](ownCloud%20Images/Step%20up%205.png)

**Step result:** **Windows Security** dialog box opens.

**Step 11:** Click **Install**.

> **Note:** Make sure **Always trust software from “Oracle Corporation”** check box is selected.

 ![](ownCloud%20Images/Set%20up%206.png)
 
**Step 12:** Click **Finish**.

![](ownCloud%20Images/VB%20Setup%207.png)
 
**Step result:** Virtual machine successfully installed in the system.

## 1.2.	Install and configure an ownCloud server

This procedure describes how to install and configure the ownCloud server.

**Prerequisite:** Need to install Virtual Machine (VM) to start with the procedure. Refer task Virtual Machine (VM) Installation for VM installation.

**Step 1:** Go to the website https://owncloud.com in the browser. 

**Step 2**: Select **Get started** option from the given list.

![](ownCloud%20Images/Getstarted.png)
 
**Step 3:** Select **install options**.

![](ownCloud%20Images/See%20Install%20Options.png)
 
**Step 4:** Select **Virtual Box**.

> **Note:** Virtualbox (ownCloud server 10.7 version) appliance is taken for this procedure.

![](ownCloud%20Images/Virtual%20Box.png)
 
**Step result:** The Virtual Box file starts to download in the system and after the successful download save the file in required location. 

> **Note:** The file size is around 1.85 GB, so the download may take some time with respect to the network speed.

**Step 5:** Open the virtual machine application.

**Step 6:** Click **Import** option from the given list.

![](ownCloud%20Images/VM%20Export%20option.png)
 
**Step result:** **Import Virtual Appliance** dialog box opens.

**Step 7:** Select the ownCloud appliance file from the folder and click **Next**.

![](ownCloud%20Images/Imoprt%20virtual%20file.png)
 

**Step 8:** Select the required folder from Machine Base Folder field and then click **Import**.

![](ownCloud%20Images/VM%20export%20option%201.png)
 
**Step result:** **Software License Agreement** dialog box opens.

**Step 9:** Click **Agree**.

![](ownCloud%20Images/Software%20License%20Agreement.png)
 
**Step result:** The file gets imported successfully. 

> **Note:** If user wants to install an ownCloud appliance in their domain after removing an existing one, they have to remember to remove the original one from the DNS configuration.

**Step 10:** Select **Start** button.

![](ownCloud%20Images/Start%20button.png)
 
**Step result:** **ownCloud** dialog box opens.

**Step 11:** Choose the language and enter the nearby city and then click **Next**.

> **Note:** Currently two language options are available one is English and other is Deutsch. Selecting nearby city helps to prefigure settings such as time zone, system language, keyboard, and layout.

![](ownCloud%20Images/ownCloud%20dialog%20box%201.png)

**Step 12:** Select the required default system locale, time zone, and keyboard layout from respective field’s drop-down and then click **Next**.

> **Note:** These settings get set by default if the user enters their city in the previous screen.

![](ownCloud%20Images/ownCloud%20dialog%20box%202.png)

**Step 13:** Click **Next**.

> **Note:** In this screen, user shall see the automatically obtained network configuration if user has a DHCP server in their network. If not, user will have to set this themself. The user can also enter an alternate DNS server if they need one. IP address is masked here for security reasons.

![](ownCloud%20Images/Domain%20and%20network%20configuration%20with%20blur.png)

**Step 14:** By default, **Manage users and permissions directly on this system** option is selected, user can proceed with that option if they do not have deep knowledge about “Microsoft Active directory and the Univention”, to proceed with the above option the user has to click **Next**.

![](ownCloud%20Images/Domain%20setup.png)

**Step 15:** Enter user organization name, email address, and set password in respective fields then click **Next**.

> **Note:** Remember the password, it is the root password for the appliance. Make sure you use a real, working email address you can access for it and used to activate the Univention Corporate Server so the user have access to the Univention App Center.

![](ownCloud%20Images/Account%20Information.png)

**Step 16:** If required, change the fully qualified domain name and LDAP base. If not, click **Next** to proceed with default FQDN and LDAP base.

![](ownCloud%20Images/Host%20Setting.png)

**Step 17:** Click **CONFIGURE SYSTEM**.

> Note: **Update system after setup** check box is selected by default. User can apply the updates later on if they choose to skip it during the installation, because the installation will take longer time to finish.

![](ownCloud%20Images/confirm%20configuration%20setting.png)

**Step result:** Setup started to install and wait until the setup is finished.

![](ownCloud%20Images/configure%20loading.png)

**Step 18:** Click **Finish** to complete the installation.

![](ownCloud%20Images/Setup%20success.png)

**Step result:** The virtual machine display the IP address to navigate in order to activate the appliance.

![](ownCloud%20Images/owncloud%20appliance.png)

**Step 19:** Enter your ownCould URL in browser.

**Step 20:** Enter email address then click **Request Activation**.

![](ownCloud%20Images/License%20Request.png)

**Step result:** License file will send to mentioned email address shortly to activate the appliance. Save that file into desired location.

> **Note:** Without activation user cannot login into the appliance. If user have entered an email address already in the configuration process, they might have already gotten an email with the Univention Corporate Server license file attached.

![](ownCloud%20Images/license%20email.png)

![](ownCloud%20Images/License%20selection.png)
 
**Step 21:** Click **Upload License File** button it will ask the license file location and select file from the saved location then click **Open**.

![](ownCloud%20Images/upload%20license.png)
 
**Step result:** File will be uploaded successfully.

**Step 22:** Click Finish to complete the activation.

![](ownCloud%20Images/License%20activation%20successful.png)
  
**Step 23:** Go to the browser and type your server IP address URL to open the ownCloud server.

**Step 24:** Click **System and domain settings** icon for create users and groups or download apps from the Univention app-center.

![](ownCloud%20Images/systems%20and%20doamin%20setting.png)

**Step 25:** Login as **Administrator** with the password which is created during the configuration wizard.

![](ownCloud%20Images/UCS%20login.png)
 
**Step result:** Univention management console screen opens like below.

![](ownCloud%20Images/UCS%20managment%20console.png)

**Step 26:** If the user need to manage the files, again login into the browser with the URL like earlier, then select ownCloud icon from the Application.

![](ownCloud%20Images/ownCloud%20portal.png)

 **Step 27:** Enter your username and password in the respective fields then click arrow mark.
 
 ![](ownCloud%20Images/user%20login%20screen.png)

**Step result:** The ownCloud server opens with default files and now the user can manage the files.

![](ownCloud%20Images/Successful%20final%20screen.png)

 **Step 28:** User also can access Admin Manual, User Manual, and Univention Blog without login credential. 
 
 ![](ownCloud%20Images/other%20options.png)


## 2. Enable users to connect to the ownCloud server using the server's IP address and port 8080

### 2.1. Installing Ubuntu OS in Virtual Box VM

This procedure describes how to enable users to connect to the ownCloud server using the server's IP address and port 8080.

**Step 1:** Go to the **https://Ubuntu.com website -> download ->Ubuntu Desktop and download 20.04 LTS version OS ->click download button** and ISO file started to download on local machine and after download completed save the file in required location.

**Step 2:** Click **New** tab.

![](ownCloud%20Images/adding%20new%20OS.png)
 
**Step 3:** Enter the following details in the screen.

**a.**	Enter required name in the **Name** field.

**b.**	Select VM located folder in **Machine Folder** field.

**c.**	Select Linux in Type **field**.

**d.**	Select **Ubuntu (64 -bit)** in **Version** field.

**e.**	Click **Next**.

![](ownCloud%20Images/add%20OS%20screen.png)
 
**Step 4**: Select required memory size by dragging blue arrow icon then click **Next**.

![](ownCloud%20Images/Memory%20Size.png)
 
**Step 5:** Select required hard disk option from given the list then click **Create**.

![](ownCloud%20Images/Hard%20disk%20seelection.png)

**Step 6:** Select required hard disk file type from the given type then click **Next**.

![](ownCloud%20Images/hard%20disk%20file%20type.png)
 
**Step 7:** Read the instructions about dynamically allocated and fixed size from the screen and select required type then click **Next**.

![](ownCloud%20Images/storage%20on%20physical%20hard%20disk.png)
 
**Step 8:** Click the folder icon to select required file location and move the blue arrow mark to choose the memory size of the virtual hard disk.

![](ownCloud%20Images/File%20location%20and%20size.png)
 
**Step result:** Ubuntu version 20.04 successfully added in the Virtual machine.

![](ownCloud%20Images/Uduntu%20installed%20screen.png)

**Step 9:** Select **Settings** tab.

![](ownCloud%20Images/settings.png)

**Step 10:** Settings dialog box opens with **General** with **Basic** tab selected by default.

![](ownCloud%20Images/general%20settings.png)

**a.**	Leave the basic settings as it is.

![](ownCloud%20Images/General%20with%20Basic%20Settings.png)

**b.**	Change **Bidirectional** in Shared Clipboard and **Drag’n’Drop** fields in Advanced settings. It is allow the user to share the files between host machine and virtual machine.

![](ownCloud%20Images/general%20with%20advance%20settings.png)

**c.**	Enter required descriptions in the **Description** field.

![](ownCloud%20Images/description.png)

**d.**	If required, select **Enable Disk Encryption** check and change the disk encryption then set password in respective fields.

![](ownCloud%20Images/disk%20encription.png)

 > **Note:** User can change the other settings as per the requirement. But selecting downloaded Ubuntu file in storage settings is the mandatory action.
 
**Step 11:** Go to the Storage tab and select **Empty -> Optical Drive CD icon -> Choose a disk file…** then choose the location where the downloaded Ubuntu file is located and click **OK**.

![](ownCloud%20Images/storage.png)
 
**Step 12:** Click **Start** tab from the VM.

![](ownCloud%20Images/Start%20tab.png)
 
**Step 13:** Click **Start** to initiate Ubuntu.

![](ownCloud%20Images/Ubuntu%20start%20screen.png)

**Step 14:** Select required language and click Install **Ubuntu**.

![](ownCloud%20Images/install%20ubuntu.png)

**Step 15:** Select required language for the keyboard and click **Continue**.

![](ownCloud%20Images/selecte%20language.png)
 
**Step 16:** If required, change the settings or proceed with default options then click **Continue**. 

![](ownCloud%20Images/updates.png)
 
**Step 17:** Proceed with the default setting **Erase disk and install Ubuntu** because this OS is going to install in the VM not in the physical machine or select **Something else** if user want to do a partitions.

![](ownCloud%20Images/installation%20type.png)

**Step 18:** Click **Continue** to proceed further. 

![](ownCloud%20Images/changes%20to%20disks.png)

**Step 19:** Select your location and click **Continue**.

![](ownCloud%20Images/location.png)

**Step 20:** Enter your name, computer name, user name, and set password in the respective field then click **Continue**.

![](ownCloud%20Images/user%20name%20and%20password.png)
 
**Step 21:** Click **Restart Now** to restart the Ubuntu OS.

![](ownCloud%20Images/installation%20complete.png)
 
**Step 22:** Press **Enter** to start the Ubuntu OS.

![](ownCloud%20Images/enter.png)
 
**Step 23:** Click on the user name and enter the password which is created during the installation and press enter.

![](ownCloud%20Images/ubuntu%20user%20name%20and%20password.png)
 
**Step 24:** Welcome window opens, click **Skip** (4 times).

![](ownCloud%20Images/welcome%20window.png)
 
**Step 25:** Finally click **Done**.

![](ownCloud%20Images/done.png)
 
**Step 26:** If you want do install software click **Install Now** or click **Remind Me Later**.

![](ownCloud%20Images/sofware%20update.png)
 
**Step result:** Ubuntu OS version 20.04 installed successfully in the VM.

![](ownCloud%20Images/ubuntu%20launch%20screen.png)
 
 
## 3. Adding User Account in the ownCloud Server

This procedure describes how to add the user account as an administrator.

**Step 1:** Go to the browser and enter your ownCloud server URL.

**Step 2:** Enter user name and password in the respective field then press arrow mark.

![](ownCloud%20Images/user%20login%20screen.png)

**Step 3:** Click **Administrator** tab then select **Users** from the drop down.

![](ownCloud%20Images/Select%20user.png)
 
**Step 4:** Enter username, email id, and select required group from the respective field then click **Create**.

![](ownCloud%20Images/user%20admin%20screen.png)
 
**Step result:** The new user added in the list. 

**Step 5:** Click pencil icon to edit user full name and password, if required.

**Note:** Username is not editable.

![](ownCloud%20Images/user%20name%20edit.png)
 
**Step 6:** From the **Groups** tab user can be changed from existing group to another groups or user can be added in new group by clicking **+ add group**.

**Sub step:** Click **+ add group**, editable field opens, enter required group name and press enter. 

**Step result:** The user has added in the created group.

![](ownCloud%20Images/group%20change.png)
 
**Step 7:** From **Group Admin for** tab, user can be changed as admin for any created group. If it is not required, leave as no group.

![](ownCloud%20Images/group%20admin.png)
 
**Step 8:** Click **Quota** tab and select required memory storage for particular user from the drop down.

**Sub step:** Click Others to enter customized storage quota, values between 512 MB to 12 GB are the allowable range.

![](ownCloud%20Images/user%20quota.png)
 
**Step 9:** Click **+ Add Group** and enter required group name then press enter, the new group has added in the group list.
Note: This is another method of adding the group.

![](ownCloud%20Images/add%20group.png)
 
**Step 10:** If created user needs to be deleted, move the cursor to the right side corner of that particular user account and click delete icon to delete the created user.

![](ownCloud%20Images/delete%20user.png)


## 4. Connecting ownCloud server by using a desktop or mobile client

### 4.1. Connecting ownCloud server by using a desktop client

This procedure describes how to connect ownCloud server by using desktop client and this helps to synchronize files between ownCloud server and local desktop automatically.

**Step 1:** Go to the website https://owncloud.com in the browser. 

**Step 2:** Select **Get started** option from the given list. 

**Step 3:** Select **Download Desktop App**.

![](ownCloud%20Images/Download%20Desktop%20APP.png)

**Step 4:** Choose required operating system (OS) and click **Download**.

**Step result:** The file is started to download in the system.

> **Note:** Setup available for Windows, Mac OS, and Linux and Windows desktop setup has taken for this procedure.

![](ownCloud%20Images/Windows%20Selection.png)

**Step 5:** Double click the downloaded file.

**Step result:** **ownCloud Setup** dialog box opens.

**Step 6:** Click **Next**.

![](ownCloud%20Images/windows%20setup.png)
 
**Step 7:** If required, change the settings as per user requirement. If not, proceed with default settings then click **Next**.

![](ownCloud%20Images/windows%20setup%201.png)
 
**Step 8:** Click **Install**.

![](ownCloud%20Images/windows%20setup%202.png)
 
**Step 9:** Select **Launch ownCloud after finish** check box if required then click **Finish**.

![](ownCloud%20Images/windows%20setup%20finish.png)

**Step 10:** Enter the URL of ownCloud server in Server Address field then click **Next**. 

![](ownCloud%20Images/windows%20server%20address.png)
 
**Step 11:** Select **Trust this certificate anyway** check box then click **OK**.

![](ownCloud%20Images/windows%20untrusted%20certificate.png)
 
**Step 12:** Enter the username and password in the respective fields then click **Next**.

![](ownCloud%20Images/windows%20username%20and%20password.png)

**Step 13:** Select required given option from the screen then click **Continue…**.

**a.**	Use virtual files instead of downloading content immediately – This option helps to manage the virtual files from the desktop app.

**b.**	Synchronize everything from server (recommended) (7.2 MB) – This option helps to sync all the data between the server and desktop app.

**c.**	Manually create folder sync connections – This option helps the user to sync connections and folder creation manually.

![](ownCloud%20Images/windows%20connect%20screen.png)
 
**Step result:** ownCloud server synchronized with the Windows app.

**Step 14:** Click triple dot icon and select **Open folder**.

![](ownCloud%20Images/windows%20open%20folder.png)

**Step result:** Local system folder opens with default files and it is synchronized with the ownCloud server and user can manage their files by using the Windows desktop client.

![](ownCloud%20Images/windows%20folder%20sync.png)

 
### 4.2. Connecting ownCloud server by using a mobile client

This procedure describes how to connect ownCloud server by using mobile app. The app is help to synchronized user mobile with the ownCloud server. So the user can manage the date from their mobile app. 

**Step 1:** Go to the website https://owncloud.com in the browser.

**Step 2:** Select **Get started** option from the given list.

**Step 3:** Select **Download Mobile App**.

![](ownCloud%20Images/mobile%20app.png)

**Step 4:** Select required Mobile OS.

> **Note:** Android OS setup taken for this procedure. IOS setup also available for the user.

![](ownCloud%20Images/mobile%20OS.png)
 
**Step result:** This page will redirect into the Google Play Store page.

> **Note:** This is a paid App, in which the user has to be pay the mentioned amount via method of payments mentioned to install the ownCloud App.

**Step 5:** After the installation, open the app and enter ownCloud URL in the **ownCloud URL** field.

> **Note:** User can download the ownCload file in desktop then they can copy that file into the mobile then it can be installed in the mobile or user can directly download and install the ownCload file from google paly store from the mobile.

**Step 6:** Enter username and password in the respective **Login details** field then click **Connect**.

![](ownCloud%20Images/mobile%20login.png)
 
**Step result:** ownCloud android app synchronized with the ownCloud server. Now the user can manage their files by using the android mobile app.

![](ownCloud%20Images/mobile%20synced.png)

--- 

**End of the guide**

Created by **Mansoor Ali**




  


 





