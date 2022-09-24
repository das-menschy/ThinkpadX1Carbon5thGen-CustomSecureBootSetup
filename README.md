# EN: How to setup laptop with SecureBoot and LUKS
# DE: Einrichten eines Laptops mit SecureBoot und LUKS 

* EN: Here I am collecting my scripts and firmware screenshots that document how I setup my Thinkpad X1 Carbon 5th Generation (20HR002MMX) with custom, personal Secure Boot certificates, running ArchLinux, LinuxMint and Windows10Home / Windows10Pro. 
* DE: Hier sammle ich meine Skripts und Firmware-Bildschirm-Fotos, die dokumentieren, wie ich mein Thinkpad X1 Carbon 5te Generation (20HR002MMX) so eingerichtet habe mit persönlichen, benutzerdefinierten SecureBoot-Zertifikaten, dass darauf sowohl ArchLinux, LinuxMint als auch Windows10Home / Windows10Pro als Betriebssystem laufen. 

## EN: 1. ADDING A UEFI-BIOS FIRMWARE PASSWORD
## DE: 1. HINZUFÜGEN EINES UEFI-BIOS FIRMWARE PASSWORTES

* EN: In order to protect the UEFI / BIOS firmware settings, so that Secure Boot cannot be turned off without a password, it is wise to protect the UEFI / BIOS firmware settings with a password, called "Supervisor Password". 
* DE: Um die UEFI / BIOS Firmware-Einstellungen zu schützen, sodass SecureBoot nicht einfach wieder deaktiviert werden kann ohne ein Passwort, ist es ratsam, die UEFI / BIOS Firmware-Einstellungen mit einem Passwort zu schützen. Dieses Passwort wird "Supervisor Passwort" genannt. 
