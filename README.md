# CMPQuickTests (CMP Quick Tests available for Orlando relase)
Used to automate testing processes of creating virtual machines, disks etc.

*This is example of Azure Disk/VM creation

Before you start please provide basic configuratuon for Cloud Management. Necessary to create:

* Cloud User (with required rorles)
* MIDServer
* Credential for Azure Cloud (Azure Principal)
* Service Account
* Cloud Accoung
* Resirce Profiles (OS Profile, Profile Compute)
* existing resource group
* Cloud Catalog Item (with ARM tempalte Version)

This test starts from *updateing defult values of cloud variables* which will autoppulate the field on *Cloud User Portal form*. You can make this same by creating tests step *Set Variable Value(sp)* after *Open Form (SP)* step. *Impersonate* user who represents the client. Opens *User Cloud Portal* and choose a desired *Cloud Catalog Item*. *Submit a Form(SP)*. Check if the Stack has been created. *Impersonate * back admin.
