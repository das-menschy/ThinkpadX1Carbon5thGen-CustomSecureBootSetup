# EN: How to setup laptop with SecureBoot and LUKS
# DE: Einrichten eines Laptops mit SecureBoot und LUKS 

* EN: Here I am collecting my scripts and firmware screenshots that document how I setup my Thinkpad X1 Carbon 5th Generation (20HR002MMX) with custom, personal Secure Boot certificates, running ArchLinux, LinuxMint and Windows10Home / Windows10Pro. 
* DE: Hier sammle ich meine Skripts und Firmware-Bildschirm-Fotos, die dokumentieren, wie ich mein Thinkpad X1 Carbon 5te Generation (20HR002MMX) so eingerichtet habe mit persönlichen, benutzerdefinierten SecureBoot-Zertifikaten, dass darauf sowohl ArchLinux, LinuxMint als auch Windows10Home / Windows10Pro als Betriebssystem laufen. 

## EN: 1. ADDING A UEFI-BIOS FIRMWARE PASSWORD
## DE: 1. HINZUFÜGEN EINES UEFI-BIOS FIRMWARE PASSWORTES

* EN: In order to protect the UEFI / BIOS firmware settings, so that Secure Boot cannot be turned off without a password, it is wise to protect the UEFI/BIOS firmware settings with a password, called "Supervisor Password". 
* DE: Um die UEFI / BIOS Firmware-Einstellungen zu schützen, sodass SecureBoot nicht einfach wieder deaktiviert werden kann ohne ein Passwort, ist es ratsam, die UEFI/BIOS-Firmware-Einstellungen mit einem Passwort zu schützen. Dieses Passwort wird "Supervisor Passwort" genannt. 

* EN: Press the power button of your laptop and shortly (!) after that the UEFI-BIOS Setup key(s), which are dependant on your PC manufacturer and model: 
* DE: Drücken Sie den Ein/Aus-Schalt-Knopf und sehr schnell (!) danach die UEFI-BIOS-Einrichtungs-Taste(n), die für jeden PC-Hersteller und jedes PC-Modell anders ist oder sind: 

| EN: UEFI/BIOS Setup key                | EN: Manufacturer or model          |
|:-------------------------------------- |:---------------------------------- |
| **DE: UEFI/BIOS-Einrichtungs-Taste**   | **DE: Hersteller oder Modell**     |
| <kbd>F1</kbd>                          | Lenovo Desktop, Lenovo Thinkpads   |
| <kbd>F2</kbd>                          | ASRock, ASUS, Acer, Dell, Gigabyte,|
|                                        | Lenovo Laptops, Toshiba, Samsung,  |
|                                        | Origin PC,                         |
| <kbd>F10</kbd>                         | HP                                 |
| <kbd>F12</kbd>                         | Toshiba Equium                     | 
| <kbd>DEL</kbd> / <kbd>ENTF</kbd>       | ASRock, ASUS, ECS, Gigabyte/Aorus, |
|                                        | MSI, Zotac                         |
| <kbd>Power</kbd> + <kbd>VolumeUp</kbd> | Microsoft Surface                  | 

* EN: On many PC's, there is also a UEFI/BIOS Interrupt menu that can be opened by pressing an Interrupt key during boot.  
* DE: Auf vielen PC's gibt es auch ein UEFI/BIOS-Unterbrechungs-Menü, das durch Drücken der Unterbrechungs-Taste während dem Boot-Vorgang aufgerufen werden kann. 
* EN: This UEFI/BIOS Interrupt menu explains which keys are available to open the different UEFI/BIOS options. 
* DE: Dieses UEFI/BIOS-Unterbrechungs-Menü erklärt, welche UEFI/BIOS-Optionen über die Tasten zur Verfügung stehen. 
* EN: This key which opens the UEFI/BIOS Interrupt menu is also different for every manufacturer or model: 
* DE: Diese Taste, die das UEFI/BIOS-Unterbrechungs-Menü öffnet, ist auch für jeden Hersteller und jedes Modell unterschiedlich: 

| EN: UEFI/BIOS Interrupt menu key       | EN: Manufacturer or model          |
|:-------------------------------------- |:---------------------------------- |
| **DE: UEFI/BIOS-Unterbrechungs-Taste** | **DE: Hersteller oder Modell**     |
| <kbd>ENTER</kbd> / <kbd>EINGABE</kbd>  | Lenovo Thinkpad                    | 

* EN: When the following boot screen is displayed, press the UEFI/BIOS Setup key or UEFI/BIOS Interrupt menu key:  
* DE: Wenn der folgende Boot-Startbildschirm angezeigt wird, drücken Sie die UEFI/BIOS-Einrichtungs-Taste oder die UEFI/BIOS-Unterbrechungs-Taste: 

![00_Startup_-_01_Boot_Screen.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/00_Startup_-_01_Boot_Screen.png) 

* EN: The UEFI/BIOS Interrupt menu will look similar to his: 
* DE: Das UEFI/BIOS-Unterbrechungs-Menü sieht so ähnlich aus wie dieses: 

![00_Startup_-_02_Interrupt_Menu.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/00_Startup_-_02_Interrupt_Menu.png) 

* EN: Press the UEFI/BIOS Setup key now. 
* DE: Drücken Sie nun die UEFI/BIOS-Einrichtungs-Taste. 

* EN: When the UEFI/BIOS Setup program is opened, the Main screen will look similar to this: 
* DE: Wenn das UEFI/BIOS-Einrichtungs-Programm geöffnet ist, sieht der Hauptbildschirm so ähnlich wie dieser aus: 

![BIOS_Setup_-_01_Main_Screen_-_Version_N1MET70W_SecureBoot_on.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_01_Main_Screen_-_Version_N1MET70W_SecureBoot_on.png)  

* EN: Inside the UEFI/BIOS Setup program, navigate to the **"Security"** tab by pressing the RIGHT-ARROW <kbd>→</kbd> key three times: 
* DE: Navigieren Sie im UEFI/BIOS-Einrichtungs-Programm zum **"Security"**/Sicherheits-Tab, indem Sie die Pfeil-Taste nach rechts <kbd>→</kbd> auf ihrer Tastatur dreimal drücken: 

![BIOS_Setup_-_02_Config.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_02_Config.png) 
![BIOS_Setup_-_03_Date_and_Time.03s-passed.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_03_Date_and_Time.03s-passed.png) 
![BIOS_Setup_-_04_Security_-_01_Password_-_00.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_04_Security_-_01_Password_-_00.png) 

* EN: In the **"Security"** tab on the **"Password"** menu option, press **<kbd>ENTER</kbd>** to open the UEFI/BIOS password settings. 
* DE: Drücken Sie im **"Security"**/Sicherheits-Tab auf der **"Password"**/Passwort-Option die **<kbd>ENTER</kbd>/<kbd>EINGABE</kbd>**-Taste, um die UEFI/BIOS-Passwort-Einstellungen zu öffnen: 

![BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_00_Disabled.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_00_Disabled.png) 

* EN: When the UEFI/BIOS Supervisor Password is "Disabled" as shown, you can press <kbd>ENTER</kbd> to set a UEFI/BIOS Supervisor Password: 
* DE: Wenn das UEFI/BIOS Supervisor Password "Disabled"/"deaktiviert" ist, drücken Sie die <kbd>ENTER</kbd>/<kbd>EINGABE</kbd>-Taste, um ein UEFI/BIOS-Supervisor-Passwort festzulegen: 

![BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_01_Enter_New_Password_-_00_letters.gif](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_01_Enter_New_Password_-_00_letters.gif)

* EN: Now type in the UEFI/BIOS Supervisor Password and press <kbd>ENTER</kbd> when finished: 
* DE: Tippen Sie nun das UEFI/BIOS-Supervisor-Passwort ein und drücken Sie die <kbd>EINTER</kbd>/<kbd>EINGABE</kbd>-Taste, wenn Sie fertig sind: 

![BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_01_Enter_New_Password.gif](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_01_Enter_New_Password.gif)

* EN: Type in the UEFI/BIOS Supervisor password one more time to confirm it. Press <kbd>ENTER</kbd> when finished: 
* DE: Tippen Sie das gewünschte UEFI/BIOS-Supervisor-Passwort noch einmal ein und drücken Sie die <kbd>ENTER</kbd>/<kbd>EINGABE</kbd>-Taste, um zu bestätigen: 

![BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_02_Confirm_New_Password.gif](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_02_Confirm_New_Password.gif)

* EN: If the two UEFI/BIOS Supervisor passwords that you entered match together, then you should get a UEFI/BIOS Setup Notice saying that the "Changes have been saved". Press <kbd>ENTER</kbd> to **"continue"**. 
* DE: Wenn die zwei UEFI/BIOS-Supervisor-Passwörter, die Sie eingegeben haben, übereinstimmen, dann sollte nun ein UEFI/BIOS-Einrichtungs-Hinweis erscheinen, der sagt: "Changes have been saved" (Ihre Änderungen wurden gespeichert). Drücken Sie die <kbd>ENTER</kbd>/<kbd>EINGABE</kbd>-Taste, um fortzufahren. 

![BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_03_Changes_have_been_saved.png](00_ADD_SUPERVISOR_PASSWORD_ON_NEW_PC/BIOS_Setup_-_04_Security_-_01_Password_-_01_Supervisor_Password_-_03_Changes_have_been_saved.png) 
